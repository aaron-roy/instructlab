RESEARCH **NOTE:**
IBM watsonx.data **brings**
Data Lakehouse to the Hybrid **Cloud**
Bridging the cloud and on-premises worlds

![0_image_0.png](0_image_0.png)

## Published May 2023 © Dbinsight Llc 2023® | Dbinsight.Io 1 Executive Summary

![1_Image_0.Png](1_Image_0.Png) Trigger

As part of IBM's new watsonx portfolio of offerings for AI and data builders, IBM is introducing its own data lakehouse. The new offering, branded watsonx.data, will be available as a fully managed SaaS service running on IBM Cloud or AWS infrastructure. It will also be available as a self-managed implementation on-premises or on any public cloud or deployed like a
"cartridge" add-on to existing Cloud Pak for Data clusters. With the announcement, IBM is the latest analytics platform provider to join the Apache lceberg lakehouse table format bandwagon. It also includes bidirectional support from IBM's existing hybrid-cloud data warehouses, including Db2 Warehouse and Netezza, and support of Spark and Presto query engines. It is intended to be the supporting data pillar of the watsonx, which also encompasses building, lifecycle management, and governance of foundation AI models. What does watsonx.data mean for IBM Db2 Warehouse and Netezza customers? And how will it compare to lakehouse offerings from the likes of Snowflake, Databricks, Starburst, Dremio, and hyperscalers, who have already disclosed their plans?

## Ourtake

As we noted in our data lakehouse market landscape research published earlier this year, we've been awaiting IBM's move. We are not surprised by IBM's choice of Apache Iceberg, as it is the lakehouse table format that has drawn the most multivendor support to date. IBM's offering is differentiated, not only by the support of IBM's data management tool portfolio
(that would be expected), but also its support of hybrid cloud deployment. IBM is the first to build a bridge to the lakehouse for on-premises data. Db2 and Netezza can be used both as query engines and analytic data sources. That will be supremely important to IBM's core enterprise base. Inclusion as part of the watsonx family will smooth the path for AI builders to access data that is likely more trustworthy than what would have come out of a conventional datalake.

While IBM is not the only lakehouse to support multiple query engines, what's notable is its support of Presto, which comes as the consequence of its recent Ahana acquisition. Given Presto's resemblance to the syntax and table structures of Netezza, IBM's support shouldn't be surprising. With Presto finally picking up contributor activity last year, we're pleasantly surprised that IBM plans to give Presto a fresh boost. Ultimately, we believe that IBM's hybrid and multicloud strategy will be a good fit for its customer base, few of whom are likely to move all of their workloads into the cloud. IBM views the lakehouse as the strategic future path for Db2 and Netezza customers, and on day one, offers support for accessing Db2 and Netezza data for lakehouse analytics and providing a simple pathway for migrating data to cloud storage; the migration path is work in progress.

Published May 2023 IBM is just beginning its deep dive into the lakehouse. IBM needs to demonstrate to Db2 and

![2_image_0.png](2_image_0.png)

Netezza customers that it will not compromise on the performance and service levels that they have had with their bespoke systems. We also need more definitive answer on how watsonx.data will leverage IBM's emerging Data Fabric, that provides a portfolio of data discovery, orchestration, and governance capabilities.

## Introducing New Choices To The Lakehouse

As the name implies, the data lakehouse is intended to bring the control and performance of the data warehouse to the data lake, while leveraging the economics of cloud storage. The lakehouse overlays a relational table structure on data stored in commonly used file formats that physically reside in cloud object storage. While there are proprietary lakehouse table formats out there, our research shows that the momentum is in open source where three projects (Delta Lake, Apache Iceberg, and Apache Hudi) are vying for vendor support. The elevator pitch for data lakehouse is about bringing ACID transactions to the data lake. This is not about making the lake into an OLTP database, but rather, to build confidence that the data in the data lake is trustworthy: it is current, consistent, and transactionally valid. And with that table structure comes other benefits such as superior performance compared to file scans; time travel; and more granular security and governance that can drill down to column and row level.

IBM has joined in, not just with a preliminary dip in the water, but a broad roadmap that addresses the diversity of its data and analytics portfolio and its existing hybrid and multicloud strategy. Let's address the highlights piece by piece.

