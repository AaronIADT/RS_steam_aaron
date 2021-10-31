***Creative Computing - Artificial Intelligence - Aaron Lynch***

**Assignment 1:**

**Introduction:**

It is my goal for this project to create a write up that details and investigates the various applications of AI in our world and specifically the use of recommender systems in our software. I also aim to be able to create a useful recommender system based off of a set of data of my choice. I will achieve this by following multiple online tutorials to educate myself in the different approaches to creating a recommender system and then using the skills I learn doing this to create my own system. With recommender systems being the main focus I will specifically look at two different approaches to creating them, a Content-Based Approach and a Collaborative Approach, I will delve further into what these entail in a later section of my write-up.

**Applications of AI:**

&quot;AI&quot;- an abbreviation for Artificial Intelligence - is exactly that; an intelligence displayed by a computer or machine to mimic certain human-like abilities such as; problem-solving, learning, memory, communication, decision-making.

 AI enables technological systems to be perceptive of their environment, make decisions based on what they perceive, problem-solve and act to achieve specific pre-programmed goals.
 AI is not only more efficient, effective and cost-reductive than human labor; it is programmed to achieve specific goals - as well as being capable of adapting its learned behavior to better achieve these set goals by analysing the effects of previous actions and working autonomously. There have been huge technological advancements in recent years which have led to major breakthroughs in AI - due to the increase in computational power, newer algorithms and the ever-expanding availability of huge quantities of data.

 In recent years Artificial intelligence is something that is commonly used in almost every aspect of daily human life. Whether we are trying to send emails, read subtitles, listen to music on the way to work, drive to college or withdraw funds from our bank account; AI is present.

**Strengths/Limitations:**

**Strengths of AI:**

 From robotics to healthcare AI is an integral part of shaping the identity of the world we see today. It has applications in almost every part of human life – online shopping, advertising, web searching, digital assistants, language translation, smart infrastructure, cars, cybersecurity; it is also paramount in aiding the fight against Covid-19 currently with thermal imaging technology now present in airports and elsewhere. With regards to medicine, it can help us recognise infection through computerised lung scans, as well as observe infection rates and provide data to track the spread of the disease.

**Limitations of AI:**

Though AI is hugely beneficial in everyday human life, it does have limitations;
 For prediction or decision models to be programmed – we need data.
 Data is seen nowadays as one of the most expensive commodities (even more so than oil). A lot of the data currently sits in the hands of large corporate organisations, which in turn puts small businesses at a disadvantage.
 There are also some hardware limitations I.e limited computation resources of which can make AI more costly – again large corporate organisations have an advantage here too as these resources are more readily available for them. &quot;Mining, storing and analysing data will be very costly in terms of energy and hardware use&quot;. (shishir, 2020)
 There is also a huge bias which can happen when designing AI algorithms; as AI is designed solely for the purpose of performance and achieving goals - concepts such as prejudiced data and social context are not tested or considered.
 Errors can happen within AI systems; AI is not meant to adapt to deviations in human circumstances I.e buying the wrong product because the photograph attached was inaccurate (and has yet to be amended or addressed by the seller). Although this may not be a massive issue, bigger errors could occur which could result in a breach of security or human safety.

**Recommender Systems:**

With the continued rise and dominance of web services such as Youtube, Netflix, Amazon and other social media platforms, so too have we seen an increase in the use and importance for recommender systems in our lives. The most common uses we see recommender systems in would be playlist generators for video and music streaming sites, recommending products in e-commerce sites or recommenders for articles and content for social media. We also see use of recommender systems in the advertisements that we see throughout the internet. All these recommender systems work on large collections of data that allows the system to accurately perform its purpose.

The Importance of recommender systems has grown vastly in the past few years as it has been proven that a good recommender system can greatly increase income and activity for a platform. For most companies large amounts of their budget is spent on improving the algorithms for these systems year after year. _&quot;Netflix organised a challenge (the &quot;Netflix prize&quot;) where the goal was to produce a recommender system that performs better than its own algorithm with a prize of 1 million dollars to win.&quot; (Baptiste Rocca, 2019)_

When we look at recommender systems we can generally see that they make use of either or both a collaborative approach and a content-based approach. The main difference between these is that a collaborative approach builds its model of a users past behaviors whereas a content-based approach works more off the data of a given object to then use that data to suggest other items to you that share similar characteristics. You can see how in many systems a combination of both methods is probably most effective.

**Content-Based Approach:**

A content-based approach to a recommender system is based on a mix of the description of the item in question and the user&#39;s personal preferences. This method is best suited when we know a lot of data about the item such as its name, description, age etc. but we do not possess much information about the user. Items are described by keywords and then a user profile is built in the system to help indicate what types of items that user might like based on their interest and the correlating item keywords. Often many different algorithms are used in the calculation of an item&#39;s features and the relevance of those features. An example of one of these would be the tf-idf algorithm, this system creates a content-based profile of users and bases it on a weighted vector of item features. This weighting helps us to determine how important to the user the different features of an item would be. The main issue with a content-based approach to recommender systems is that the system must learn its user preference from user&#39;s actions regarding one item and then use this across other item types. In some cases this could keep the recommendations very stale as they would all be related. The main advantage to a content-based approach is that it is very cold start friendly, not requiring the same level of background information on the user.

