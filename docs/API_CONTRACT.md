# API 契约（公开演示版）

## `POST /chat`

统一的对话入口。

### 请求示例

```json
{
  "message": "给我一份两平台对比后利润大于100的商品",
  "session_id": "demo-1"
}
```

### 返回结构

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

生成双平台利润对比报表（结构化结果）。

### 请求示例

```json
{
  "profit_min": 100,
  "limit": 200,
  "reload_compare_source": true
}
```

### 核心返回字段

- `rows`：利润对比结果行
- `table_preview_markdown`：快速表格预览
- `report.download_url`：下载路径
- `stats`：对比统计与数据源元信息

## `GET /reports/download/{filename}`

下载已生成报表文件（演示版为 CSV）。

## `GET /health`

健康检查与运行态元数据，包括：

- 模块加载状态
- 检索后端模式
- 回退状态
