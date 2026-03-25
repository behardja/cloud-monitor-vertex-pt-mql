# cloud-monitor-vertex-pt-mql

MQL queries for Google Cloud Monitoring dashboards and Metrics Explorer to help measure and plan for Vertex AI [Provisioned Throughput](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/provisioned-throughput/measure-provisioned-throughput).

- [Provisioned Throughput Price Calculator](https://console.cloud.google.com/vertex-ai/provisioned-throughput/price-estimate)

## Queries

| File | Description |
|---|---|
| `tokens_per_query_by_type.mql` | Average tokens per query, broken down by token type (input, output, image, reasoning) over a 7-day window |
| `avg_qps_7d.mql` | Average queries per second (QPS) over a 7-day window, grouped by model and location |

## Usage

1. Open [Google Cloud Monitoring → Metrics Explorer](https://console.cloud.google.com/monitoring/metrics-explorer)
2. Switch to **MQL** mode
3. Paste the contents of the desired `.mql` file
4. Adjust the time window (`7d`) as needed
5. View results in the **Table** tab
6. Use the results to estimate costs with the [Provisioned Throughput Price Calculator](https://console.cloud.google.com/vertex-ai/provisioned-throughput/price-estimate)


## Additional Reference

- [Calculate Provisioned Throughput requirements](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/provisioned-throughput/measure-provisioned-throughput)
- [Burndown rates for supported models](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/provisioned-throughput/supported-models)
