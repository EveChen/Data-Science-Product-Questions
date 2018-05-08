# SQL
### Question: [name,sports category]; [user id, name, date], [user id, following id, date following]
### I made 3 tables here: http://tpcg.io/6dt7ja

* Q1: 求每個category的follower
* Q2: 求有多少個NBA category follow NFL

### Q1 Answer: 把table1 & 2用 name 相連
http://tpcg.io/HGM4yQ
Code: SELECT t1.name, t1.sports_category, t2.user_id
      FROM Table1 t1
      INNER JOIN Table2 t2 ON t1.name = t2.name;
      
### Q2 Answer: 用 Where 去看 category 中 follow NFL 的，然後用 COUNT 去計算 category 數量
http://tpcg.io/ucS8Wl
Code: SELECT DISTINCT sports_category
      From table1
      WHERE name LIKE "%NFL%";
      
# 檢討
1. Q1 跟 Q2 SUM 跟 COUNT 實際運用
2. Q2 中如果 NFL 無法完全 == sports_category 字串? 例如 "ABC NFL"? 要怎麼用 Where 去包含?
### Q2: WHERE sports_category LIKE "%NFL%"


##### Credit to
http://www.1point3acres.com/bbs/forum.php?mod=viewthread&tid=423523&extra=page%3D1%26filter%3Dsortid%26sortid%3D311%26sortid%3D311
