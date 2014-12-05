#### 接受需求本體的序列化 JSON

於 `PUT`、`PATCH`、`POST` 需求本體接受序列化 JSON，可與表單資料並存，或取代它。這與回應本體的序列化 JSON 取得平衡，例如：
```bash
$ curl -X POST https://service.com/apps \
    -H "Content-Type: application/json" \
    -d '{"name": "demoapp"}'

{
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "demoapp",
  "owner": {
    "email": "username@example.com",
    "id": "01234567-89ab-cdef-0123-456789abcdef"
  },
  ...
}
```
