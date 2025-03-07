---
title: Editions
layout: page-notitle
---

<div class="editions-matrix mt-5">
    <div class="comparison">

  <table>
    <thead>
      <tr>
        <th class="tl tl2"></th>
        <th colspan="3" class="qbse">
          <strong>Features</strong>
        </th>
        <th colspan="1" style="border-right: 0; border-top: 0">
        </th>
      </tr>
      <tr>
        <th class="tl"></th>
        <th class="compare-heading p-3">
          <div class="d-flex flex-column flex-md-row justify-content-center mb-2 w-100">
            <div><a href="https://github.com/SoftInstigate/restheart"><img class="img-fluid mr-md-2" src="/images/octocat.png" width="20"></a></div>
            <a class="mt-auto" href="{{ "/faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>OSS</strong> </a>
          </div>
          <a style="font-weight: 100" href="{{ "/faq/#letter-to-os-users" | prepend: site.baseurl }}">Letter to OS Users</a>
        </th>
        <th class="compare-heading restheart-version p-3">
          <a href="{{ "/faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>Platform PE</strong></a>
        </th>
        <th class="compare-heading restheart-version p-3">
          <a href="{{ "/faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>Platform EE</strong></a>
        </th>
        <th class="compare-heading restheart-version p-3">
          <a href="{{ "/faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>Platform OEM</strong></a>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td></td>
        <td colspan="4">REST API for admin operations (manage <a href="/docs/mgmt/dbs-collections/" class="text-dark">databases, collections</a>, <a href="/docs/mgmt/indexes/" class="text-dark">indexes</a>, <a href="/docs/mgmt/relationships/" class="text-dark">relationships</a>)</td>
      </tr>
      <tr class="compare-row">
        <td>REST API for admin operations (manage <a href="/docs/mgmt/dbs-collections/" class="text-dark">databases, collections</a>, <a href="/docs/mgmt/indexes/" class="text-dark">indexes</a>, <a href="/docs/mgmt/relationships/" class="text-dark">relationships</a>)</td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/read-docs/" class="text-dark">REST API for Create Read Update Delete</a></td>
      </tr>
      <tr>
        <td><a href="/docs/read-docs/" class="text-dark">REST API for Create Read Update Delete</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/write-docs/#bulk-write-requests" class="text-dark">Bulk write operations</a></td>
      </tr>
      <tr class="compare-row">
        <td><a href="/docs/write-docs/#bulk-write-requests" class="text-dark">Bulk write operations</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/aggregations/" class="text-dark">Aggregations and Map-Reduce operations</a></td>
      </tr>
      <tr>
        <td><a href="/docs/aggregations/" class="text-dark">Aggregations and Map-Reduce operations</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4">Plugins (<a href="/docs/services/" class="text-dark">Services</a>, <a href="/docs/transformers/" class="text-dark">Transformers</a>, <a href="/docs/checkers/" class="text-dark">Checkers</a> and <a href="/docs/hooks/" class="text-dark">Hooks</a>)</td>
      </tr>
      <tr class="compare-row">
        <td>Plugins (<a href="/docs/services/" class="text-dark">Services</a>, <a href="/docs/transformers/" class="text-dark">Transformers</a>, <a href="/docs/checkers/" class="text-dark">Checkers</a> and <a href="/docs/hooks/" class="text-dark">Hooks</a>)</td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/json-schema-validation/" class="text-dark">JSON Schema data validation and enforcement</a></td>
      </tr>
      <tr>
        <td><a href="/docs/json-schema-validation/" class="text-dark">JSON Schema data validation and enforcement</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/csv/" class="text-dark">Bulk data import, uploading CSV files from Excel</a></td>
      </tr>
      <tr class="compare-row">
        <td><a href="/docs/csv/" class="text-dark">Bulk data import, uploading CSV files from Excel</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/transactions/#sessions" class="text-dark">Support for MongoDB sessions</a></td>
      </tr>
      <tr>
        <td><a href="/docs/transactions/#sessions" class="text-dark">Support for MongoDB sessions</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/security/overview/" class="text-dark">Basic Security (authentication and authorization)</a></td>
      </tr>
      <tr class="compare-row">
        <td><a href="/docs/security/overview/" class="text-dark">Basic Security (authentication and authorization)</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/develop/security-plugins/" class="text-dark">Extended IAM with plugins (LDAP, AD, etc)</a></td>
      </tr>
      <tr>
        <td><a href="/docs/develop/security-plugins/" class="text-dark">Extended IAM with plugins (LDAP, AD, etc)</a></td>
        <td><span class="tickblue">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/faq/#distribute-derivative-work" class="text-dark">Can use in closed source application</a></td>
      </tr>
      <tr class="compare-row">
        <td><a href="/faq/#distribute-derivative-work" class="text-dark">Can use in closed source application</a></td>
        <td></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/security/authentication/#restheart-authenticator" class="text-dark">Identity Manager with users on MongoDB</a></td>
      </tr>
      <tr>
        <td><a href="/docs/security/authentication/#restheart-authenticator" class="text-dark">Identity Manager with users on MongoDB</a></td>
        <td></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/security/authentication/#jwt-authentication" class="text-dark">JWT Authentication</a></td>
      </tr>
      <tr class="compare-row">
        <td><a href="/docs/security/authentication/#jwt-authentication" class="text-dark">JWT Authentication</a></td>
        <td></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/change-streams/" class="text-dark">Change Streams</a></td>
      </tr>
      <tr>
        <td><a href="/docs/change-streams/" class="text-dark">Change Streams</a></td>
        <td></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/transactions/" class="text-dark">Transactions</a></td>
      </tr>
      <tr class="compare-row">
        <td><a href="/docs/transactions/" class="text-dark">Transactions</a></td>
        <td></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4"><a href="/docs/clustering/" class="text-dark">Clustering</a></td>
      </tr>
      <tr>
        <td><a href="/docs/clustering/" class="text-dark">Clustering</a></td>
        <td></td>
        <td></td>
        <td><span class="restheart-red">✔</span></td>
        <td><span class="restheart-red">✔</span></td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4">Access Manager with DSL permissions on MongoDB<</td>
      </tr>
      <tr class="compare-row">
        <td>Access Manager with DSL permissions on MongoDB</td>
        <td></td>
        <td></td>
        <td><span class="restheart-red">✔ (v4.1)</span></td>
        <td><span class="restheart-red">✔ (v4.1)</span></td>
      </tr>
    </tbody>
  </table>

