# 聯絡我們 API

## 取得聯絡我們內容

|請求方式||
|--------|-----|
| Method | POST |
| Url    | /contactus/ |

### 傳入參數

Url:

**無**

Query:

**無**

Content:

|欄位|型態|欄位說明|
|--|--|
|Username|string|姓名|
|Email|email|電子郵件|
|Phone|integer|電話|
|Content|string|內容|

### 回傳結果
| 欄位  | 型態 | 欄位說明 |
|--|--|
| Id | integer | 聯絡我們 ID |

### 錯誤
| 狀態碼  | 錯誤說明 |
|--|--|
|400| 錯誤的請求 |
