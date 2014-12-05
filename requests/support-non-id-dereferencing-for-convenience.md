#### 支援非 ID 的便利存取

以 ID 來辨別資源對使用者來說有時很不方便。舉個例子，使用者會以 Heroku app 名稱來思考，但那個 app 可用 UUID 辨識。這種情況您會希望同時接受 ID 與名稱，例如：

```bash
$ curl https://service.com/apps/{app_id_or_name}
$ curl https://service.com/apps/97addcf0-c182
$ curl https://service.com/apps/www-prod
```

不要只接受名稱而排除 ID。