# Probability Question - Microsoft
### Question: a和b玩骰子，先擲到6的算贏，問a贏的概率
### My Answer: 

# 作圖
假設 a 先骰骰子
a - win (prob = 1/6)
  - a lose (prob = 5/6) & b lose (5/6) - win (1/6)
                                       - a lose (5/6) & b lose (5/6) - win (1/6)
                                                                     - a lose (5/6) & b lose (5/6) 
                                                                     
故 a win probability = 1/6 + 1/6 * (5/6)^2 + 1/6 * (5/6)^4 + 1/6 * (5/6)^6 + ...
無窮等比級數公式 a1 / (1 - r), 其中，a1 = 1/6, r = (5/6)^2, 故答案 = 6/11

##### Credit to:
http://www.1point3acres.com/bbs/forum.php?mod=viewthread&tid=206057&extra=page%3D1%26filter%3Dsortid%26sortid%3D311%26sortid%3D311
