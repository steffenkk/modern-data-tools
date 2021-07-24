# List of Modern Data Tools
## What is "the modern data stack", actually?
Thats a tough one!  You can't really say that there is such a thing as the one and only modern data stack.However, there are certain ideas/tools/do's and dont's/etc. that can be combined to form one thing that is modern and is a data stack. These tools tend to be easy-to-use, open, cloud-native or even SaaS. Go Data Driven has a [blog article](https://godatadriven.com/blog/modern-data-stack-the-road-to-democratizing-data/) that describes this pretty well. Are you asking yourself now, "So that's it, I'll just switch all my tools to the ones listed here and then I've got it?" - Far from it! As always, it's all about the people ...

## WORK IN PROGRESS:
Next things to add
- more tools
- maybe best practices / reference architecutres?

## DISCLAIMER
The author is in no way affiliated with the companies listed here and receives no compensation. The listing serves as an example and does not claim to be complete.

## Contents

- [Data Platforms](#data-platforms)
- [Data Integration](#data-integration)
- [Data Transformation](#data-tranformation)
- [Data Analytics](#data-analytics)
- [Data Visualization](#data-visualization)
- [Data Quality](#data-quality)
- [Data Explorability](#data-explorability)
- [Machine Learning](#machine-learning)
- [Languages](#languages)

## data-platforms
Answer the question: where to put the data?


- [Amazon S3](https://aws.amazon.com/s3/): Typical cloud-based object storage that integrates with a multitude of different data lake tools. Offered by AWS.
- [Google Cloud Storage](https://cloud.google.com/storage): Typical cloud-based object storage that integrates with a multitude of different data lake tools. Offered by Google.
- [Azure Data Lake Gen2](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction): Typical cloud-based object storage that integrates with a multitude of different data lake tools. Offered by Microsoft.
- [Delta Lake](https://delta.io/): An open-source file engine build ontop of apache parquet that brings high performance, acid transactions, updates & deletes, and muche more to your data lake. Compatible with Spark, Databricks, etc. 

## data-integration
Answer the question: how to get the data from the system into our platfrom?


- [Meltano](https://meltano.com/): open-source data integration using the singer specification.
- [Airbyte](https://airbyte.io/): open-source data integration with a rich UI, an API and CLI.
- [Fivetran](https://fivetran.com/): fully managed SaaS data integration tool with several prebuild connectors.
- [Stitch Data](https://www.stitchdata.com/): fully managed SaaS data integration tool with several prebuild connectors and an SDK (Singer) to easily add more integrations.
- [Azure Data Factory](https://docs.microsoft.com/en-us/azure/data-factory/quickstart-create-data-factory-portal): cloud based data intagration, transformation and orchestration in Azure.
- [Kafka Connect](https://docs.confluent.io/platform/current/connect/index.html#:~:text=Kafka%20Connect%20is%20a%20free,Kafka%20Connect%20for%20Confluent%20Platform.): When working with Kafka use kafka connect to integrate your data natively into your data platform.

## data-tranformation
Answer the question: how can we make this data consumable?


- [DBT](https://www.getdbt.com/): SQL first data transformations in your datawarehouse. The "T" in ELT. Extends SQL with jinja templates for more powerful operations. Open-source or SaaS (offered by DBT Labs).
- [AWS Glue](https://aws.amazon.com/glue/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc): Serverless Apache Spark for big data transformations. Enriched by AWS Glue tools and integrations.
- [Databricks](https://databricks.com/): Managed Apache Spark for big data transformations in Python, Scala, Java, SQL, or R. Enriched by Databricks Utils, integrations, and a whole ecosystem of different tools (e.g. Delta Lake). 


## data-orchestration
Answer the question: which data comes in from where and when?

- [Dagster](https://dagster.io/): open-source data orchestration tool to build DAGs and run them. Provides an UI, CLI and an API. 
- [Prefekt](https://www.prefect.io/): data orchestration SaaS tool with API, UI and CLI.
- [Airflow](https://airflow.apache.org/): open-source platform to orchestrate and monitor workflows with several integrations and a powerful UI.
- [Google Cloud Composer](https://cloud.google.com/composer): Cloud based version of Airflow in GCP.
- [AWS Stepfunctions](https://aws.amazon.com/step-functions/): Serverless orchestration tool for AWS Services.

## data-analytics
Answer the question: how can we access tha data?

- [Snowflake](https://www.snowflake.com/): data warehouse of the cloud era. Sits on top of your data platform and offers you a fully fledged data warehouse. 
- [Google BigQuery](https://cloud.google.com/bigquery): Cloud DWH from google. Serverless and dynamically scalable to adjust to any workload. 
- [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/): Cloud DWH from Azure (SQL Pools). Use serverless (on top of the data datalake) or with provisioned instances in the Azure Cloud.
- [AWS Redshift](https://aws.amazon.com/redshift/): Cloud DWH from Amazon. Analyze your data in a relational SQL DWH which looks and feels like postgres, or directly in the datalake with Redshift Spectrum. 
- [Dremio](https://www.dremio.com/): SQL Lake House Solution: Build your DWH on top of your data lake to reduce data movement. 
- [Databricks SQL Analytics](https://databricks.com/product/databricks-sql): SQL Lake House from Databricks with the power of the delta engine which allows you to use your Data Lake just like a DWH. 
- [Trino (formerly PrestoSQL)](https://trino.io/): Open-source SQL-Based federated query engine to query files in your data lake as well as distributed databases.


## data-visualization
Answer the question: what does the data tell us?

- [Tableau](https://www.tableau.com/): Dashboards and BI from Tableau (Sales Force). Self hosted or SaaS.
- [Looker](https://looker.com/): Google-cloud based SaaS BI Platform. Supports AWS Deployment as well. 
- [PowerBI](https://powerbi.microsoft.com/en-us/): Dashboards and BI from Microsoft. Self hosted or SaaS in Azure.
- [ThoughtSpot](https://www.thoughtspot.com/): SaaS, search-driven BI Platform to allow users create visualizations with natural language questions.


## data-quality
Answer the question: can we trust that data?

- [Datafold](https://www.datafold.com/): Data observability platform, SaaS based. With features such as Data Diff to regression test your ETL Code. 
- [Monte Carlo Data](https://www.montecarlodata.com/): SaaS based data observability platform to detect data-downtime and ensure data reliability. 
- [Great Expectations](https://greatexpectations.io/): A python package to help you test and validate your data in the ETL process.  

## data-explorability
Answer the question: what data do we actually have?

- [Atlan](https://atlan.com/platform/data-catalog/): A modern data catalog for the modern data stack. Integrate and expose all your data assets in a curated and centralized repository. 
- [Tableau Data Management Add-On](https://www.tableau.com/products/add-ons/data-management): Data Catalog and lineage for tableau online or server deployment.
- [DBT Docs](https://docs.getdbt.com/reference/artifacts/catalog-json): Catalog from open-source data transformation tool dbt. Auto-genereated from your DBT Transformations and extensible in a YAML template.
- [Amundsen](https://www.amundsen.io/): open-source data catalog developed by lyft and used by multiple other companies.  Integrations to common data stores like redshift, snowflake, bigquery, etc.  

## machine-learning
Answer the question: what can the data tell us about the future?


- [Amazon Sagemaker](https://aws.amazon.com/sagemaker/): Build, train, deploy, and monitor machine learning models with this platform in AWS.
- [Databricks Managed ML Flow](https://databricks.com/product/managed-mlflow): An open source machine learning platform based on top of Apache Spark.
- [Azure Machine Learning](https://azure.microsoft.com/en-us/services/machine-learning/#features): Managed ML Ops platform in Azure.


## languages
Answer the question: how to do all this?


- [SQL](https://en.wikipedia.org/wiki/SQL): Database Query Language, the must-have for all data peoples.
- [Python](https://www.python.org/): the *best* programming language on earth (author's opinion 😜).
- [Terraform](https://www.terraform.io/): Infrastructure as code (IaC) for multiple cloud providers. Uses own language (HCL).
- [Pulumi](https://www.pulumi.com/): IaC for multiple cloud providers. Uses mainstram languages like JavaScript and Python.
- [AWS CDK](https://github.com/aws/aws-cdk): IaC for AWS Cloud written in TypeScript with APIs for multiple programming languages.

