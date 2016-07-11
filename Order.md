# 訂單模組 API

+ APIPath

  例如 APIPath 為 /contactus 網址 API 就應該是 APIBase + APIPath => https://easy.express/{slug}/api/payment


## 取得付款模組內容

|請求方式||
|--------|-----|
| Method | POST |
| Url    | /payment/ |

### 傳入參數

Url:

**無**

Query:

| 欄位  | 型態 | 欄位說明  |
| ---- | ---- | -------- |
| return_url | string | 付款完成後導回網址 |
| token | string | JWT token |
| payment_type | integer | 付款方式 |

Content:

**無**

### 回傳結果

RedirectResponse

### 錯誤

| 狀態碼  | 錯誤說明 |
|---------|----------|
| 400 | 錯誤的請求 |