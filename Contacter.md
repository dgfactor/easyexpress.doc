# 聯絡人API

+ APIPath

  例如 APIPath 為 /contacter 網址 API 就應該是 APIBase + APIPath => https://easy.express/{slug}/api/contacter/{id}

## 取得聯絡人列表

|請求方式||
|--------|-----|
| Method | GET |
| Url    | /contacter/{id} |

### 傳入參數

Url:

| 欄位  | 型態 | 欄位說明 |
|-------|------| -------- |
| id  | integer | 會員ID |

Query:

**無**

Content:

**無**

### 回傳結果

#### array

| 欄位 | 型態 | 欄位說明 |
| ----| ---- |------- |
| name | string | 聯絡人姓名  |
| email | string | 聯絡人E-mail  |
| phone | string | 聯絡人電話  |
| zip | string | 聯絡人郵遞區號  |
| address | string | 聯絡人地址  |

### 錯誤

| 狀態碼  | 錯誤說明 |
|---------|----------|
| 400 | 錯誤的請求 |

## 新增聯絡人

|請求方式||
|--------|-----|
| Method | POST |
| Url    | /contacter/create |

### 傳入參數

Url:

**無**

Query:

| 欄位  | 型態 | 欄位說明 |
|-------|------| -------- |
| memberId  | integer | 會員ID |
| name | string | 聯絡人姓名  |
| email | string | 聯絡人E-mail  |
| phone | string | 聯絡人電話  |
| zip | string | 聯絡人郵遞區號  |
| address | string | 聯絡人地址  |

Content:

**無**

### 回傳結果

| 欄位 | 型態 | 欄位說明 |
| ----| ---- |------- |
| id | integer | 聯絡人ID  |
