# Milestone P3
Extension Project proposition - Paper 'Twitter proposals'

**1. Title**

Testing replicated propositions from Twitter studies on Instagram: generalization of social media user behavior.

**2. Abstract**

On the 10 proposals of social studies of the paper, only 4 are replicated. The authors suggest 'it might be because these propositions reflect the homogeneity of online user behaviors'. Thus the idea is to have a closer look on this statement and test if 3 of the 4 replicated proposals are robust when tested on another social media, here Instagram. As said in paper, we 'Need to retest the robustness of these propositions before we can consider them as universal’. Our goal will be to select these 3 proposals and try to replicate the results from the Twitter social studies.


**3. Research questions**

1. Is there a circadian rythm on Instagram ?
2. Do users on Instagram with most followers post more, i.e. is attention related to productivity ?
3. How is the followee-followers network distributed on Instagram ?

**4. Proposed Dataset**

- In order to answer the first question, we need an Instagram dataset containing the hour of posting, therefore [this dataset](https://github.com/eldersantos/instagram-dataset) from Github will be used. It contains the time of posting as well as the user ID.
- For the second question, we will use another [dataset on GitHub](https://github.com/samudm98/dataset_instagram/blob/master/data_set.csv) containing user ID as well as their number of followers and followees and the number of posts.
- For the third question, we will use [Huawei Social Network Data](https://www.kaggle.com/andrewlucci/huawei-social-network-data), more precisely, the Instagram network consisting of 1000 nodes and 4933 edges

**5. Methods**

The main idea is to use similar methods as in the paper in order to compare our results to the study's results.

**Data collection:** we chose to use datasets available as the access to Instagram API is very limited.

**Circadian rythm:** we will plot daily and weekly rythm of Instagram activity, i.e. plot number of tweets and number of users against the hours for each day of the week.

**Attention vs. productivity:** For attention, we will consider both followers and followees. Unfortunately, we can not consider friends (a friend is a mutual follwer-followee connection betwwen two users) as our dataset is not suited to compute reciprocity. The idea is to plot the number of followers and the number of followees against the number of tweets and add a tendency curve. We will also compute Pearson correlation between the number of followers (and followees) and the number of tweets. Then we will compare these with the Pearson correlation computed for the Twitter dataset in the paper.


**6. Proposed timeline**

**Week 1:** downloading of the datasets and first checks of consistency: visualization and exploratory data analysis.

**Week 2:** first plots to check for the ciracdian rythm, build up of the plots for the second question (is attention related to productivity ?) with the tendency curve.

**Week 3:** compute the needed values for the follower-followee network analysis

**7. Organization within the team**
