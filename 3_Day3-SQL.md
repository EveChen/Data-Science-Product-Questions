# SQL
### Question: [name,sports category]; [user id, name, date], [user id, following id, date following]
* Q1: 求每個category的follower
* Q2: 求有多少個NBA category follow NFL
### Q1 Answer: 把table1 & 2用 name 相連，最後算 SUM
Code: Select SUM(sports_category)
      From table1 join table2 
      On table1.name = table2.name;
      
### Q2 Answer: 用 Where 去看 category 中 follow NFL 的，然後用 COUNT 去計算 category 數量
Code: Select Count(sports_category)
      From table1
      Where sports_category == "NFL";
      
# 弱點
1. Q1 跟 Q2 SUM 跟 COUNT 實際運用
2. Q2 中如果 NFL 無法完全 == sports_category 字串? 例如 "ABC NFL"? 要怎麼用 Where 去包含?
