# Reddit-WebScraping
Python project using PRAW for web scraping Reddit's DataScience subreddit to collect and clean data from top posts and comments in 2024.

# Overview
Reddit, a social news and discussion platform, is a vast online community with millions of users. The platform is known for its diverse content, from politics to poultry farming and gaming to green hydrogen. This project discusses one subreddit in particular – r/datascience and how we can collect/explore data from it

# Why Reddit ?
Reddit's unique upvote/downvote system allows users to collectively determine the most popular content. Analyzing top reddit posts on data science can provide valuable insights on what real practitioners and soon to be data scientists are concerned about. In addition, users are assumed to be anonymous and are more likely to share their opinions without any reservations. Lastly, Reddit data can be accessed programmatically with the help of a Python library that allows easy interaction with the Reddit API.

# Methodology
For fetching reddit posts from the data science subreddit, we use Python Reddit API Wrapper(PRAW)
Key features:
1) It can be used to access popular posts, search for content and explore different categories of reddit data
2) Simplifies making API requests to reddit
3) Offers methods to filter and sort data based on various criteria, such as time range, score, and more

![image](https://github.com/user-attachments/assets/134fea48-2ded-4f7e-bbf8-cad0abd93003)

 # Criteria for filtering out the posts

![image](https://github.com/user-attachments/assets/3ac03fab-c7ad-424b-820d-5457f847b374)

1) Year - Posts of the year 2024 are likely to showcase content that resonates strongly with the data science subreddit community
2) Importance of the posts - Only posts with score more than 50 are to be considered. Those with a lesser score may not be valuable for our purpose 
3) No. of words in the title - Beware of jokes and memes which usually have less than 5 words in the title.
4) No. of posts - We need our data set to be sufficiently large to explore the concerns of the subreddit community. A limit of 100 posts would be adequate to achieve this

Once the data is collected, it is converted into a dataframe and exported into a format that is more readable such as a CSV file. It will have relevant details of the posts such as body of the post, title, top 3 comments, time of the post in a readable format

# Inference from the data
The posts & comments that we collected highlight several key points
1) Data Science Jobs in Sports - Discussions surrounding use of data in baseball, basketball, cricket and soccer
2) Skills required to be successful in the field - Comments on what kind of math, coding and interpersonal skills could potentially lead to a successful career
3) Vagueness of job descriptions - Remarks on what kind of jobs one could target to have a rewarding careerwhich maybe contradictory to how they are titled
4) Amount of math required to be successful - Is Data Science only meant for statisticians ?

![image](https://github.com/user-attachments/assets/ad63fdd1-0fd6-444b-950e-169a230c1439)

# Conclusion and Takeaways
1) Web Scrapping of Reddit - It was achieved by familiarizing ourselves with PRAW by following the official documentation before proceeding to gather the data
2) Data cleaning - We had to exercise caution once the data was gathered by filtering it as per our custom requirements and exporting the resulting dataframe into a csv file
3) Current landscape - The top posts reflect job openings in unexpected fields, concerns of soon to be data scientists and key skills that could lead to a rewarding career
4) Insights - Analyzing the top posts provides valuable insights into user preferences which could potentially enable us to take better decisions
