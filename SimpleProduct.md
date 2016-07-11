# 簡單產品 API (尚未寫好)

+ APIPath

  例如 APIPath 為 /simpleproduct 網址 API 就應該是 APIBase + APIPath => https://easy.express/{slug}/api/simpleproduct/

## 取得產品內容

|請求方式||
|--------|-----|
| Method | GET |
| Url    | /simpleproduct |

### 傳入參數

Url:

| 欄位  | 型態 | 欄位說明 |
|-------|------| -------- |
| id  | integer | 產品編號 |


Query:

**無**

Content:

**無**

### 回傳結果
| 欄位  | 型態 | 欄位說明 |
|-------|------|----------|
| Id | integer | 產品 ID |
| Name | string | 產品名稱 |
| ProductCode | string | 產品編號 |
| Brief | string | 產品簡介 |
| Content | string | 產品內容 (html 格式) |
| Status | boolean | 產品狀態 |
| Price | integer | 產品價格 |
| Photos | [Photo](Photo.md) [] | 照片 |
| CreatedAt | DateTime (W3C) | 建立時間 |
| UpdatedAt | DateTime (W3C) | 更新時間 |

### 錯誤
| 狀態碼  | 錯誤說明 |
|---------|----------|
|404| 找不到產品 |
