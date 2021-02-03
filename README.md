# News NLP Classification

## Business Problem
With the ease of access to the internet there are now millions of people writing blogs, articles, and stories on many different subjects posted on many different websites. In order for discovery of articles by those who do not intentionally search for an author or article, there must be tags that a person is able to search by to find what they are interested in. This project seeks to solve that problem by using machine learning to predict the category of article based only on the title and a short description.

## The Data
The data in this project is a set of 200,000 news articles that are labeled with their category. The information provided on each article is category, headline, author, link to website, short description, and the data. There are 41 categories that are going to be used as the target for the predictions. There is class imbalance with politics (16%), wellness (9%), and entertainment (8%) having the largest portion of the articles. The smallest categories only having ~1000 articles. This should not be a major problem as there is such a large number of documents.

## Modeling
In the case of this NLP multi-class classification, accuracy is going to the measure I am going to be focusing on. The two models used are random forest and multi-nomial bayes as they are the most common for NLP. Random forest did obtain the highest accuracy of 55% on the test set but was highly overfit due to no stopping criteria in the training phase. Multi-nomial bayes was worse with an accuracy of 40% but was not overfit.

## Conclusions
This project and process shows how TF-IDF and bag of words manipulation can be so powerful for text classification. I believe that if the number of categories was reduced and the information on each article was increased that the accuracy would have been much higher. The title and short description were informative but having the text of the article itself would have been much more powerful for classification.
