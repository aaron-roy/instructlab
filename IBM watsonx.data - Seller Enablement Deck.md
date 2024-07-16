IBM watsonx.data Seller presentation
—Kevin Shen Product Manager | Data and AI SoftwareYuankai.Shen@ibm.com

Joshua Kim Program Director | Data and AI SoftwareJoshkim@ca.ibm.com

Shawn Brennan
WW Sales Leader | watsonx.data | Data and AI Software
sbrennan@us.ibm.com 

Anson Kokkat
Senior Product Manager | Software
ansonk@ibm.com

Adam LearmonthAdvisory, Learning Content DevelopmentAdam.Learmonth@ca.ibm.com
Seller guidance and legal disclaimer

References in this presentation to IBM products, programs, or services do not imply that they will be available in all countries in which IBM operates. Product release dates and/or capabilities referenced in this presentation may change at any time at IBM’s sole discretion based on market opportunities or other factors and are not intended to be a commitment to future product or feature availability in any way. Nothing contained in these materials is intended to, nor shall have the effect of, stating or implying that any activities undertaken by you will result in any specific sales, revenue growth, or other results. 

All client examples described are presented as illustrations of how those clients have used IBM products and the results they may have achieved. Actual environmental costs and performance characteristics may vary by client.

Slides in this presentation marked as "IBM and Business Partner Internal Use Only" are for IBM and Business Partner use and should not be shared with clients or anyone else outside of IBM or the Business Partners’ company.

© IBM Corporation 2023. All Rights Reserved.

The information contained in this publication is provided for informational purposes only. While efforts were made to verify the completeness and accuracy of the information contained in this publication, it is provided AS IS without warranty of any kind, express or implied. In addition, this information is based on IBM’s current product plans and strategy, which are subject to change by IBM without notice. IBM shall not be responsible for any damages arising out of the use of, or otherwise related to, this publication or any other materials. Nothing contained in this publication is intended to, nor shall have the effect of, creating any warranties or representations from IBM or its suppliers or licensors, or altering the terms and conditions of the applicable license agreement governing the use of IBM software.


IBM and Business Partner Internal Use Only
Agenda

AI market trends
Data Management market trends
Data Management market growth and dynamics 
Watsonx.data product overview 
Feature highlights
Key components
Integrations 
Packaging and pricing
Competitors and differentiators
Use cases 
Call to action and timeline 

AI market trends
The Generative AI sales play spotlight (required for all sellers): on Seismic
Data Management market trends 

Like-for-like compatibility for databases, apps and ETL in hybrid deployments
Zero downtime database migration tooling & automation
Fully-managed services and consumption-based pricing for lowest TCO
Combine structured and unstructured data, no matter where it resides for AI workloads and applications
Multiple analytics engines to support new use cases across AI, real-time analytics, data engineering, and data sharing
Single source of truth with zero-copy semantic layer (no ETL needed)
Centralized or federated metadata management querying datawhere it lives
Governed, secure data access control point across all repositories and query engines to truly democratizedata access
Strategic 
objective
Pervasive needs
How IBM helps
1
Infrastructure modernization

Improve resiliency of existing apps
Reduce direct and indirect data management costs
Scale workloads faster to meet customer demand
2
AI and digital transformation

Scale AI across a broader range of data
Make decisions using real-time data
Derive new insights from broader range of data

3
Security and compliance

Avoid the risk of embarrassing and costly data breach
Strictly enforce data locality rulesand boundaries 
Market drivers for changes in data management strategy
Hybrid-cloud data ecosystem
8
Public cloud SaaS is overtaking on-premises.
Transactional/operational systems represent the largest segment of the databases market, with $41B, 12% CAGR (‘21-’25).
The warehouse & data lake market is $23B, 17% CAGR (‘21-’25) and almost all the growth is coming from public cloud SaaS and the data lake segment.
Enterprises look to open source to: 
reduce license costs, 
leverage community innovation and support, and
avoid vendor lock-in. Open source provides fit-for purpose technologies for diverse data types.

Data management market drivers
There’s more data

Exploding data growth
The aggregate volume of data stored is set to grow over 250% in the next 5 years.
In more locations

Multiple locations, clouds, applications and silos
82% of enterprises are inhibited by data silos.
In more formats 
Documents, images, video
80% of time is spent on data cleaning, integration and preparation.

