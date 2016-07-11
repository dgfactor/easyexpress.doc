# 訂單模組 API

+ APIPath

  例如 APIPath 為 /order 網址 API 就應該是 APIBase + APIPath => https://easy.express/{slug}/api/order


## 試算訂單金額

|請求方式||
|--------|-----|
| Method | POST |
| Url    | /query |

### 傳入參數

Url:

**無**

Query:

**無**

Content:



### 回傳結果

|欄位|型態|欄位說明|
|----|----|--------|
| Amount | bigint | 總金額 |
| AmountForPay | bigint | 應付金額 |
| OrderItems | ------ | 關聯欄位 |
| CreatedAt | DateTime (W3C) | 建立時間 |
| UpdatedAt | DateTime (W3C) | 更新時間 |
| Payment | String | 付款方式 |

|關聯欄位|型態|欄位說明|
|----|----|--------|
| ProductName | String | 產品名稱 |
| UnitPrice | bigint | 產品價格 |
| Quantity | bigint | 產品數量 |

### 錯誤

| 狀態碼  | 錯誤說明 |
|---------|----------|
| 403 | 沒有權限 |