Looking below the tip of Apache Iceberg IBM has placed its lakehouse table format bet with Apache Iceberg, which in turn has support for a variety of open source file formats, initially including Parquet, and ORC. From a market perspective, lceberg is the logical choice for IBM because it is the lakehouse table format that until recently drew the most multivendor support, such as Snowflake, Oracle, Cloudera, Google BigQuery, and AWS. There's a bit more nuance to all this with the two hyperscalers. While both AWS and Google Cloud plan to support Delta Lake and Hudi as well, Iceberg has been the first in line. By comparison, Databricks (which created and still controls Delta Lake) is a direct competitor to IBM because of its core focus on Apache Spark engine; in recent days, Delta Lake has picked up its first major support from third-party data platforms with Microsoft Fabric and SAP Datasphere. Given that Microsoft and Databricks have for over five years been tied at the Published May 2023 hips with the jointly delivered Azure Databricks analytics cloud service, we would have been

![3_image_0.png](3_image_0.png)

shocked if Microsoft wouldn't have chosen Delta Lake. As to Apache Hudi, it has drawn only scant commercial support. At this point, Teradata is the last major holdout on committing to open source lakehouse table formats. As we noted in our lakehouse market landscape research, while there is some functional differentiation across lakehouse formats, those differences are modest and given the pace of development, we expect broad functional equivalency within the next 18 months. Ecosystem, not technology, will determine which data lakehouse platforms prevail, because critical mass skillsets and commercial support will make the difference. As the market demands some competition, we expect that Apache Iceberg, along with Delta Lake, will be the two lakehouse formats left standing, putting IBM on the right side of history.

## What Is Watsonx.Data?

Figure 1 provides a conceptual view of watsonx.data. Apache Iceberg, as the lakehouse table format, will serve as the fulcrum of the offering. Parquet or ORC files sitting in Amazon S3compatible or IBM Cloud object storage is surfaced via several open source projects (Apache Hive for metadata, and Apache Ranger for access control). It can be queried by Presto, Apache Spark, Db2, or Netezza. The same goes for data sitting in Db2, Netezza and other data sources such as  Apache Kafka, MongoDB, MySQL, and PostgreSQL across hybrid-cloud deployments. As we noted above, including the lakehouse as an element of the watsonx family emphasizes the reality that when it comes to AI (both generative and traditional machine learning) it takes two to tango: models and data.

This is just the beginning. At IBM's Think conference, we saw demonstrations of capabilities for integrating data ingest and for semantic query based on one (or more) generative AI
foundation models. There are also the questions about data governance and data delivery.

The watsonx portfolio includes a separate SKU for AI model governance. By implication, data governance will be part of watsonx.data's remit. And in turn, to avoid becoming an island, we expect that there will be integration with IBM's Data Fabric, which is currently a work in progress.

## Hybrid And Multicloud Cloud Support

As data lakehouses have been premised on inexpensive cloud object storage and elastic compute, most existing offerings are deployed exclusively in the public cloud. With some exceptions (e.g., Google BigQuery Omni), hyperscaler lakehouse implementations only run in their own clouds, while others (e.g., Snowflake, Dremio, Starburst) can run in multiple public clouds. But the common thread is that until now, data lakehouses and public cloud have been joined at the hip.

Published May 2023

![4_image_1.png](4_image_1.png)

![4_image_0.png](4_image_0.png)

Given IBM's sizable landed enterprise customer base, few of them are expected to move all of their data or analytics workloads to the cloud anytime soon. Watsonx.data will run fully managed on IBM Cloud and AWS, with support for more clouds coming soon, like most of its non-hyperscaler rivals. The solution, like all Cloud Pak for Data offerings, will also run on Red Hat OpenShift for deployment in private cloud (which could physically be deployed in a public cloud or on premises). That provides the foothold into the on-premises data center.

A key differentiator for watsonx.data's lakehouse will be support for remote distributed caching, through future integration with IBM Spectrum Fusion, allowing organizations with data distributed across multiple physical instances to cache it where they want. By contrast, most other lakehouse implementations restrict caching to the local cluster adjacent to where the data is physically stored. The benefit of IBM's distributed remote caching is for use cases requiring low-latency performance. There are several scenarios that this enables. For instance, with support for access to Db2 and Netezzadata, this provides a way for the lakehouse to analyze data bridging on premises and the cloud. An alternative scenario would be for locally caching data from one or more public clouds for low-latency analytics; Db2 and Netezza already supported federated query for this purpose. The criteria for using this feature would involve balancing the benefits of reduced network overhead with costs for cloud data egress. Either way, remote distributed caching bolsters performance of the lakehouse on-premises and offers customers added flexibility on where they want to run their analytics workloads.

Published May 2023

## Query Engines

