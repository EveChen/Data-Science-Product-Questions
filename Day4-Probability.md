# Probability - FB
### Question: 如何跟business的人解釋 p-value?
#### Original Definition: P-value is a measure of the strength of the evidence to reject the null hypothesis.
* 算法步驟: 先有 hypothesis, 根據 hypothesis 算統計量(e.g. Z = (x - u)/(standard deviation/sqrt(n)), 用該統計量與 significant level (alpha) 相比
* 判斷標準: 若 p-value < significant level, 則 reject null hypothesis
* 意思: p-value 指的是 reject area 那塊面積，若我們在意的值落在 reject area ，代表此值被排除在 hypothesis 之外

#### 解釋給 Business 人聽: Let's say we have a hypothesis that our average consumption of our product is around $10,000. We then collect some samples to test if our hypothesis is correct or not. Based on the samples, we know there's a reject area, that's said $12,000. This means if the new samples we collect said the average consumption is higher than $12,000, then we'll reject the hypothesis. Here, the p-value means the value above $12,000 which leads us to reject our assumption.

##### Resources:
* Blogger1:http://yenchic-blog.logdown.com/posts/159549-talking-about-the-p-value-p-value
* Youtube: https://www.youtube.com/watch?v=HTZ8YKgD0MI
* Original Question: http://www.1point3acres.com/bbs/forum.php?mod=viewthread&tid=195241&extra=page%3D1%26filter%3Dsortid%26sortid%3D311%26sortid%3D311
