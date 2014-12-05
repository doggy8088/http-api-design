#### 以 Accept 標頭做版本控管

從一開始就對 API 版本控管。以 `Accepts` 標頭來協調版本，將其附加在自定內容形態 (content type) 之後，例如：

```
Accept: application/vnd.heroku+json; version=3
```

寧可不預設版本，而讓客戶端依用途採用特定版本。
