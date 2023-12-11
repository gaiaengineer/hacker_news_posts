# Exploring Hacker News Posts
## Project Description
In this project, I compare two types of posts from a popular site [Hacker News](tab:https://news.ycombinator.com/) to determine: 

* Which of them receive more comments on average?
* Do posts created at a certain time receive more comments on average?

The types of posts I'm interested in are ```Ask HN``` (created to ask a question to the community) and ```Show HN``` (created to show the community a project that you've created). 

## Data Set
[Hacker News](tab:https://news.ycombinator.com/) is a site started by the startup incubator [Y Combinator](tab:https://www.ycombinator.com/), where user-submitted stories (known as "posts") receive votes and comments, similar to reddit. Hacker News is extremely popular in technology and startup circles, and posts that make it to the top of the Hacker News listings can get hundreds of thousands of visitors as a result.

The original dataset can be found [on Kaggle](tab:https://www.kaggle.com/datasets/hacker-news/hacker-news-posts). For this project, the original dataset was downsampled to [this set](tab:https://dq-content.s3.amazonaws.com/356/hacker_news.csv). The number of rows was reduced from almost 300,000 rows to approximately 20,000 rows by removing all submissions that didn't receive any comments and then randomly sampling from the remaining submissions.

### The descriptions of the columns

* ```id```: the unique identifier from Hacker News for the post
* ```title```: the title of the post
* ```url```: the URL that the posts links to, if the post has a URL
* ```num_points```: the number of points the post acquired, calculated as the total number of upvotes minus the total number of downvotes
* ```num_comments```: the number of comments on the post
* ```author```: the username of the person who submitted the post
* ```created_at```: the date and time of the post's submission

## Technologies
* [Python](https://www.python.org):
  * **data analysis:** working with strings, OOP (Object-Oriented Programming), working with dates and times 
* [Jupyter Notebook](https://jupyter.org)
