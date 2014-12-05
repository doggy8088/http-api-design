#### 巢狀表示外來鍵關係

以巢狀結構物件序列化外來鍵，例如：

```javascript
{
  "name": "service-production",
  "owner": {
    "id": "5d8201b0..."
  },
  // ...
}
```

而非如此：

```javascript
{
  "name": "service-production",
  "owner_id": "5d8201b0...",
  // ...
}
```

這種方法可記錄更多有關資源關係的訊息，而不用改變回應的結構或帶來更多上層的回應欄位，例如：

```javascript
{
  "name": "service-production",
  "owner": {
    "id": "5d8201b0...",
    "name": "Alice",
    "email": "alice@heroku.com"
  },
  // ...
}
```

而非如此：

```javascript
{
  "name": "service-production",
  "owner_id": "5d8201b0...",
  "owner_name": "Alice",
  "owner_email": "alice@heroku.com"
  // ...
}
```