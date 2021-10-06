---
title: Apache Flink - Stateful Computations over Data Streams
draft: false
---
<!--
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Apache Flink
{{< center >}} 
### A framework and distributed processing engine for stateful computations over *unbounded* and *bounded* data streams.
{{< /center >}}

![Apache Flink](/images/flink-home-graphic.png)

{{< column >}}

#### All streaming use cases

* Event-driven applications
* Stream & batch analytics
* Data pipelines & ETL 

[Learn more](https://flink.apache.org/usecases.html)

#### Operational focus

* Flexible deployment
* High-availability setup
* Savepoints

[Learn more](https://flink.apache.org/flink-operations.html)

<--->

#### Guaranteed correctness

* Exactly-once state consistency
* Event-time processing
* Sophisticated late data handling

[Learn more](https://flink.apache.org/flink-applications.html#building-blocks-for-streaming-applications)

#### Scales to any use case

* Scale-out architecture
* Support for very large state
* Incremental checkpointing

[Learn more](https://flink.apache.org/flink-architecture.html#run-applications-at-any-scale)

<--->

#### Layered APIs

* SQL on stream & batch data
* DataStream API & DataSet API
* ProcessFunction (time & state)

[Learn more](https://flink.apache.org/flink-applications.html#layered-apis)

#### Excellent performance

* Low latency
* High throughput
* In-memory computing

[Learn more](https://flink.apache.org/flink-architecture.html#leverage-in-memory-performance)

{{< /column >}}

### Upcoming Events

[![Flink Forward](/images/flink-forward.png)](https://flink-forward.org)

### Latest Blog Posts

{{ range ( first 3 ( where .Site.Pages "Type" "blog" ).ByDate ) }}
  <li><a href="{{ .Permalink }}">{{ .Title }}</a></li>
{{ end }}

{{ range ( where .Site.Pages "Type" "blog" | first 3 ) }}
  <li><a href="{{ .Permalink }}">{{ .Title }}</a></li>
{{end}}

{{ range where (where .Pages "Type" "blog" ) "Params.date" "=" 2021-08-06T00:00:00Z }}

{{ range first 5 (where .Site.Pages "type" "blog") }}

{{ range where .Site.Pages "Params.type" "blog" }}
   {{ .Title }}
{{ end }}

{{ range (where .Site.Pages "Params.type" "eq" blog) }}

{{ range .Site.Pages.type }}
  <p>Title: {{ .title }}</p>
{{ end }}

{{% notice info %}}
29.09.2021 - Apache Flink 1.14 has been released and we would love to hear your feedback. :)
{{% /notice %}}
