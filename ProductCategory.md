# 分類 API

## 取得分類

|請求方式||
|--------|-----|
| Method | GET |
| Url    | /productcategory/{id} |

### 傳入參數

Url:

| 欄位  | 型態 | 欄位說明 |
|-------|------| -------- |
| id  |integer| 分類ID |


Query:

**無**

Content:

**無**

### 回傳結果
| 欄位  | 型態 | 欄位說明 |
|-------|------|----------|
| Id | integer | 產品 ID |
| Name | string | 產品名稱 |
| Code | string | 產品編號 |
| Brief | string | 產品簡介 |
| Photos | [Photo](Photo.md) [] | 照片 |
| CreatedAt | DateTime (W3C) | 建立時間 |
| UpdatedAt | DateTime (W3C) | 更新時間 |

### 錯誤
| 狀態碼  | 錯誤說明 |
|---------|----------|
|404| 找不到分類 |



## 取得產品

|請求方式||
|--------|-----|
| Method | GET |
| Url    | /productcategory/{id} |

### 傳入參數

Url:

| 欄位  | 型態 | 欄位說明 |
|-------|------|--------- |
| id  |integer| 產品ID |


Query:

**無**

Content:

**無**

### 回傳結果
+ Category

|欄位|型態|欄位說明|
|----|----|--------|
| Id | integer | 分類ID |
| Name | string | 分類名稱 |
| MetaData | [Photo](Photo.md)[] | 照片 |

+ Product

| 欄位  | 型態 | 欄位說明 |
|-------|------|----------|
| Id | integer | 產品 ID |
| Name | string | 產品名稱 |
| Code | string | 產品編號 |
| Brief | string | 產品簡介 |
| Photos | [Photo](Photo.md) [] | 照片 |
| CreatedAt | DateTime (W3C) | 建立時間 |
| UpdatedAt | DateTime (W3C) | 更新時間 |

### 錯誤
| 狀態碼  | 錯誤說明 |
|---------|----------|
|404| 找不到產品分類 |
