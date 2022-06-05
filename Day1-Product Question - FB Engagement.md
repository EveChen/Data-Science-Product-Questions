# Question: How would you improve engagement on FB?
  * Need to define "engagement" first. What are the metrics of interest?
  * I assume this is an interview question from Facebook (Meta) itself? If it's from a different company whose goal is to maximize their revenue from FB ads, my thought process would be different.


##### Firstly, the engagement means how the users 'play' on FB. This means the metric we find should be able to measure user's activity on FB. In this case, I would choose the **participation rate** as my metric. To be more specific, we will calculate how many times did the users click a "like" or post a feed within a day.
  * Does "like" mean any button, or do we distinguish between "like", "love", "care", "haha", "wow", "sad", "angry"?
  * What types of posts did the users click on? e.g. friends' posts, group posts, FB pages, sponsored ads.

##### Secondly, I would collect other data like:
  * Demographic data: Age, location, gender, education (consider the prevalence of missing data)
  * Engagement data: number of friends, how many feeds did a user have, how long did a user use FB per day
  * Device data: what platform did a user use (phone/PC/laptop/iPad), what browser did a user use (Google Chrome/Edge/Safari etc)
  
##### After we collect those data, we will use a simple model to see which features play as the important factors toward the engagement? Here, I would use the **random forest** because a function **VarImpPlot** will show the importance of each features. Of course we can use other methods like the correlation or model comparisons to select the features.

##### Because our final goal is to **improve the engagement on FB**, I may not modify my random forest model to have a highest accuracy. Instead, once I know the important features, I would put much focus on the recommodation. For example, let's say we found **the number of friends** factor has a postive impact on the engagement (i.e. if we have more friends on FB, we will increase the engagement on FB). We can **recommend** new friends to a user to broaden the interpersonal relationship so that the user may have more feeds to read/like.
