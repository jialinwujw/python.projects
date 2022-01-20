# About The Analysis
Utilize Natural Language Processing (NLP) to analyze text data derived from a variety of sources, including social media, customer service live chats, emails, product reviews and surveys, for example.

## Project

### Data
https://www.kaggle.com/zynicide/wine-reviews

### Discription
This dataset consists of wine reviews, including information about their variety, location, winery, price, and description. Using a natural language processing algorithm, we will conduct an analysis of the description text to gain a deeper understanding of what tasters think about a particular wine.

### Python Packages
* pandas
* numpy
* matplotlib
* seaborn
* re
* nltk
* textblob
* gensim
* sklearn
* wordcloud

### Outputs
A process of **NMF topic modeling** is employed to uncover latent topical patterns. This application generates word distributions from a corpus of documents. Based on the results, it can determine whether there are any distinct themes present within the text.
<br><br>
A **word cloud** illustrates words and phrases that are used more frequently. By providing a graphic representation of the text data, simple insight can be gained quickly and easily, which can then be used for further analysis.
<br><br>
By using **POS tagging**, words are characterized based on their parts of speech and then labeled accordingly. Consequently, we can gain a deeper understanding of the most commonly used words, breaking them down into nouns, adjectives, verbs, etc. These results are more thorough than a word cloud.
<br><br>
In **Sentiment Analysis**, we attempt to determine whether a given piece of text reflects positive, negative, or neutral sentiment. This technology enables companies to interpret feedback from customers, understand their needs, and develop better products. The two most popular methods and packages - *VADER* and *Textblob* - are used to do sentiment analysis.