With less quality 
Stale and inconsistent
82% of enterprises say data quality is a barrier on their data integration projects.


And when it comes to scaling AI, leaders are faced with unprecedented data challenges 
Source: https://www.idc.com/getdoc.jsp?containerId=US49018922)

This environment leads to more cost and complexity for those who seek to use governed data for AI.


Data management market evolution 
Traditional approaches: Data Warehouse vs Data Lake
Learn more about the data lakehouse kitchen analogy in this 101 video
101: Data Lake
How can we discover what we don't know?
As volume, velocity and variety of data grew, data lakes were designed for data discovery and data science/machine learning use cases.
Commonly built on large data platforms such as Hadoop (HDFS)
Data is stored in RAW and unstructured format = lower cost for large volumes of data
Highly flexible and scalable
Difficult to use and govern, and complex to maintain, required data scientist, now many are data swamps
Unstructured data
Low-cost storage
AI/ML
101: Data Warehouse
How can we ask enterprisewide questions requiring historical data?
A data warehouse gathers structured data from multiple sources into a central repository 
Supports multiple data analytics and business intelligence applications such as enterprise reporting, to answer questions about your business
Normalized and structured data made it easy to analyze, but was an expensive choice
 
High performance
BI
Governed
Costly
Additional links:
Databases 101
What is a data warehouse 
What is a data lake 
The data warehouse remains the center of analytics at most organizations

Data warehouses emerged as the dominant method to analyze data
Normalized and trusted data made it easy to analyze, however it’san expensive choice
Warehouses technology has evolved continuously to improve… from appliance form factors to in-memory technologies

High up-front costs
Structured data only
ETL required
Vendor lock-in
Limited scalability
Data warehouse

Late 1990s
Early 2000s
Present

As volume, velocity, and variety of data grew, data lakes emerged as the new technology to replace data warehouses
Data stored in raw and unstructured format = lower cost for large volumes of data
Highly flexible & scalable
Difficult to use & complex to maintain, and required a data scientist
Ultimately, most data lakes failed and required a two-tier architecture
High up-front costs
Structured data only
ETL required
Vendor lock-in
Limited scalability
Data warehouse
Data lake
High complexity
Poor data quality
Limited performance
Expensive to maintain


Late 1990s
Early 2000s
Present
The emergence of the data lake


Specifically, cloud data warehouses introduced the separation of compute and storage
Addressed the scalability challenge with traditional warehouses – no data redistribution
Ability to add more compute resourcesto the same data to solve the problem
Easier to manage, however, much more expensive vs. on-premises warehouses
High up-front costs
Structured data only
ETL required
Vendor lock-in
Limited scalability
Data warehouse
Data migration
Vendor lock-in
High costs
Limited AI/MLuse cases
Data lake
Cloud data warehouse
High complexity
Poor data quality
Limited performance
Expensive to maintain



Cloud data warehouses evolved to address specific challenges of data warehouses 
Late 1990s
Early 2000s
Present
15
Traditional approaches to addressing these challenges have created more overall complexity and cost, which has led to the emergence of data lakehouse architectures


Today, leaders at most large enterprises manage their data and workloads using a mix of data repositories and data stores in hybrid environments. 
The overall cost across all these repositories remains high.
It’s difficult for leaders to effectively leverage and govern the data across multiple environments and use enterprise data for analytics and AI.

Early 2000s
Analytics Repositories Market Landscape


Technology
Deployment
On-premises
$12bn 2025
2% CAGR (’21-’25)
SaaS
$31bn 2025
27% CAGR (’21-’25)
Proprietary
$26bn 2025
13% CAGR (‘21-’25)
Open
$17bn 2025
27% CAGR (’21-’25)
Disruptions are driving the growth in the analytics repositories market from on-premises to SaaS and from proprietary to open technologies 
Grow
Modernize
Acquire
Surround
IIAS Appliance
Db2 BigSQL
Market dynamics
Lakehouse overview and first-generation lakehouses 
The data lakehouse
Data lakehouse (n):
A data lakehouse combines the high-performance characteristics of a data warehouse with the cost-efficiency, flexibility and scalability of a data lake to support highly complex data transformations and a wide variety of use cases

