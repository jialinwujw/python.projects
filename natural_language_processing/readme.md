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

```sh
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns

import re # https://www.w3schools.com/python/python_regex.asp

import nltk
# NLTK was not fully installed by pip, so many components were absent, resulting in some features not working. 
# By running ntlk.download(), a new window will open. From there, you can choose which additional packages to install.
nltk.download()
from nltk.corpus import stopwords
from nltk.corpus import wordnet as wn
from nltk.tokenize import word_tokenize
from nltk.sentiment.vader import SentimentIntensityAnalyzer
from nltk.stem.wordnet import WordNetLemmatizer

from textblob import TextBlob
from textblob import Word

import gensim
import gensim.corpora as corpora

from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.decomposition import NMF

from wordcloud import WordCloud, STOPWORDS, ImageColorGenerator

import warnings
warnings.filterwarnings('ignore') # Never print matching warnings
```

### Outputs
A process of **NMF topic modeling** is employed to uncover latent topical patterns. This application generates word distributions from a corpus of documents. Based on the results, it can determine whether there are any distinct themes present within the text.
<br><br>
A **word cloud** illustrates words and phrases that are used more frequently. By providing a graphic representation of the text data, simple insight can be gained quickly and easily, which can then be used for further analysis.
<br><br>
By using **POS tagging**, words are characterized based on their parts of speech and then labeled accordingly. Consequently, we can gain a deeper understanding of the most commonly used words, breaking them down into nouns, adjectives, verbs, etc. These results are more thorough than a word cloud.
<br><br>
In **Sentiment Analysis**, we attempt to determine whether a given piece of text reflects positive, negative, or neutral sentiment. This technology enables companies to interpret feedback from customers, understand their needs, and develop better products. The two most popular methods and packages - *VADER* and *Textblob* - are used to do sentiment analysis.
