General Execution:

```
bin/start.sh GCP_PROJECT=<gcp-project-id> \
REGION=<region>  \
SUBNET=<subnet>   \
GCS_STAGING_BUCKET=<gcs-staging-bucket-folder> \
HISTORY_SERVER_CLUSTER=<history-server> \
TEMPLATE_NAME=GCSTOBIGQUERY 
```

### Configurable Parameters
Update Following properties in  [template.properties](../../../../../../../resources/template.properties) file:
```
project.id=<project id>
gcs.bigquery.input.format=<avro,parquet,csv,json>
gcs.bigquery.input.location=<input file location>
gcs.bigquery.output.dataset=<bq output dataset>
gcs.bigquery.output.table=<bq output table>
gcs.bigquery.temp.bucket.name=<temp bucket>
```
