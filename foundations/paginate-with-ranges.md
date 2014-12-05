#### 以 Range 分頁

將任何可能產生大量資料的回應做分頁。使用 `Content-Range` 標頭來傳達分頁需求。
需求與回應標頭、狀態碼、限制、排序及逐頁瀏覽的詳細內容，可參考 [Heroku Platform API on Ranges](https://devcenter.heroku.com/articles/platform-api-reference#ranges) 的範例。