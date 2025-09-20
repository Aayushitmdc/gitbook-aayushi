---
description: >-
  Use this page as a reference to understand the end-to-end steps, the
  capabilities you need, and the DataOS components involved in building a
  production-grade Data Product.
---

# Data Product Creation

<table data-full-width="true"><thead><tr><th>Objective</th><th>Capability You Need</th><th>Capability You Need</th></tr></thead><tbody><tr><td><strong>Set up your environment</strong></td><td>Install CLI , <br>Initialize CLI, <br>Setup IDE</td><td><code>dataos-ctl</code> (CLI),  <br>VS Code (IDE)</td></tr><tr><td><strong>Connect securely to your raw data</strong></td><td>Secure source connection, credential handling</td><td><a data-footnote-ref href="#user-content-fn-1"><code>Depot</code>, <code>Instance-Secret</code></a></td></tr><tr><td><strong>Extract the metadata</strong> </td><td>Schema extraction, metadata,</td><td><code>Scanner</code></td></tr><tr><td><strong>Understand source data</strong></td><td>Unified metadata catalog, schema browsing, and lineage</td><td><code>Metis</code></td></tr><tr><td><strong>Ingest and transform data</strong></td><td>Declarative pipelines, task DAGs</td><td><a data-footnote-ref href="#user-content-fn-2"><code>Flare</code>, <code>Bento</code>, <code>Workflow</code>, <code>Service</code>, <code>Worker</code></a></td></tr><tr><td><strong>Store data for analytics and reuse</strong></td><td>Durable, scalable storage</td><td><code>Lakehouse</code>, <code>Database</code>, <code>Volume</code></td></tr><tr><td><strong>Create semantic model</strong></td><td>Logical modeling, documentation, metrics</td><td><code>Lens</code></td></tr><tr><td><strong>Ensure data quality</strong></td><td>Quality checks</td><td><code>Soda</code></td></tr><tr><td><strong>Observe and get alert for pipeline failures</strong></td><td>Detect failures, track key metrics, trigger alerts on thresholds</td><td><code>Monitor</code>, <code>Pager</code></td></tr><tr><td><strong>Secure &#x26; govern access</strong></td><td>Fine-grained access control<br>Role-based and policy-driven access control to Data Products and Resources</td><td><code>Policy</code>, <code>Bifrost</code> , <code>Grant</code></td></tr><tr><td><strong>Package and release the product</strong></td><td>Reproducible deployment of Data Product components</td><td><code>Bundle</code></td></tr><tr><td><strong>Provision computation infrastructure</strong></td><td>Define scalable, cloud-native node pools for processing</td><td><code>Compute</code></td></tr><tr><td><strong>Execute workloads at scale</strong></td><td>Run queries and pipelines with dedicated runtime environments</td><td><code>Cluster</code></td></tr></tbody></table>

[^1]: Other resources not included in this table are:\
    \
    Secret, Operator

[^2]: Other stacks not included in this are: Beacon, Talos, Flash, Container\
    Lakesearch, dbt, steampipe,&#x20;
