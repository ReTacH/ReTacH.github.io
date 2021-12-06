---
layout: post
title: Reflection Blog
---
In this blog post, we will reflect on the experience of completing the class project: Echo chamber in Social media: [https://github.com/ReTacH/Echo-chamber](https://github.com/ReTacH/Echo-chamber)

### Overall, what did you achieve in your project?

Our project first started from the paper *Political Discourse on Social Media: Echo Chambers, Gatekeepers, and the Price of Bipartisanship (2018)* by Garimella et al. Fortunately, Prof. Garimella provided us with the necessary twitter data that we can work on. Here, we decided to work with a dataset about **Obamacare**, since it looked like we might see a concrete echo chamber from the topic itself (based purely on intuition!).

Using this dataset, we managed to clean and filter the 39 million data (sigh!) to calculate the production polarity and consumption polarity scores by ourselves based on the mathematical formulas which were presented in the paper by Garimella et al. This took us forever since we need to carefully clean the big data using dataframe manipulation and database extraction (with sqlite3). 

Later on, the scores we receive look promising to do some data science analysis; in this sense, we consider some complex visualizations with clustering methods. The result seems incredible; we did see the kind of echo chamber we expected at the start of the project. Lastly, we move our analysis to the network created from the following/follower in Twitter. Combining the two methods, network analysis, and polarity score measurement, yields an interesting result that people tend to follow those with the same kind of political ideology, thus giving rise to the echo chamber in the society, pretty cool!  

In the end, we created an excellent web app to demonstrate our findings of the echo chamber on Twitter (Flora did the CSS things, which is pretty beautiful, I would say). Since echo chamber is probably a technical term that most people don't know, it would be good to present such a concept to the general audience about the biases people face in social media nowadays.

### What are two aspects of your project that you are especially proud of? 

- Obviously, all the visualizations of scores that observed concrete echo chambers (with *plotly* and *gephi*) are just fantastic, nothing more, nothing less. I always enjoy working on a project inspired by a research problem: whenever the results work out from hours of blood, sweat, tears of cleaning the millions of data, it is just pure bliss to me.
- More broadly, I'm proud of the team-working aspects of our team; our strengths and weaknesses complement each other well. This culminates into the web app, which we are content with; the web app is excellent, stylish, and contains a sufficient balance for the general audience and those from the mathematical fields. 

### What are two things you would suggest doing to improve your project further? 

- At the end of the network analysis, we briefly explore the centrality measures in our Twitter network. After we plot the node size based on the eigenvector centrality, we found that people with more conservative ideology tend to have higher eigenvector centrality. It would be interesting for the future project to test this hypothesis and rigorously explore how the eigenvector centrality correlates with the polarity scores. 
- If time permitted, it would be interesting to run the experiments on the *whole* dataset. While the general results may not differ much, it would give better accuracy for the polarity scores and open more research directions on the scalability of the analysis on the Twitter data.

### How does what you achieved compare to what you set out to do in your proposal? 

We manage to complete all **Partial Success** directions and most **Full Success** in the project proposal. In the last couple of weeks, we were trying to analyze each tweet's sentimental analysis to gather the sentimental coefficients to incorporate into the polarity models. However, since this is an unsupervised machine learning problem that is still being researched, we didn't manage to obtain the results. Nevertheless, I feel like we've achieved all the **core** parts of the project direction which we planned at the beginning (around 80% of the whole success), and we feel pretty content with how much work we have done in just a single quarter.

### What are three things you learned from the experience of completing your project? Data analysis techniques? Python packages? Git + GitHub? Etc? 

- I learned to use GitHub effectively in a team-working environment; I've been yearning to master Git + GitHub for a long time!
- I feel like I learned **a lot** about handling large datasets with Pandas and data analysis techniques. Usually, the dataset we obtained from Kaggle or any class projects is organized neatly. In this project, I learned to work with the raw data from scratch, and, more importantly, the data is the real one that has been used extensively for the research paper. I feel like I've gained a lot of adaptability and flexibility in working with messy data more than I could have imagined from other courses. 
- This might not be related to the course materials, but I learned how to tackle large network structures (of millions of edges) using an external program called *gephi*. I've always used *NetworkX* for all the research projects for my undergrad career. I finally realized that *NetworkX* is not a good choice to tackle complex networks, and these skills will surely help me for research projects in the future.

### How will your experience completing this project help you in your future studies or career? Please be as specific as possible. 

This experience would tremendously help me in my future career. I plan to pursue a Ph.D. in applied mathematics in the upcoming year. However, UCLA does not offer many courses on programming for mathematics students in general. Here, I learned to use Python effectively on a project based on a research problem, which helped me gain a lot of experience in formulating a concrete research direction. Also, I enjoy many Python packages covered in this class, such as the geographic visualizations with Plotly, which would help me create a beautiful plot for my research papers. Tensorflow is another popular tool that would help me with many machine learning problems in the future, whether in academic research or industrial projects. All in all, this class offers me many aspects of data science that apply to my future careers, and it is truly a correct choice for me to enroll in this class even though it doesn't satisfy any of my major requirements.