Lakehouses are meant to be a new class of data store thatcombines the best of data warehouses and data lakes
First generation lakehouses are still limited by their ability to address cost and complexity challenges:

Single query engines set up to support limited workloads … typically just BI or ML

Typically deployed on cloud only with no support for multi-/hybrid-cloud deployments

Minimal governance and metadata capabilities to deploy across the entire ecosystem
Enterprise leaders require a data architecture that can provide quick access to data, centralized governance and fit-for-purpose use
1
Ability to scale AI while supporting compliance with lineage and reproducibility of data  

2
Real-time analytics and BI that can connect to existing data in minutes without expensive duplicating or moving of data 
3
Data sharing and self-service access for more users and more data while strengthening governance and security




What is IBM watsonx.data?
watsonxScale and accelerate the impact of AI with trusted data.
A next generation enterprise studio for AI builders to train, validate, tune, and deploy both traditional machine learning and new generative AI capabilities powered by foundation models. It enables you to build AI applications in a fraction of the time with a fraction of the data.

Fit-for-purpose data store, built on an open lakehouse architecture, supported by querying, governance and open data formats to access and share data.
End-to-end toolkit for AI governance across the entire model lifecycle to accelerate responsible, transparent, and explainable AI workflows


watsonx.ai
Train, validate, tune and 
deploy AI models
watsonx.data
Scale AI workloads, for all 
your data, anywhere
watsonx.governance
Accelerate responsible, transparent and explainable AI workflows
The platformfor AI and data
23
Leverage governed enterprise data in watsonx.data to seamlessly train or fine-tune foundation models
Leverage foundation models to automate data search, discovery, and linking in watsonx.data 
Enable fine-tuned models to be managed through market-leading governance and lifecycle management capabilities
Scale AI workloads, for all your data, anywhere
Train, validate, tune, and deploy AI models
Accelerate responsible, transparent. and explainable AI workflows
watsonx.ai
watsonx.data
watsonx.governance
Put AI to work with watsonx
Scale and accelerate the impact of AI with trusted data





Scale AI workloads,for all your data, anywhereA fit-for-purpose data store, based on an open lakehouse architecture, supported by querying, governance and open data formats to access and share data

Get started in minutes with built-in governance, security and automation.
Access all your data through a single point of entry across all clouds and on-premises environments.
Reduce the cost of your data warehouse by up to 50%* through workload optimization across multiple query engines and storage tiers. 
*When comparing published 2023 list prices normalized for VPC hours of IBM watsonx.data to several major cloud data warehouse vendors. Savings may vary depending on configurations, workloads and vendors. 
watsonx.data



Cloud warehouse

Cloud data lake


On-prem warehouses
Optimize cloud warehouse workloads
Make the most of fit-for-purpose query  engines and compute resources  


Optimize and access on-prem warehouse workloads
Use low-cost object storage and fit-for-purpose engines


Modernize data lakes Run existing reporting and enable new AI workloads without the cost and complexity of Hadoop


Deploy across hybrid cloud and multicloudSeamlessly deploy to both the public cloud and to your existing on-premises investment
Access all your data quickly and optimize your data architecture with multi-engine support and hybrid deployment of analytics and AI workloads 
Link to full IBM watsonx.data client deck on Seismic
watsonx.data key components 
IBM watsonx.data is the next evolution of current first-generation lakehouses

First-generation lakehouse

Next generation lakehouse – IBM watsonx.data
IBM watsonx.data is the only lakehouse with multiple open-source query engines allowing clients to optimize costs and performance  by pairing the right workload with the right engine
Run all workloads from a single point of entry
Deploy anywhere with full support for hybrid cloud and multicloud environments
Shared metadata across multiple engines eliminates the need to re-catalog, accelerating time to value while ensuring governance and eliminating costly implementation efforts


Governance and Metadata

Overview of the key components of IBM watsonx.data: multiple query engines, open table formats, and built-in enterprise governance
Multiple engines such as Presto and Spark that provide fast, reliable, and efficient processing of big data at scale
Cost-effective, simple, object storage available across hybrid cloud and multicloud environments
Hybrid cloud deployments and workload portability across hyperscalers and on-premises with Red Hat OpenShift
watsonx.data
Storage
Infrastructure
Your existing ecosystem
Optimize workload costs and performance using multi-engine functionality 
Reduce storage costs and facilitate data ingest 
Deploy on any infrastructure and optimize available resources
Data warehouse
Data lake
Query engines


