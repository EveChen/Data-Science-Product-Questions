# Probability Question - Microsoft
### Question: a和b玩骰子，先擲到6的算贏，問a贏的概率
### My Answer: 

# Case1
假設 a 先骰骰子且骰子公正 (fair dice)
1. a 1st round win = 1/6
2. a 2nd round win = a 1st round lose & b 1st round lose & a 2nd round win = 1/6 * 5/6 * 5/6
3. etc
                                                                     
### 故 a win probability = 1/6 + 1/6 * (5/6)^2 + 1/6 * (5/6)^4 + 1/6 * (5/6)^6 + ...
### 無窮等比級數公式 a1 / (1 - r), 其中，a1 = 1/6, r = (5/6)^2, 故答案 = 6/11

# Case2
假設 a 先骰骰子，但骰子不公正
1. a 1st round win = p, lose = 1-p
2. a 2nd round win = p * (1-p)^2
3. a 3rd round win = p * (1-p)^4
4. etc

### 根據無窮等比級數公式: p / (1 - (1-p)^2) = 1/(2-p)

##### Credit to:
http://www.1point3acres.com/bbs/forum.php?mod=viewthread&tid=206057&extra=page%3D1%26filter%3Dsortid%26sortid%3D311%26sortid%3D311
