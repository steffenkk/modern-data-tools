# List of Modern Data Tools

## What do you get?
- A list of tools used in "the modern data stack" 
- Short describtions of the tools and their use cases
- Links to the projects / companies behind these tools

## What is "the modern data stack", actually?
Thats a tough one! You can't really say that there is something as the one and only modern data stack. However, there are certain ideas/tools/do's and dont's/etc. that can be combined to form a thing which is modern and is a data stack. These tools are generally easy-to-use, open, cloud-native or even SaaS. Go Data Driven has a [blog article](https://godatadriven.com/blog/modern-data-stack-the-road-to-democratizing-data/) that describes this pretty well. Now do you ask yourself: "So that's it, I just switch all my tools to those listed here and then I have it?" - far from it! As always, it's people's business ...

## TODO:
- add lists
- add best practices?
- add more describtion

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


- [DBT]()
- [AWS Glue]()
- [Google Data Fusion]()
- [Databricks]()


## data-orchestration
Answer the question: which data comes in from where and when?

- [Airflow](https://airflow.apache.org/): open-source platform to orchestrate and monitor workflows with several integrations and a powerful UI.
- [Google Cloud Composer](https://cloud.google.com/composer): Cloud based version of Airflow in GCP.
- [AWS Stepfunctions](https://aws.amazon.com/step-functions/): Serverless orchestration tool for AWS Services.
- [Dagster](https://dagster.io/): open-source data orchestration tool to build DAGs and run them. Provides an UI, CLI and an API. 
- [Prefekt](https://www.prefect.io/): data orchestration SaaS tool with API, UI and CLI.


## data-analytics
Answer the question: how can we access tha data?

- [Snowflake]():
- [Google BigQuery]():
- [Azure Synapse Analytics]():
- [AWS Redshift]():
- [Dremio](): data lake house with dremio.
- [Databricks](): Walk into your data lake house with databricks.
- [Trino (formerly PrestoSQL)](): SQL-Based federated query engine to query files in your data lake as well as distributed databases.


## data-visualization
Answer the question: what does the data tell us?

- [Tableau]()
- [Looker]()
- [PowerBI]()
- [ThoughtSpot]()


## data-quality
Answer the question: can we trust that data?

- [Datafold]()
- [Monte Carlo]()
- [Great Expectations]()

## data-explorability
Answer the question: what data do we actually have?

- [Atlan](https://atlan.com/platform/data-catalog/): A modern data catalog for the modern data stack. Integrate and expose all your data assets in a curated and centralized repository. 
- [Tableau Data Management Add-On]():
- [DBT Docs]():
- [DBT Docs]():


## machine-learning
Answer the question: what can the data tell us about the future?


- [Amazon Sagemaker](https://aws.amazon.com/sagemaker/): Build, train, deploy, and monitor machine learning models with this platform in AWS.
- [Databricks Managed ML Flow](https://databricks.com/product/managed-mlflow): An open source machine learning platform based on top of Apache Spark.
- [Azure Machine Learning](https://azure.microsoft.com/en-us/services/machine-learning/#features)


## languages
Answer the question: how to do all this?


- [SQL](https://en.wikipedia.org/wiki/SQL): Database Query Language, the must-have for all data peoples.
- [Python](https://www.python.org/): the *best* programming language on earth (author's opinion 😜).
- [Terraform](https://www.terraform.io/): Infrastructure as code (IaC) for multiple cloud providers. Uses own language (HCL).
- [Pulumi](https://www.pulumi.com/): IaC for multiple cloud providers. Uses mainstram languages like JavaScript and Python.
- [AWS CDK](https://github.com/aws/aws-cdk): IaC for AWS Cloud written in TypeScript with APIs for multiple programming languages.