![5_Image_0.Png](5_Image_0.Png)

We've noted above how the respective vendor ecosystems around Apache Iceberg and Delta Lake are crystallizing. Here are a few comparisons as to how IBM's implementation with lceberg compares to some of the others.

Taking a closer look at the depth of Iceberg support, here is a comparison between IBM,
Snowflake, and Google BigQuery regarding metadata. For IBM, watsonx.data and WKC (Watson Knowledge Catalog) are the logical points where Iceberg metadata is treated as a first-class citizen, and how customers that might also be using Db2 or Netezza get a unified view of and access to the data. Snowflake and BigQuery are also treating Iceberg metadata natively, where Iceberg tables appear as "normal" rather than external tables on each platform. And those tables will be governable by the existing frameworks and tooling on each platform. For IBM, along with Snowflake and Google, Iceberg metadata support is clearly not lip service.

IBM promotes support of multiple open source query engines as a differentiator for its lakehouse, with Presto targeted for BI workloads while Spark is the preferred choice for data transformation and AI/ML. Most competing vendor lakehouse offerings also offer dual support, although not always with open source. While each of these engines may have their own control planes, IBM promises to offer a unified pane of glass bridging all workloads and query engines. This will be key to simplifying the experience of choreographing multiple query engines: it will be important to be able to spot and prioritize workload footprints as enterprises more closely scrutinize their cloud costs. Going forward, we would like to see "backwards compatibility" with IBM's data virtualization technologies to maximize watsonx.data's accessibility to the existing IBM customer base.

For IBM watsonx.data, the closest comparisons are with Dremio and Starburst, who both leverage open source with support for Spark by Dremio and Trino by Starburst and of course, already support Iceberg. By contrast, Databricks and Snowflake's support consists of a mix of open source and proprietary engines. Both rely on their own respective SQL query engines.

For transformation and AI workloads, Databricks (not surprisingly) uses Spark while Snowflake doesn't (at least, not directly). Instead, Snowflake relies on Snowpark which enables data scientists and engineers to package their own code as SQL-encapsulated user-defined functions or stored procedures. Snowflake also has a strategic partnership with Anaconda for optimizing its curated Python libraries to run in Snowpark. We believe that IBM could likewise benefit from a such a tie-in with Anaconda to make Python (the most popular data science language) a first-class query engine in its lakehouse. As to Google Cloud, a major differentiator for BigQuery Iceberg support is leveraging of serverless Spark.

## Governance And Metadata

![6_Image_0.Png](6_Image_0.Png)

The initial watsonx.data announcement was sparse on this area. The press release stated that watsonx.data would "provide built-in governance tools, automation and integrations with an organization's existing databases and tools to simplify set-up and user experience." The metastore will operate at two levels. At the bottom, it will use Apache Hive and Ranger for rudimentary metadata management, and WKC as the focal point where policies are applied and data lineage is exposed. All query engines supported by IBM's lakehouse will have access to the same shared metadata for data discovery and application of governance and security. When IBM implements WKC in watsonx.data, it will be first among equals with data catalogs.

In the long run, IBM's lakehouse will interoperate with third party catalogs (as a catalog of catalogs), as few organizations are likely to operate on a single data catalog. Consistent with IBM's AWS partnership, AWS Glue (which is primarily a technical metadata catalog utilized for managing data transformations) will interoperate with the metadata store of watsonx.data as a high priority future release on the roadmap. Another building block is IBM's emerging data fabric, which offers a series of modular and composable capabilities for developing and delivering data products that can be mixed and matched and delivered through Cloud Pak for Data. The fabric will be the underlying utility for data delivery (and associated tasks such as data pipeline orchestration) to the lakehouse.

As noted above, IBM data fabric support was not part of the initial announcement. It goes without saying that IBM's data governance and security portfolio spanning data protection, data observability, replication, virtualization, data matching, lineage, and other functions will ultimately have first-party support from the lakehouse. The initial announcement did not specify how these capabilities will be supported by watsonx.data, but we expect that blank will be filled by the time of general release. Given that IBM's lakehouse is being offered under the watsonx umbrella, targeted at AI and data builders, "traditional" (e.g., machine learning) and generative AI workloads are going to be frequent use cases. Watsonx does have an offering dedicated to model governance.

However, for organizations that seriously embrace building or customizing their own AI
models, model and data governance of necessity will have to get intertwined; attributes from explainability to model performance and bias detection will be driven by the assumptions of the model, choice of algorithm, and the data that is utilized. We would love to see a single pane of glass overlay that overviews both model and data governance, with slider-like controls for taking corrective actions when model and/or data drifts occur. By the way, IBM is not the only one that doesn't yet have the complete answer to the data and model governance question.

