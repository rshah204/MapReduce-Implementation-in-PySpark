MapReduce Implementation using PySpark in Google Colab
----------------

In this work, we will perform basic data processing task using PySpark.

The Amazon_Responded_Oct05.csv contatins information of 400K tweets. The following 3 columns will be used for this implementation:

1. user_id_str: user ID

2. user_followers_count: the number of followers

3. text_: the text of tweets

Tasks:

1. Find out popular users whose followers are more than 5000, and

2. Get Top 10 most popular words from the tweets posted by these popular users

Specifically, we need to do the following steps:

1. Read/load data

2. Extract the columns (user_id_str and user_followers_count and text_)

3. Remove the duplicated user id: some users have different number of followers in different rows. In this case, we will just keep the maximum number of followers for a particular user.

4. Find popular users: create a filter to find popular users who have more than 5000 followers using the new pairs in step 3.

5. Count words frequency: count words frequency of of the tweets posted by the popular users we get from step 4, and get the Top 10 most popular words and their words frequency