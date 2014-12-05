#### 情況許可時提供全部資源

盡可能於回應裡呈現全部資源 (意即物件的所有屬性)。永遠於 200 與 201 回應提供全部資源，其中包含 `PUT`、`PATCH` 和 `DELETE`
需求，例如:

```bash
$ curl -X DELETE \  
  https://service.com/apps/1f9b/domains/0fd4

HTTP/1.1 200 OK
Content-Type: application/json;charset=utf-8
...
{
  "created_at": "2012-01-01T12:00:00Z",
  "hostname": "subdomain.example.com",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "updated_at": "2012-01-01T12:00:00Z"
}
```

202 回應不會完整呈現全部資源，例如：

```bash
$ curl -X DELETE \  
  https://service.com/apps/1f9b/dynos/05bd

HTTP/1.1 202 Accepted
Content-Type: application/json;charset=utf-8
...
{}
```
