# Question: How would you improve engagement on FB?

##### Firstly, the engagement means how the users 'play' on FB. This means the metric we find should be able to measure user's activity on FB. In this case, I would choose the **participation rate** as my metric. To be more specific, we will calculate how many times did the users click a "like" or post a feed within a day.
##### Secondly, I would collect other data like:
  * Demographic data: Age, location, degree, gender
  * Engagement data: numbers of friends, how many feeds did an user have, how long did an user use FB per day
  * Device data: what platform did an user use (phone/PC/notebook), what browser did an user use (Google Chrome/IE/Safari etc)
##### After we collect those data, we will use a simple model to see which features play as the import factors toward the engagement? Here, I would use the **random forest** because a function **VarImpPlot** will show the importance of each features. Of course we can use other methods like the correlation or model comparisons to select the features.
##### Because our final goal is to **improve the engagement on FB**, I may not modify my random forest model to have a higest accuracy. Instead, once I know the important features, I would put much focus on the recommodation. For example, let's say we found **the numbers of friends** factor has a postive impact on the engagement (i.e. if we have more friends on FB, we will increase the engagement on FB). We can **recommend** new friends to an user to broaden the interpersonal relationship so that the user may have more feeds to read/like.
