#### 保持所有回應中的 JSON 最小化

額外的空白增加了無用的回應大小，而許多人用的客戶端會將 JSON 輸出自動排版。所以最好讓 JSON 回應最小化，例如：

```json
{"beta":false,"email":"alice@heroku.com","id":"01234567-89ab-cdef-0123-456789abcdef","last_login":"2012-01-01T12:00:00Z","created_at":"2012-01-01T12:00:00Z","updated_at":"2012-01-01T12:00:00Z"}
```

而非：

```json
{
  "beta": false,
  "email": "alice@heroku.com",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "last_login": "2012-01-01T12:00:00Z",
  "created_at": "2012-01-01T12:00:00Z",
  "updated_at": "2012-01-01T12:00:00Z"
}
```

您可考慮讓客戶端額外取得更詳細的回應，透過查詢參數 (如 `?pretty=true`) 或 `Accept` 標頭參數 (如
`Accept: application/vnd.heroku+json; version=3; indent=4;`)。
