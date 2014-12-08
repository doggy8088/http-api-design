#### 減少巢狀路徑

當資料模型有著多重的從屬關係，路徑可能會長成巢狀的樣子：

```
/orgs/{org_id}/apps/{app_id}/dynos/{dyno_id}
```

為了限制巢狀深度，此時可於根路徑訂定資源。使用巢狀結構標明資料範圍。
舉例而言，上述的例子中 org 所屬 app 的 dyno 可以如此標示：

```
/orgs/{org_id}
/orgs/{org_id}/apps
/apps/{app_id}
/apps/{app_id}/dynos
/dynos/{dyno_id}
```
