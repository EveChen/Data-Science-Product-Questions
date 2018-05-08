# SQL
### Question & Answer: Find the average cost of each advertisements given the following two tables
http://tpcg.io/7wzqGi
#### 就我的理解，此題目中有兩個 Tables:
* Advertisement_Info: 裡面有九家公司委託 FB 幫忙刊登廣告，其中有三款廣告形式，spend 代表該公司刊登其中一款廣告的總支出費用
* ad_info: 記載了哪些使用者點擊該款廣告，price 則代表使用者願意為該產品所支付的價格
* 例如: A01 公司採用 001 號廣告，總共支付了 $200；而 001 號廣告有 B01 和 B04 兩位使用者點擊，最後他們分別支付 $500 跟 $800 產品費用

# Product Question
### Question: 如果 FB 想了解目前廣告能否讓刊登廣告的廠商滿意，該如何設計 metrics? 先解釋，再用 SQL 表達。
### Answer: 
* 「滿意」代表公司願意為該款廣告付高價格，所以 SQL 用 Max 去找三款廣告的 Max 是多少
  - Code1: http://tpcg.io/dyvgaJ
* 使用者滿意 == 有賺錢 == 有 Revenue，而 Revenue = 產品價格 - 成本。我想創造新的 column 去存每間公司的 Revenue (見 Code2)
  - Code2: 


##### Credit to: http://www.1point3acres.com/bbs/forum.php?mod=viewthread&tid=235689&extra=page%3D1%26filter%3Dsortid%26sortid%3D311&page=1

##### 本紀錄僅為個人練習使用
