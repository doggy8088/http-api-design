#### 產生結構化的錯誤訊息

於回應本體產生一致、結構化的錯誤訊息。包含機器可讀的錯誤 `id`、一般人可讀的錯誤 `message`，以及額外的 `url` 指引客戶端更多有關此錯誤的訊息，及如何解決它，例如：

```
HTTP/1.1 429 Too Many Requests
```

```json
{
  "id":      "rate_limit",
  "message": "Account reached its API rate limit.",
  "url":     "https://docs.service.com/rate-limits"
}
```

將錯誤格式即使用者可能碰到的錯誤 `id` 寫成文件。