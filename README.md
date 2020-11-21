# Splunk Enterprise (Locally (on k8s))

Run the free version of Splunk Enterprise (up to 500mb ingestion per day) on
your local k8s cluster.


```
helm upgrade splunk .
```


Then to ingest:

```
curl -k https://localhost:32088/services/collector/event -H "Authorization: Splunk 27a712c7-53b3-4874-aab5-2b0b08a04e38" -d '{"event": "hello world"}'
```
