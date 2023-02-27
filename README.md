# Qbias
𝑄𝑏𝑖𝑎𝑠 - A Dataset on Media Bias in Search Queries and Query Suggestions

## allsides_balanced_news_headlines-texts.csv
The dataset contains 21,747 news articles collected from [AllSides balanced news headline roundups](https://www.allsides.com/headline-roundups) in November 2022. 
The AllSides balanced news feature three expert-selected U.S. news articles from sources of different political views (left, right, center), often featuring spin bias, and slant other forms of non-neutral reporting on political news. All articles are tagged with a bias label by four expert annotators based on the expressed political partisanship, left, right, or neutral. The goal of the AllSides balanced news is to offer multiple political perspectives on important news stories, for educating users on biases, and provide multiple viewpoints. Collected data further includes headlines, dates, news texts, topic tags (e.g., "Republican party", "coronavirus", "federal jobs"), and the publishing news outlet. We also include AllSides' neutral description of the topic of the articles.
Overall, the dataset contains 10,273 articled tagged as left, 7,222 tagged as right and 4,252 articles tagged as center. To provide easier access to the most recent and complete version of the dataset for future research, we provide the scraping tool described earlier in this section.

Data was scraped on 2022-11-15 from [https://www.allsides.com/headline-roundups](https://www.allsides.com/headline-roundups).

## suggestions.csv 
The second dataset we provide consists of 671,669 search query suggestions for root queries based on tags of the AllSides biased news dataset. 
We collected search query suggestions from Google and Bing for the 1,431 topic tags, that have been used for tagging AllSides news at least five times, approximately half of the total amount of topics. 
On average, the dataset contains 469 search queries for each topic.
In total, 318,185 suggestions have been retrieved from Google and 353,484 from Bing.

The file contains a "root_term" column based on the AllSides topic tags. The "query_input" column contains the search term submitted to the search engine ("search_engine"). "query_suggestion"	and "rank" represent the search query suggestions at the respective positions returned by the search engines at the given time of search "datetime". We scraped our data from a US server saved in "location".

