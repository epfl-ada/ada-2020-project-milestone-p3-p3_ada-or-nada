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

**Data collection:** We chose to use datasets available as the access to Instagram API is very limited.

**Circadian rythm:** In the dataset that will be used for the circadian rythm there are two different subsets of data that are interesting. The first one is the time at which the instrgram post is created, this is in relative time with respect to the local time of the creator of the dataset. The second subset that is relevant to this study is the longitude of the post, this indicates the local time at which the post is created. With these two parameters it is possible to plot the number of posts in function of the local time and thus hopefully reproduce the trend of the circadian rythm.

**Attention vs. productivity:** For attention, we will consider both followers and followees. Unfortunately, we can not consider friends (a friend is a mutual follwer-followee connection betwwen two users) as our dataset is not suited to compute reciprocity. The idea is to plot the number of followers and the number of followees against the number of posts and add a tendency curve. We will also compute Pearson correlation between the number of followers (and followees) and the number of posts. Then we will compare these with the Pearson correlation computed for the Twitter dataset in the paper.

**Followers-followees network:** : The available data is a network with the relationship of follower/followee between users in instagram. From this network, the number of mutual or singular followers will be extracted. Then the  degree distribution in the follower-followee network will be plotted for the three different relationships:  follower,followee or reciprocal.

**6. Proposed timeline**

**Week 1:** Downloading of the datasets and first checks of consistency: visualization and exploratory data analysis.

**Week 2:** First plots to check for the ciracdian rythm, build up of the plots for the second question (is attention related to productivity ?) with the tendency curve.

**Week 3:** Compute the needed values for the follower-followee network analysis and check all question results to draw conclusions

**7. Organization within the team**
