# Model Monitoring in Airflow

### Dag and Tasks documentation 
https://airflow.apache.org/docs/apache-airflow/stable/concepts/dags.html#dag-task-documentati

### BigQuery

- To transfer between bigquery table, use BigqueryToBigQueryOperator
https://airflow.apache.org/docs/apache-airflow-providers-google/stable/_api/airflow/providers/google/cloud/transfers/bigquery_to_bigquery/index.html

- What does it mean by write_disposition and create_disposition?
- https://cloud.google.com/bigquery/docs/reference/auditlogs/rest/Shared.Types/BigQueryAuditMetadata.WriteDisposition





# mm psi tasks | project:mm_psi
* [X] write email tasks in task groups  #8f4bc09a
* [X] use pendulum to write timedelta  #6642db1b
* [X] write dag and task docs [link](https://airflow.apache.org/docs/apache-airflow/stable/concepts/dags.html#dag-task-documentation)  #0bb93299
* [X] write dag and task docs  #dba269fb
* [ ] try branch python operators  #9dafb96a
* [ ] try bigqueryoperators  #d2dc3788
    * [X] read about the operators [link](https://airflow.apache.org/docs/apache-airflow-providers-google/stable/operators/cloud/bigquery.html#check-that-a-table-exists)  #44a4e25b
* [ ] try dataflow operators  #ddb8a561
