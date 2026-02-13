# cloud-monitor-vertex-pt-mql

# Vertex AI — Tokens Per Query by Type

MQL query that can be used on Google Cloud Monitoring dashboards and metrics explorer.
Calculates the **average tokens per query**, broken down by token type (input, output, image, reasoning).

## Usage

1. Open [Google Cloud Monitoring → Metrics Explorer](https://console.cloud.google.com/monitoring/metrics-explorer)
2. Switch to **MQL** mode
3. Paste the contents of `tokens_per_query_by_type.mql`
4. Adjust the time window (`7d`) as needed

## Output

| metric.type        | Description                        |
|--------------------|------------------------------------|
| `input`            | Input text tokens per query        |
| `input_image`      | Image input tokens per query       |
| `output`           | Output text tokens per query       |
| `output_reasoning` | Reasoning output tokens per query  |

## Additional Reference

[Calculate Provisioned Throughput requirements](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/provisioned-throughput/measure-provisioned-throughput)
