#### 接受需求本體的序列化 JSON

接受於 `PUT`、`PATCH`、`POST` 需求本體中的序列化 JSON，使其可與表單資料並存，或取代它。這與回應本體的序列化 JSON 相呼應，例如：
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
