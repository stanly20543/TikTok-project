## **TikTok Project**


TikTok is working on the development of a predictive model that can determine whether a video contains a claim or offers an opinion

TikTok users have the ability to report videos and comments that contain user claims. 
These reports identify content that needs to be reviewed by moderators.
This process generates a large number of user reports that are difficult to address quickly. 

TikTok is working on the development of a predictive model that can determine whether a video contains a claim or offers an opinion.
With a successful prediction model, TikTok can reduce the backlog of user reports and prioritize them more efficiently.

### **Part1: Clean and investigate data**

 -**Target**:<br> 
 To get clear insights, the data must be inspected, organized, and prepared for analysis.<br>

 -**Conclusion**: <br>
 There are 50.3% and 49.7% for claim video and opinion video,
but are more interactions with claim video. It should be a key to explore more detailly.

### **Part2: Explore and analyze data**

-**Target**:<br>
 Exploratory data analysis and data visualization<br>

-**Conclusion**:<br>
In the histograms, the vast majority of videos are grouped at the bottom of the range of values for three variables (view, like, comment) that showcase TikTok users engagement with the videos.<br>
Classification model will need to account for these variables and imbalance in opinion video counts.<br>


### **Part3: Statistic analysis**

-**Target**:<br>
To determine whether there is a statistically significant difference in the number of views for TikTok videos posted by verified accounts versus unverified accounts


-**Conclusion**:<br>
There might be fundamental behavioral differences between these two groups: **_verified accounts_** and **_unverified accounts_**.<br> 

### **Part4: Build linear regression model**

-**Target**:<br>
 To explore how to predict verified status to help them understand how video characteristics relate to verified users. The results may be used to inform the final model related to predicting whether a video is a claim vs an opinion.<br>

-**Conclusion**:<br>
 From the logistic regression, beside `claim_status` and `author_ban_status`, longer videos tend to be associated with higher odds of the user being verified.<br>


### **Part5: Build tree-base model**

-**Target**:<br>
 To develop a machine learning model to assist in the classification of videos as either claims or opinions. <br>

-**Conclusion**:<br>
 The primary predictors were all related to video engagement levels, like `video_view_count`, `video_like_count`, `video_share_count`, `video_download` are the most important features to determine the video is claim or opinion.

