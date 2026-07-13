# Mock governed run

This example is descriptive only. It does not invoke the private ZipVerse engine.

## Submitted packet

See [`basic-task-packet.json`](basic-task-packet.json).

## Illustrative decision

```json
{
  "schema_version": "0.1",
  "task_id": "example-docs-check-001",
  "status": "accepted",
  "summary": "The packet is valid, read-only, and within the declared public-documentation scope.",
  "evidence": [],
  "errors": [],
  "metadata": {
    "mock": true
  }
}
```

## Illustrative completion

```json
{
  "schema_version": "0.1",
  "task_id": "example-docs-check-001",
  "status": "completed",
  "summary": "Review completed. Two broken links were reported. No files were modified.",
  "evidence": [
    {
      "type": "report",
      "reference": "mock://reports/example-docs-check-001"
    }
  ],
  "errors": [],
  "metadata": {
    "mock": true,
    "independent_review": "passed"
  }
}
```

A future mock runtime will generate equivalent contract-safe responses locally.
