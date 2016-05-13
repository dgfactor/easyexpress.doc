# CM4 REST API 文件

## 名詞定義

+ slug

    每個站台的唯一識別代碼，必須是 小寫字母，數字以及底線的組合。例如 ( easyexpress,  _demo01 ... )
    
+ APIBase
    
    網站提供的 API 必須是 APIBase url + 各個 API 的網址組合。 
    根據不同的專案可能會有不同的 APIBase 格式為 https://easy.express/{slug}/api。
    
+  APIPath

    例如 APIPath 為  /contactus
    網址 API 就應該是 APIBase + APIPath => http://easy.express/{slug}/api/contactus


## Request 方式

參數必須以 JSON 格式放在 request content 中

request header 必須包含

```
Content-Type: application/json
Accept: application/json
```

request content

```
{
   "name" : "my_username",
   "first-name" : "My",
   "last-name" : "Username",
   "display-name" : "My Username",
   "email" : "user@example.test",
   "password" : {
      "value" : "my_password"
   },
   "active" : true
}
```

完整的 Http 傳輸內容


## Response 方式

以 http status code 代表成功或失敗

```
200:    成功
4xx:    失敗
```

Content:    json 格式