</div>
</div>


<div class="editions-matrix mt-5">
    <div class="comparison">

  <table>
    <thead>
      <tr>
        <th class="tl tl2"></th>
        <th colspan="3" class="qbse">
          <strong>Licensing, Pricing, Purchase</strong>
        </th>
        <th colspan="1" style="border-right: 0; border-top: 0">
        </th>
      </tr>
      <tr>
        <th class="tl"></th>
        <th class="compare-heading restheart-version p-3">
          <div class="d-flex flex-column flex-md-row justify-content-center mb-2 w-100">
            <div><a href="https://github.com/SoftInstigate/restheart"><img class="img-fluid mr-md-2" src="/images/octocat.png" width="20"></a></div>
            <a class="mt-auto" href="{{ "/faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>OSS</strong> </a>
          </div>
          <a style="font-weight: 100" href="{{ "/faq" | prepend: site.baseurl }}">Letter to OS Users</a>
        </th>
        <th class="compare-heading restheart-version p-3">
          <a class="d-block" href="{{ "faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>Platform PE</strong></a>
        </th>
        <th class="compare-heading restheart-version p-3">
          <a class="d-block" href="{{ "faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>Platform EE</strong></a>
        </th>
        <th class="compare-heading restheart-version p-3">
          <a class="d-block" href="{{ "faq/#os-vs-pe" | prepend: site.baseurl }}"><strong>Platform OEM</strong></a>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td></td>
        <td colspan="4">Type of License</td>
      </tr>
      <tr class="compare-row">
        <td>Type of License</td>
        <td>Open Source AGPL which requires distributing source code</td>
        <td>Standard Commercial with no custom terms</td>
        <td>Enterprise License with custom terms</td>
        <td>Embedded License with custom terms</td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4">Pricing</td>
      </tr>
      <tr>
        <td>Pricing</td>
        <td>Free</td>
        <td>30-Day Free Trial then USD 499 per Deployment Instance per Year. <div class="small text-muted">VAT applies for EU customers</div></td>
        <td>Negotiable</td>
        <td>Negotiable</td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4">Purchase</td>
      </tr>
      <tr class="compare-row">
        <td>Purchase</td>
        <td>n/a</td>
        <td>Online with credit card</td>
        <td>Company Purchase Order</td>
        <td>Company Purchase Order</td>
      </tr>
      <tr>
        <td>&nbsp;</td>
        <td colspan="4">Obtain</td>
      </tr>
      <tr>
        <td>Obtain</td>
        <td><a style="font-weight: 100" href="https://github.com/SoftInstigate/restheart">GitHub Repository</a></td>
        <td>
          <a href="{{ "/get" | prepend: site.baseurl }}"><button style="1" type="button" class="pl-3 pr-3 btn btn-danger">GET</button></a>
        </td>
        <td><a href="mailto:ask@restheart.org?subject=RESTHeart EE">Contact</a></td>
        <td><a href="mailto:ask@restheart.org?subject=RESTHeart OEM">Contact</a></td>
      </tr>
    </tbody>
  </table>

</div>
</div>

{% include roi-calculator.html %}