Strengthen governance and reduce time to insight with centralized metadata and access management
Built-in governance that is compatible with existing solutions such as IBM Knowledge Catalog
Governance and metadata

Access all of your data across databases and data lakes
Vendor agnostic open formats for analytic data sets, allowing different engines to access and share the same data, at the same time
Data format

Access control management
Metadata store
Access 100% of your data across databases and data lakes
Optional 
Deploy seamlessly across any cloud or on-premises environments in minutes

Combine on-prem and cloud data to create a unified view of data that is easier to manage, govern, and analyze
Keep sensitive data on-premises while leveraging the scalability and cost-efficiency of the cloud
1
Deploy across any cloud or on-prem environment
2
Data load ready in minutes
No open-source complexity
Full service – storage, engine, and metadata store all integrated and preconfigured
Deploy seamlessly and fully managed in minutes

Cloud

On-prem
watsonx.data 
Storage
Infrastructure
Your existing ecosystem
Data warehouse
Data lake
Query engines


Governance and metadata

Data format

Access control management
Metadata store
Store large volumes of data in low-cost object storage and share it through an open table format built for high performance analytics


Apache Iceberg is a high-performance table format that excels at large-scale data processing and analytics
Time travel and rollback features enable reproducible queries to examine changes over time and rollback quickly to a previous state
Utilize simple object storage to store vast amounts of data at fractions of the cost of traditional block storage
Cost effective – Object storage is a fraction of the cost of traditional block storage and available from multiple providers

watsonx.data 
Storage
Infrastructure
Query engines


Governance and metadata

Data format

Access control management
Metadata store

Ensure enterprise compliance and security using built-in unified governance or connect to existing solutions
Leverage a single unified/shared metadata service across all lakehouse and warehouse engines that simplifies access with holistic access management policies
Directly integrate with IBM Knowledge Catalog and enforce Knowledge Catalog policies in the lakehouse via metadata service
1
Connect to existing governance solutions
2
Utilize built-in open-source technology to manage governance and security, including metadata, lineage, access, and cataloging
Utilize built-in metadata & access control solutions




watsonx.data 
Storage
Infrastructure
Query engines


Governance and metadata

Data format

Access control management
Metadata store
Optimize costly warehouse workloads using fit-for-purpose engines that scale up/down automatically with a client's needs

watsonx.data 
Storage
Infrastructure
Query engines


Governance and metadata

Data format

Access control management
Metadata store
Integrations and IBM ecosystem for watsonx.data 
The integrated IBM watsonx.data ecosystem for maximum workload coverage and optimal price-performance 


IBM watsonx.data functionality
Integrations at GA
2
4
Watsonx.data Metadata Store
IBM Knowledge Catalog

Db2W
Netezza
Spark
Presto
1
3
Object storage
Object storage
5
Db2 z/OS
6


Investments in a trusted data foundation will accelerate and scale AI
Effortlessly populate with trusted data leveraging best-in-class data ingestion and observability 
watsonx.data + IBM DataStage 
Easily build EL(T) pipelines with an intuitive visual design
Ingest data from any sourceLeverage 60+ native connectors to ingest data into watsonx.data from any type of source, ensuring top performance with built-in engine scalability
Reduce cost by offloading data from cloud data warehousesOffload data from cloud data warehouses to enable shifting workloads like BI, reporting, or data science to fit-for-purpose query engines

watsonx.data + IBM Databand
Continuously detect and resolve data quality incidents
Monitor, detect, and resolve data quality incidentsMonitor and improve the health of DataStage, Spark, or Python pipeline workloads running on watsonx.data; detect data anomalies and accelerate issue resolution 

1
2
3
watsonx.data
IBM databases and watsonx.data cross-sell narrative 
watsonx.data + databases cross-sell overview 
When do I sell what and who do I sell to?
IBM and Business Partner – Internal Use Only
Packaging and pricing 
Link to watsonx Packaging and Pricing (owner: Jason Foss)
IBM and Business Partner – Internal Use Only

