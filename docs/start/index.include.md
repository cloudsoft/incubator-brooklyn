## What is Brooklyn?

**brooklyn** is a library that simplifies application deployment and management.

For **deployment**, it is designed to tie in with other tools, 
giving single-click deploy and adding the concepts of 
manageable clusters and fabrics:

* many common software entities available out-of-the-box
* integrates with [Apache Whirr](http://whirr.apache.org) -- and thereby Chef and Puppet --
  to deploy well-known services such as Hadoop and elasticsearch
  (or use POBS, plain-old-bash-scripts)
* use PaaS's such as OpenShift, alongside self-built clusters, for maximum flexibility

Brooklyn makes roll-out an integral part of the DevOps chain,
as code which can be version-controlled and automatically tested,
and portable across many clouds or fixed IP machines,
using [jclouds](http://jclouds.org),
or just hitting ``localhost`` for quick dev/test.

Brooklyn's main emphasis is post-deployment, **managing** an application once it is live:
management policies are an integral part of the deployment descriptor,
and at runtime have access to all aspects of the deployment.
They are aware of the deployment topology (hierarchical) and locations (machines, PaaSes, and jurisdictions), 
as well as launch mechanisms, instrumentation from managed entities or third-party systems,
and operational goals and constraints.
This means they're all set, once the application is launched, to keep the application running optimally,
based on whatever *optimally* means for a particular application.

These deployment patterns and management policies are expressed as Java (and Groovy) classes,
open-sourced here, and giving you full control over what you want to happen.
More importantly, however, this code can be shared, improved, and extended.

We're still near the beginning of figuring this out: 
[join us to make it better]({{site.url}}/meta/contact.html).


## To Get Started

* See the [developer's walkthrough]({{site.url}}/start/walkthrough/index.html) for a quick tour
* Dive in to the [user guide]({{site.url}}/use/guide/) describing the 
  [concepts]({{site.url}}/use/guide/defining-applications/basic-concepts.html)
  and including a [tutorial]({{site.url}}/use/guide/quickstart/).
* Or jump straight in to the [code]({{site.url}}/dev/code/), 
  including [examples]({{site.url}}/use/examples/), or other [documentation]({{site.url}}/start/docs-summary.html).

If you like it, or if you have ideas how it could be better,
[join the discussion]({{site.url}}/meta/contact.html).