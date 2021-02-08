The Databricks add-on for Splunk allows Splunk Enterprise and Splunk Cloud users to run queries and execute actions, such as running notebooks and jobs, in Databricks. The add-on also makes it easy to send events from Databricks to Splunk via Splunk HEC.
### Features
- Run Databricks SQL queries right from the Splunk search bar and see the results in Splunk UI
- Execute actions in Databricks, such as notebook runs and jobs, from Splunk
- Push events, summary, alerts to Splunk from Databricks
- Pull events, alerts data from Splunk into Databricks
<img src="/docs/functional_architecture.png" height="70%" width="70%">

#### Bidirection Splunk Connector documentation:

* Databricks Add-on for Splunk Integration Installation And Usage Guide:
   * Documenation:  [[markdown](/docs/markdown/Splunk%20Integration%20Installation%20And%20Usage%20Guide.md),[pdf](/docs/pdf/Splunk%20Integration%20Installation%20And%20Usage%20Guide%20-%201.0.0.pdf),[word](/docs/word/Splunk%20Integration%20Installation%20And%20Usage%20Guide%20-%201.0.0.docx)]
   * [Link to Databricks add-on for Splunk on Splunkbase](https://splunkbase.splunk.com/app/5416)
* Splunk DB Connect Guide for Databricks:
  * Documenation:  [[markdown](),[pdf](/docs/pdf/Splunk%20DB%20Connect%20Guide%20for%20Databricks.pdf),[word](/docs/word/Splunk%20DB%20Connect%20Guide%20for%20Databricks.docx)]
* Push Data to Splunk from Databricks.docx: 
  * Documenation: [[markdown](),[pdf](/docs/pdf/Push%20Data%20to%20Splunk%20from%20Databricks.pdf),[word](/docs/word/Push%20Data%20to%20Splunk%20from%20Databricks.docx)]
  * [Notebook](/notebooks/dbc/push_to_splunk.dbc)
* Pull Data from Splunk into Databricks.docx:
  * Documenation:  [[markdown](),[pdf](/docs/pdf/Push%20Data%20to%20Splunk%20from%20Databricks.pdf),[word](/docs/word/Push%20Data%20to%20Splunk%20from%20Databricks.docx)]
  * [Notebook](/notebooks/dbc/pull_from_splunk.dbc)

### Data collection sources with Notebooks and documentation are included for the following sources: 

This project also provides documentation and notebooks to show case specifics on how to use Databricks for collecting varous logs (a comprehensive list is provided below) via stream ingest and batch-ingest using Databricks autoloader and Spark streaming into cloud Data lakes for durable storage on S3. The included documentation and notebooks also provide methods and code detials for each log type: parsing, schematizing, ETL/Aggregation, and storing in Delta format to make them available for analytics. 

#### Log Collection documentation:

* Cloudtrail logs
  * Documenation: [[markdown](),[pdf](/docs/pdf/Databricks%20%20-%20AWS%20CloudTrail.pdf),[word](/docs/word/Databricks%20%20-%20AWS%20CloudTrail.docx)]
  * [Notebook 1](/dbc/cloudtrail_ingest.dbc)
  * [Notebook 2](/dbc/cloudtrail_insights_ingest.dbc)
* VPC flow logs
  * Documenation: [[markdown](),[pdf](/docs/pdf/Databricks%20-%20AWS%20VPC%20Logs.pdf),[word](/docs/word/Databricks%20-%20AWS%20VPC%20Logs.docx)]
  * [Notebook](dbc/vpc_flowlogs_ingest.dbc)
* syslogs
  * Documenation: [[markdown](),[pdf](/docs/pdf/Databricks%20-%20Syslog.pdf),[word](/docs/word/Databricks%20-%20Syslog.docx)]
  * [Notebook 1](dbc/syslog_rfc3164.dbc) 
  * [Notebook 2](dbc/syslog_rfc5424.dbc) 
