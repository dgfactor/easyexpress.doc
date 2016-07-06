# 分類文章 API

+ APIPath

  例如 APIPath 為 /article 網址 API 就應該是 APIBase + APIPath => https://easy.express/{slug}/api/carticles/{id}

## 取得文章內容

|請求方式||
|--------|-----|
| Method | GET |
| Url    | /carticles/{id} |

### 傳入參數

Url:

| 欄位  | 型態 | 欄位說明 |
|-------|------| -------- |
| id | bigint | 分類id |


Query:

**無**

Content:

**無**

### 回傳結果
| 欄位  | 型態 | 欄位說明 |
|-------|------|----------|
| Id | integer | 分類 ID |
| Title | string | 文章標題 |
| Brief | string | 文章簡介 |
| Content | string | 文章內容 |
| CreatedAt | DateTime (W3C) | 建立時間 |
| UpdatedAt | DateTime (W3C) | 更新時間 |

### 錯誤
| 狀態碼  | 錯誤說明 |
|---------|----------|
| Access Denied | Access Denied |