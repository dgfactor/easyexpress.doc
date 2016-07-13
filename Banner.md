# Banner API

+ APIPath

  例如 APIPath 為 /banner 網址 API 就應該是 APIBase + APIPath => https://easy.express/{slug}/api/banner/{id}

## 取得Banner版位內容

|請求方式||
|--------|-----|
| Method | GET |
| Url    | /banner/{id} |

### 傳入參數

Url:

| 欄位  | 型態 | 欄位說明 |
|-------|------| -------- |
| id  | integer | Banner版位ID |


Query:

**無**

Content:

**無**

### 回傳結果
| 欄位  | 型態 | 欄位說明 |
|-------|------|----------|
| Id | integer | Banner版位 ID |
| Name | string | Banner版位標題 |
| Photo | [Photo](Photo.md) [] | 照片 |
| CreatedAt | DateTime (W3C) | 建立時間 |
| UpdatedAt | DateTime (W3C) | 更新時間 |

### 錯誤
| 狀態碼  | 錯誤說明 |
|---------|----------|
|404| 找不到Banner版位 |
