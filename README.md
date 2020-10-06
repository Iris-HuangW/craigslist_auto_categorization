# Craigslist Auto Categorization
This project is a demo version of craigslist auto-categorization feature for "General" ad posts in Chicago based on the NLP models trained with ad posts of "For Sale" category in Chicago region

#### -- Project Status: Completed

## Project Intro/Objective
The objective of the project is to deploy NLP approches including text mining and image recognition for auto categorization features to improve the ad-viewers’ experience and help platform managers to easily manage the platform, without changing the experience of advertisers. 

### Craigslist
* Craigslist is an American classified advertisements website with sections devoted to jobs, housing, for sale, items wanted, services, community, gigs, résumés, and discussion forums. It is one of the largest peer-to-peer user-generated advertisements website serving 570 cities in 70 countries.
* The website is advertiser-oriented. Advertisers can easily publish advertisements in a flexible and unstructured format, typically shown as text description and/or uploaded images. However, this incurs a high cost for ad-viewers to extract relevant information. In addition, the unstructured data brings a high cost for platform managers to maintain and organize the website.
* https://chicago.craigslist.org/

### Methods Used
* Natural Language Processing(NLP)
* Machine Learning
* Predictive Modeling
* Text Mining 
* Image Recognition
* Web Crawling
* Data Visualization

### Technologies
* Python
* Scrapy
* Pandas, Numpy, Seaborn
* Scikit-learn, Keras, Natural Language Toolkit(NLTK), 
* Convolution Neural Net(CNN) architectures (VGG16, VGG19)

## Project Description
Craigslist users are not able to identify categories of ad posts under "General" category, which are in the flexible and unstructured format. This problem led to reduced views and lower user satisfaction. In order to resolve this problem and improve user experience and product engineering of craigslist, we proposed to develop an automatic categorization feature by deploying NLP approches.
In this project, we first collected data from categorized posts, then we build predictive/NLP model on collected text and image data. Eventually, we used the model to implement auto-categorization function.

## Getting Started

1. Scraped ad posts data from "For Sale" in Chicago using Scrapy framework in Python [craigslist_auto_categorization/spiders/data.py] (Repo folder containing data processing scripts/notebooks)
- Multiple pages, nested layer pages
- 40+ Categories
- 81,000+ posts till 12/3/2019, 21,000+ extracted sample data
- 3 features: Category, Title, Description

2. Data processing/transformation
* Text mining[Text_Analysis.py]
- token, lemmatize, remove stop words
- text mining processing: take out general category and partition 
- text mining processing: term-document matrix

3. Model Training
* Text mining[Text_Analysis.py]
* Image recognition using pretrained VGG16, VGG19 models [Unstructured_Final_Project_Image_Classification.py]
* https://www.tensorflow.org/api_docs/python/tf/keras/applications/VGG16
* https://www.tensorflow.org/api_docs/python/tf/keras/applications/VGG19

4. Tested on ad posts in "General" category


## Contact
* Feel free to contact with any questions or if you are interested in contributing!
