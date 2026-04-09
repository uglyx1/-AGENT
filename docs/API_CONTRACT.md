# API Contract (Public Demo)

## `POST /chat`

Unified conversational entrypoint.

### Request

```json
{
  "message": "Give me products with profit greater than 100 after two-platform comparison",
  "session_id": "demo-1"
}
```

### Response Shape

```json
{
  "answer": "string",
  "intent": "string",
  "session_id": "string",
  "tool_calls": [],
  "data": {}
}
```

## `POST /compare/profit/report`

Generate structured two-platform profit report.

### Request

```json
{
  "profit_min": 100,
  "limit": 200,
  "reload_compare_source": true
}
```

### Response Fields

- `rows`: report data rows
- `table_preview_markdown`: quick preview table
- `report.download_url`: downloadable file path
- `stats`: compare stats and source metadata

## `GET /reports/download/{filename}`

Download generated report file (CSV contract in demo).

## `GET /health`

Health and runtime metadata:

- module loaded states
- retrieval backend mode
- retrieval fallback status

