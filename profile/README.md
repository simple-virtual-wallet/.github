# simple virtual wallet 簡單虛擬錢包 - by Josh Tsai

**simple virtual wallet**是一個錢包的系統，為[Paper Trade Chatbot](https://github.com/simple-virtual-wallet) 中的錢包部分擷取出來，使用java spring boot撰寫與grpc架設，利用microservice架構結合mysql, redis等資源架設，使用者可以註冊會員、出入金。

### 簡介
本系統為用來練習`java spring boot`的side project，商業邏輯部份由Josh獨立開發完成，目前僅開發後端部份。

### 微服務

simple virtual wallet 包含以下微服務：

* `auth` 登入、驗證(還未連接redis)
* `user` 用戶註冊、用戶資料(僅完成新增用戶，還未加入驗證)
* `wallet` 用戶錢包資料、交易(僅完成新增錢包、處理交易，還未加入驗證)

### 資源

* `mysql` 各microservice各自有其schema，便於拆分db使用量

### Postman

還未寫swagger，暫時先提供postman:
* [user api](https://api.postman.com/collections/4586812-a0c62082-1e88-45ab-b4c8-eb9d310d401c?access_key=PMAT-01H266TPNYZFNTQXWQH21M1X4C)
* [wallet api](https://api.postman.com/collections/4586812-379e3bd4-63bc-4b5c-a625-265461a4d7c6?access_key=PMAT-01H266Y4MD4H18T8Y5AX056J8H)
* [auth api](https://api.postman.com/collections/4586812-cb5390ef-160c-4906-95f8-736a14af6aa5?access_key=PMAT-01H266CAXS2SS861VT5WBMY5CQ)


---

## 開發者
以上程式商業邏輯與相關工具開發來自 [Josh](https://github.com/lisyaoran51), 系統設計架構參考101投資平台, 重新撰寫並優化流程
