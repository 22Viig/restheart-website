---
title: Initializers
layout: docs
---

<div markdown="1" class="col-12 col-md-9 col-xl-8 py-md-3 bd-content">

{% include docs-head.html %} 

{% include doc-in-progress.html %}

An initializer is a class with the method `init()` that is invoked at RESTHeart startup.

It can be used to perform initialization code. For instance, it can programmatically add _Transformers_ and _Checkers_ and init the db.

The Initializer class can be specified in the configuration file

{: .black-code}
``` yml
### Initializer

# A custom initializer implmenting the org.restheart.init.Initializer interface
# Can be used to inizialize data or add global transformers, checkers or security predicates
# See org.restheart.init.TestInitializer for a simple example

initializer-class: org.restheart.init.TestInitializer
```

For an example look at [org.restheart.init.TestInitializer](https://github.com/SoftInstigate/restheart/blob/master/src/main/java/org/restheart/init/TestInitializer.java)

The class must implement the `Initializer` interface

{: .black-code}
``` java
package org.restheart.init;

public interface Initializer {
    public void init();
}
```
## Best practices

### Get the MongoClient

{: .black-code}
``` java
// get the MongoClient
MongoClient client = MongoDBClientSingleton.getInstance().getClient();
```

### Add Global Transformers

> Global Transformers are applied to all requests.

See [Request Transformers](/learn/request-transformers#global-transformers) for more information on `GlobalTransformer`

{: .black-code}
``` java
GlobalTranformer globalTranformer;

// transform the request
RequestTransformerHandler.getGlobalTransformers().add(globalTranformer);

// transform the response
ResponseTransformerHandler.getGlobalTransformers().add(globalTranformer);
```

### Add Global Checkers

> Global Checkers are applied to all requests.

See [Request Checkers](/learn/request-checkers#global-checkers) for more information on `GlobalChecker`.

{: .black-code}
``` java
// check the request
GlobalChecker globalChecker;

CheckerHandler.getGlobalCheckers().add(globalChecker);
```

### Add Global Security Predicates

> Global Security Predicates are applied to all requests.

{: .black-code}
``` java
// allow users with role "ADMIN" to GET /
RequestContextPredicate securityPredicate = new RequestContextPredicate() {
            @Override
            public boolean resolve(HttpServerExchange hse, RequestContext context) {
                return context.isRoot()
                        && context.isGet()
                        && context.getAuthenticatedAccount() != null
                        && context.getAuthenticatedAccount().getRoles().contains("ADMIN");
            }
        }

// add the global predicate
AccessManagerHandler.getGlobalSecurityPredicates().add(securityPredicate);
```