## Takeaways

![7_Image_0.Png](7_Image_0.Png)

As noted, we've been waiting for when IBM would take its deep dive into the data lakehouse.

IBM's strategy is broad-based. The clear delineators are IBM's hybrid and multi-cloud support, capabilities such as distributed caching, and native support for its broad portfolio of data and Al governance and lifecycle management tools. A potential key advantage for IBM watsonx.data lakehouse is its large third party partner ecosystem. IBM is not alone here, as Databricks and Snowflake also boast extensive partner networks. But the presence of a large partner ecosystem does not guarantee that all will be certified for lakehouse support on day one. For all comers, IBM included, the race is on for crtifications. The importance of private cloud support via Red Hat OpenShift for IBM customers cannot be overemphasized. With IBM's historical presence across large enterprises, providing a bridge to the on-premises world is critical. Even for enterprises intent on public cloud adoption, few are likely to move all of their data into the public cloud, and this is especially true for the heart of IBM's enterprise base. At this point, IBM's lakehouse is almost unique for its on-premises, private cloud support. Yes, we've qualified that statement because, through BigQuery Omni, where Google Cloud will support BigQuery running on Anthos (their equivalent of Red Hat OpenShift) anywhere, they could establish a beachhead in the data center with BigLake. But Google lacks the home court advantage of IBM, which has established presence with customers already using much of its data management portfolio.

With watsonx.data, IBM is not sunsetting Db2 or Netezza; in fact, both of them are complimentary to watsonx.data to support cost and performance optimizations across multiple query engines. Both will have "augment" options that will carry their own optimizations for lakehouse workload support. With a multi-engine approach, Db2 and Netezza customers can pair the right workload with the right engine. IBM' challenge will be to make augment options simple. As we have stated, the data lakehouse will not necessarily replace data warehouses, because not every business question will require using a data lake.

Watsonx.data will be complementary to those engines by providing to first-class, ACID- compliant access to cloud storage and access to some of the best query engines that the open source world has to offer. Those query engines would be in addition to, rather than instead of the native query engines of Db2 and Netezza.

For Db2 and Netezza customers, the transition to Presto should be fairly straightforward given the similarity of syntax and table structures. In some cases, Presto has leapfrogged its legacy counterpart, such as with its more advanced time travel capabilities. At launch, IBM is supporting the ability for the lakehouse to access data from Db2 and Netezza and for Db2 and Netezza users to move their data into cloud storage. IBM needs to double down to automate Published May 2023 the migration path; given the parallels between the query engines and Presto, we would also

![8_image_0.png](8_image_0.png)

like to see IBM add a virtualized Netezza native shell atop Presto as an option to make Netezza customers feel at home.

We've noted above that full support from Watson Query and IBM's data governance portfolio are key to filling out watsonx.data. At the macro level, there is the need to formally integrate IBM's emerging data fabric and rationalize Cloud Pak for Data with watsonx.data. Right now, they appear to be two different product portfolios and technology stacks. They should be the same SKU, with the option to "expand" or "augment" with Iceberg lakehouse tables.

We would also like to see upgraded support of Python. Today, customers working with Cloud Pak for Data can use Jupyter notebooks to write Python and run it on Spark. Within the Python community, there are those who prefer native support of Python libraries as an alternative to using the PySpark API (which connects to Spark Resilient Distributed Datasets, or RDDs). A partnership with Anaconda for its curated, supported Python libraries, would be icing on the cake.

## Author

Tony Baer, Principal, dbInsight tony@dbinsight.io LinkedIn https://www.linkedin.com/in/onstrategies/

## About Dbinsight

dbInsight LLC® provides an independent view on the database and analytics technology ecosystem. dbInsight publishes independent research, and from our research, distills insights to help data and analytics technology providers understand their competitive positioning and sharpen their message.

Tony Baer, the founder and principal of dbInsight, is a recognized industry expert on datadriven transformation. Onalytica named him as a Top Cloud Influencer for 2022 for the fourth straight year. AnalyticsInsight named him one of the 2019 Top 100 ArtificialIntelligence and Big Data Influencers. His combined expertise in both legacy database technologies and emerging cloud and analytics technologies shapes how technology providers go to market in an industry undergoing significant transformation.

dbInsight® is a registered trademark of dbInsight LLC.

Published May 2023