**Collaborative Approach:**

Collaborative filtering relies heavily on the idea that people who agreed in the past will agree in the future, this simple concept allows the system to assume that given shared interest between users you can infer that they will like similar kinds of items. One of the great advantages of a collaborative approach is that the system does not rely on any machine analysable content, this makes it so that the system is capable of recommending complex items without actually having and understanding of what the item itself is. In general collaborative filtering algorithm can be split into two sub-categories, memory based and model based. With a memory based approach the systems uses recorded interactions with assuming no model and are based on nearest neighbours (e.g closest user to another user and suggest most popular items from both of these users). A model based approach instead assumes an underlying generative model that looks at and explains user-item interaction in order to make new predictions.

Collaborative approaches often run into three main problems. On a cold start there is just not enough user/item data to make accurate recommendations. In large systems this approach can struggle with scalability given the large amount of computations to make in a big system with a lot of users. Finally sparsity of data, in most large systems users will only have rated a small amount of your database overall leaving you short on data in many cases.

**Steam Library Recommender:**

The recommender system that i have designed is a system that holds a database of the vast majority of steams current library of games and when given the exact name of a game in steam&#39;s library or this games ID, the system will then search its database and provide a recommendations of ten similar games that the user may like based of the game they provided the system with.

**Description:**

The database that the system pulls from is a .csv file that contains over 27000 entries of different video game titles available on steam currently. The idea was to create a system that is not only recommending games of a similar name but to also take into account other factors such as maybe the genre that the game belongs to. The various data sections in my file where &#39;appid&#39;, &#39;name&#39;, &#39;release\_date&#39;, &#39;english&#39;, &#39;developer&#39;, &#39;publisher&#39;, &#39;platforms&#39;, &#39;required\_age&#39;, &#39;categories&#39;, &#39;genres&#39;, &#39;steamspy\_tags&#39;, &#39;achievements&#39;, &#39;positive\_ratings&#39;, &#39;negative\_ratings&#39;, &#39;average\_playtime&#39;, &#39;median\_playtime&#39;, &#39;owners&#39;, &#39;price&#39;. Some of these categories are not used in my example but could be used in the future to further refine your recommendation, this would especially work if we had a user profile built up to also aid in suggesting titles.

**Implementation (refer to research):**

To implement my recommender system i created it in jupyter notebook, in my very first attempt at creating my system i started with a much smaller dataset of the top 50 songs on spotify so as not to confuse myself with complex data, to build my first system i followed a tutorial that used the nearest neighbor method to determine its recommendations. While this worked fine for comparing rankings, durations etc, it was not capable of performing the same comparisons with Strings of text and only worked with numbers. This would not work for the final system I wanted to create so ultimately I went in search of a new method. Following this I followed some tutorials that approached the system using count vectorising and the cosine similarity in order to determine what was the closest and most accurate recommendation. In order to create diverse and accurate comparisons I first created a new column in my database that combined the name, game developer and the games genre all into one column.

![](RackMultipart20211031-4-u4jqln_html_e45b6f3ddb0091e.png)

This then allowed me to perform all my comparisons based off this column meaning my recommendations came out more accurate as the system is taking multiple factors into account when recommending you games. The system was able to upon being given a game name or id from the system, create a list of tuples that holds the game id and a percentage of how closely the 3 main categories match.

![](RackMultipart20211031-4-u4jqln_html_600327e3e20c92f4.png)

From here the list is sorted by similarity and then the top ten from this list is taken and printed excluding the top result which is removed as it will always be most similar to itself.

![](RackMultipart20211031-4-u4jqln_html_d50552f57aba3d63.png)

**References:**

_27 Examples of Artificial Intelligence Shaking Up Business as Usual_. (2021). Built In. [https://builtin.com/artificial-intelligence/examples-ai-in-industry](https://builtin.com/artificial-intelligence/examples-ai-in-industry)

Baptiste Rocca. (2019, June 2). _Introduction to recommender systems - Towards Data Science_. Medium; Towards Data Science. [https://towardsdatascience.com/introduction-to-recommender-systems-6c66cf15ada](https://towardsdatascience.com/introduction-to-recommender-systems-6c66cf15ada)

_CSDL | IEEE Computer Society_. (2021). Computer.org. [https://www.computer.org/csdl/magazine/co/1986/07/01663273/13rRUyg2jQJ](https://www.computer.org/csdl/magazine/co/1986/07/01663273/13rRUyg2jQJ)

#### _(2021). Retrieved 31 October 2021_, from

[https://test.globalinfocloud.com/technodigisoftnew/wp-content/uploads/2019/07/Applications-of-Artificial-Intelligence-Associated-Technologies.pdf](https://test.globalinfocloud.com/technodigisoftnew/wp-content/uploads/2019/07/Applications-of-Artificial-Intelligence-Associated-Technologies.pdf)

_Recommender Systems_. (2011). Google Books. https://books.google.ie/books?hl=en&amp;lr=&amp;id=eygTJBd\_U2cC&amp;oi=fnd&amp;pg=PR5&amp;dq=recommender+systems&amp;ots=mWw2a6CTvD&amp;sig=sIkn1ydqqxEUpYIUbcOhtGulXcQ&amp;redir\_esc=y#v=onepage&amp;q=recommender%20systems&amp;f=false

‌

‌
