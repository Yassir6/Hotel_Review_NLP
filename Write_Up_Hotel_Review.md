# NLP Hotel Review
## Backstory & scope
For luxury hotels, it is very important to overlook the users feedback about their experience in the hotel and its services to improve and avoid negative 
things and keep the positives. Also, reviews can be analyzed to understand where a hotel failed to provide a good customer experience and where it succeed to do 
so. Therefore, booking.com has provided this great feature which allows customers to write text reviews about their experience in a hotel, to help the hotels and other costumers.

The goal of this project is to build unsupervised Natural Language Processing (NLP) machine learning models that decide whether a text review is positive review or 
negative review. This project, will help hotels to determine the category of text review and cluster them automaticity to improve their services. 
Also the project will build  a recommendation system from the user nationality that will recommend unvisited hotels from in each county and the most similar nationalities based on the reviewer score.
## Data
The data for this project will be read into a CSV file (Find the dataset on the following [link](https://www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe/discussion)). 
This dataset is a scraped data from booking.com contains 515,000 customer reviews (rows)  for 1493 luxury hotels across Europe and it has 17 columns as will. However, 
this data set has been manipulated to contain only two columns: review text , and its category (positive review 1 or negative review 0 ).

Before cleaning the data the positive reviews are 50% as will as the negative reviews, but after clearing the data by dropping the duplicated reviews it become 
44% negative reviews and 56% positive reviews.

## Algorithms
The classification algorithms that has been used in this project on both Counter Vectorization and TF-IDF:
- Logistic Regression
- Bernoulli NB
- Decision Tree

Best Algorithm was Logistic Regression TF-IDF with testing score 0.943 without overfitting.


Topic modeling algorithms that has been used in this project:
- LSA
- NMF
- CorEX

Best Algorithm that made sensible results is CorEX with 3 topics for posative reviews and 4 negative reviews topics.


## Tools
- Pandas library will be used to create data frames.
- NLTK toolkit to perform common NLP tasks.
- Sklearn library will be to implement the classification and clustering models.
- Matplotlib, Seaborn and Wordcloud to visualize and discuss the results of the analysis.
- Autocorrection for Spelling Correction.
- SVD for building recommendation system.


## Communication
The project process and result has presented. To see the presentation slides click [here](https://github.com/Yassir6/Hotel_Review_NLP/blob/main/Hotel_Reviews_NLP_Presentation.pdf).

#
[Project Proposal](README.md)

[Project MVP](MVP_Hotel_Review.md)

[Project Presentation](https://github.com/Yassir6/Hotel_Review_NLP/blob/main/Hotel_Reviews_NLP_Presentation.pdf)

[Project Code](Hotel_Reviews_NLP.ipynb)
