#### 顯示次數限制狀態

對客戶端限制需求次數可保障服務的健康並維持對其他客戶端好的服務品質。您可採用 [token bucket algorithm](http://en.wikipedia.org/wiki/Token_bucket) 來量化需求限制。

於每次 `RateLimit-Remaining` 回應標頭回傳剩餘的需求次數。