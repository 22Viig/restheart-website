---
title: User Management
layout: docs
---

<div markdown="1" class="d-none d-xl-block col-xl-2 order-last bd-toc">

* [Introduction ](#introduction)
* [User document](#user-document)
* [Get existing users](#get-existing-users)
* [Create a user](#create-a-user)
* [Update a user](#update-a-user)
* [Delete a user](#delete-a-user)

</div>
<div markdown="1" class="col-12 col-md-9 col-xl-8 py-md-3 bd-content">

{% include docs-head.html %} 

## Introduction 

This section provides instructions on how to create, update and delete users for the default [RESTHeart Authenticator](/docs/security/authentication/#restheart-authenticator).

{: .bs-callout.bs-callout-info}
**RESTHeart Authenticator** uses the collection `/users` by default.

### Before running the example requests

The following examples assume RESTHeart Platform running on the localhost with the default configuration: the database *restheart* is bound to `/` and the user *admin* exists with default password *secret*.

## User document

With the default configuration, a user is represented as follows:

{: .black-code}
```
{
    "_id": "username",
    "roles": [ "list", "of", "roles" ],
    "password": "secret"
}
```

{: .bs-callout.bs-callout-info}
**RESTHeart Authenticator** can be configured to use different properties for the username, roles an password. Check [RESTHeart Authenticator](/docs/security/authentication/#restheart-authenticator) for more information.

## Get existing users

{% include code-header.html type="Request" 
    link="http://restninja.io/share/b6876216ee3fb0999f7c5178e42a7978f6cc3c4c/0"
%}

{: .black-code}
```
GET /users HTTP/1.1
```

{% include code-header.html type="Response" %}

{: .black-code}
```
[
  {
    "_id": "admin",
    "roles": [
      "admin"
    ],
    "_etag": {
      "$oid": "5d2edb155883c050065d6a8a"
    }
  }
]
```

{: .bs-callout.bs-callout-info}
The password is always hidden on GET requests.

{: .bs-callout.bs-callout-warning}
For security reasons, it not possbile to use the `filter` query parameter on the password field; the following request is forbidden and will cause an error: `GET /users?filter={"password":{"$regex":"^a.*"}}`

## Create a user

{% include code-header.html type="Request" 
    link="http://restninja.io/share/38c1eb85a21213dd39192ccd474789f4abdbd6bc/0"
%}

{: .black-code}
```
POST /users HTTP/1.1

{
    "_id": "foo",
    "roles": [ "user" ],
    "password": "secret"
}
```

{: .bs-callout.bs-callout-info}
The password is automatically encrypted by RESTHeart Platform.

## Update a user

{% include code-header.html type="Request" 
    link="http://restninja.io/share/3e541e5b4f1ce82ae255b8f6746d49f5faed9778/0"
%}

{: .black-code}
```
PATCH /users/foo HTTP/1.1

{
    "password": "betterSecret"
}
```

## Delete a user

{% include code-header.html type="Request" 
    link="http://restninja.io/share/ae4858bc59f5ac755f03dc8858220e0a470a3779/0"
%}

{: .black-code}
```
DELETE /users/foo HTTP/1.1
```