SaaS subscription based on tiers below + consumption:EssentialsIndividual users, self-served POCs, and experimentsStandardEnterprise-grade production usePremium*Enterprise-wide adoption*available soon
watsonx.data
↓
SaaS and software offerings available

Free trial available

SaaS pricing based on consumption of quantity and duration of deployed nodes and supporting services

Software pricing based on nodes

watsonx.ai
↓
SaaS offering available


Free trial available

SaaS pricing for inference, tuning, and hosting







watsonx.governance
↓
Will offer both SaaS and software options




Pricing and packaging options available for watsonx 
IBM and Business Partner – Internal Use Only
Competitors and objection handling 
IBM watsonx.datacompetitive insights

Get the presentation on Seismic  →


Learn more about the competition

Provide feedback

Request help with an opportunity

IBM and Business Partner – Internal Use Only
Types of competitors
Data lakehouse competitors
Designed for both structured and unstructured data

Based on open    table and data formats for data storage

Fit for purpose query engine for different use cases

Cost optimization for compute engine and storage

Separate compute and storage
Augmented data warehouse competitors
Primarily designed for structured and semi- structured data

Uses proprietary or open file formats, but supports open table format for data storage

Query processing uses data warehouse engine

Compute and storage are not completely separated
A data lakehouse combines the best features of data warehouses and data lakes to provide cost optimization for clients. Compute and storage are separated so that data can be accessed from different engines.

An augmented data warehouse may be able to access different types of data, but all compute processing is performed through the data warehouse engine. There is no compute cost optimization allowing different engines, only the compute amount used by the data warehouse engine can be adjusted.
IBM and Business Partner – Internal Use Only
watsonx.dataCompetitoroverview(weaknesses not mentioned)
All competitors are relatively new companies (within the past decade) and are rapidly growing in the public cloud market
Data Lakehouse Competitors


Others
IBM and Business Partner – Internal Use Only
Breaking news from competitors
Find the watsonx.data Competitive and Objection Handling presentation on Seismic→
For the latest breaking news on Databricks, Snowflake, Microsoft, and others, 
please refer to Latest updates slides within the “Competitors at a glance” section of  the                                       watsonx.data Competitive and Objection Handling presentation
IBM and Business Partner – Internal Use Only
Competitive landscape
Other competitors 
IBM and Business Partner – Internal Use Only
Data lakehouse competitors 

watsonx.dataPrimary competitors at a glance Hybrid cloud
IBM and Business Partner – Internal Use Only
watsonx.dataPrimary competitors at a glance Multiple query engines
IBM and Business Partner – Internal Use Only

watsonx.dataPrimary competitors at a glance Open-source based
IBM and Business Partner – Internal Use Only
watsonx.dataPrimary competitors at a glance Data governance
IBM and Business Partner – Internal Use Only
watsonx.dataPrimary competitors at a glance Market presence
IBM and Business Partner – Internal Use Only
(GA July 2023)
watsonx.data Differentiators
Other data lakehouse competitors do NOT have the level of experience with mission critical applications, and level of research in query optimization and query processing, as IBM

Watsonx.data plus other IBM data sources (Netezza Performance Server and Db2) deliver a query performance spectrum not offered by other data lakehouse competitors

Watsonx.data and its selection of Apache Iceberg and Presto delivers an open solution versus a single contributor open-source lock-in
No other data lakehouse offering has integrated data warehouse engines in addition to the Apache Spark and open-source query engines

The cloud hyperscalers (AWS, Microsoft Azure, and GCP) along with Databricks provide no hybrid cloud deployment capability

Deployment flexibility in other clouds – no other data lakehouse offering can be deployed as easily across different cloud platforms
IBM and Business Partner – Internal Use Only
74%
LESS EXPENSIVE  vs. SNOWFLAKE
A large retailer found watsonx.data in their test to be…
Concepts and market entry points
Three key concepts for IBM watsonx.data
Presto is a next-generation open-source SQL engine designed to run efficiently over data lakes.

Warehouses and first-generation lakehouses are monolithic, and not optimized to work on all workloads. Only IBM watsonx.data’s multi-engine architecture allows for true workload optimization.

Iceberg is an open-table format that allows multiple engines to access the same data – this means, Snowflake, Netezza, and IBM watsonx.data can all access data in Iceberg at the same time.
IBM and Business Partner – Internal Use Only
Market entry points + use cases
1. Warehouse Optimization narrative 
Competitive and IBM (Netezza + Db2)
Talk track – Client is concerned with the spend on traditional warehouse today – looking to optimize for both performance and cost 
Value prop: Cost optimization and openness through the shared meta layer and fit-for-purpose engines
Use case – Snowflake write-intensive workloads moving to Spark and/or Presto, thus reducing cost of Snowflake virtual data warehouses 
2. Modernizing data lake narrative
Modernizing storage architecture to facilitate shared metadata and fit-for-purpose engines
Talk track – Converting legacy file storage structures into open-file structures and assigning those into the shared meta layer, thus facilitating fit-for-purpose engines
Value prop: Modernize with warehouse-like performance for querying data in open formats, built-in governance 
Use case – Move from HDFS to open-source iceberg within a consolidated shared meta layer 

IBM and Business Partner – Internal Use Only
Call to action and timeline 
Call to action

2
Begin conversations with clients
Announce was at Think 2023, GA on July 7th, 2023
Cost reduction is top of most clients’ minds
Four questions sellers should ask
“Are there concerns with the cost of your Cloud Data Warehouse?”
“Are you running all workloads on your warehouse today? For example,  ETL, Ingest, BI, Dashboards?”
“Do you have a Hadoop data lake? Have you considered modernizing?”
“Are you getting value out of your data lake today, or is it mostly being used for data storage (a data swamp)?”



1
Prepare yourself!
Visit watsonx.data sales kit on Seismic for additional enablement and sales materials
Additional watsonx.data specific enablement sessions will be scheduled
Do not hesitate to reach out to PM team with any questions or additional enablement needs
IBM and Business Partner – Internal Use Only
Client briefing 
Discussion and custom demonstration of IBM’s generative AI watsonx point-of-view and capabilities. Understand how watsonx.data can be leveraged in client’s AI strategy.
Pilot program
Watsonx pilot developed with IBM AI engineers. Prove watsonx.data value for the selected use case(s) with a plan for adoption.


Three ways clients can get started with watsonx.data today IBM’s investment in partnering with clients
Free trial
Experience watsonx.data and test out core capabilities with a free trial.


Link to free trial
2-4 hours
1-4 weeks
Technology Expert Labs watsonx.data companion services


Services offering to implement one supported use case with watsonx.data. Suitable for on-premises or SaaS. 

Integrate withclient infrastructure
Implementation & validation
User Acceptance testing and go live support


Outcome: Successful optimization of client workload with watsonx.data

Install
(Non-SaaS Only)
2 Weeks
Services offering to deploy and configure a watsonx.data environment and integrate with the client IT environment.

Install and configure OpenShift  (non-SaaS only).
Install and configure watsonx.data service



Outcome: Scalable watsonx.data environment ready for client workload
Install Offering
(Non-SaaS only)
Build Offering
3 Weeks


Subscription-based service that provides access to deep technical expertise in design, deployment, operations,and transformation whilebuilding a client’scapacity and skills.


Expertise Connect is the insurance policy that helps clients succeed with IBM technologies and allowsthem to move forward in their IBM journey. 
Expertise Connect
1 Year


Tailored services to help a client augment their existing data management systems with watsonx.data.

Planning 
Solution design
Installation
Workload optimization
User acceptance testing
Go-live support
Enablement

Engage Solution Engineering →
Custom Services
IBM and Business Partner – Internal Use Only
Client path to watsonx.data adoption through Technology Expert Labs

1
Attach pre-scoped offerings to all new license sales
2
Expand withExpertise Connect
3
Engage Expert Labs Services Sellers early in the software sale
Expert Labs Contacts

Jennifer Wales
Services Product Manager, Data and AI

Ted Trask
Program Director, WW Data & AI Services Sales Leader

Pradeep Kutty
Business Unit Executive - Solution Engineering

Suzanne Golledge 
WW Principal Delivery Practice Leader

Seller Locator Tool

Slack: #ask-expert-labs
*New watsonx part numbers will be available in late July 2023, see offering pages for latest part numbers
IBM and Business Partner – Internal Use Only
IBM watsonx.data – High-level milestones & timeline	
*Subject to change 
IBM and Business Partner – Internal Use Only