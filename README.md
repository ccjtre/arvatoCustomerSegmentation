# arvatoCustomerSegmentation
# libraries used:
numpy
pandas
matplotlib.pyplot
seaborn
sklearn.preprocessing
sklearn.decomposition
time
sklearn.metrics
sklearn.naive_bayes
sklearn.ensemble
sklearn.svm
sklearn.grid_search
sklearn.metrics

# motivation

apply unsupervised machine learning techniques to general and known-customer demographic data sets to build a profile of the core customer base of a mail order sales company.
The problem statement is thus: Given that we can obtain a topography of the underlying demographic clusters of a general population, how can we map a know customer population to this topography and in turn derive its relevant demographic characteristics to create high-precision mail order marketing strategy?
Our success criteria in this respect will be two fold. First, we must be able to build practical interpretations of our demographic clusters to identify the core customer base. That is, translating mathematical data into the financial, familial, and social characteristics of the underlying groups. Secondly, our resulting customer prediction model must have a high precision rate. That is, of the people it identifies as potential customers, a high proportion do actually fit within the demographics of our core customer base.
Four data files are associated with this project (not included):
Udacity_AZDIAS_052018.csv: Demographics data for the general population of Germany; 891 211 persons (rows) x 366 features (columns).
Udacity_CUSTOMERS_052018.csv: Demographics data for customers of a mail-order company; 191 652 persons (rows) x 369 features (columns).
Udacity_MAILOUT_052018_TRAIN.csv: Demographics data for individuals who were targets of a marketing campaign; 42 982 persons (rows) x 367 (columns).
Udacity_MAILOUT_052018_TEST.csv: Demographics data for individuals who were targets of a marketing campaign; 42 833 persons (rows) x 366 (columns).

Each row of the demographics files represents a single person, but also includes information outside of individuals, including household, building, and neighborhood characteristics.
Alongside the demographics we also used two data dictionaries: 'DIAS Information Levels - Attributes', containing descriptive and hierarchical information for many attributes in the data set, and 'DIAS Attributes - Values', which maps the value domain of many of the attributes to their corresponding meanings, and also provides attribute-level descriptions.

# files

- Arvato Project Final Workbook.ipynb - notebook containing data exploration, pre-processing, unsupervised and supervised learning pipelines

# summary

Our success criteria in this respect were two fold. First, we wanted to build practical interpretations of our demographic clusters to identify the core customer base. Secondly, our resulting customer prediction model needed to have a high precision rate. 
In the first respect we had a modest success: we successfully mapped the general demographics data to four clusters and in turn mapped the customer base onto this topography. By visualizing over-represented clusters in the customer base relative to the general population, and marrying these clusters to our principal component interpretations, we were able to build a profile of a likely core customer base.
Our efforts with the prediction model were less successful, lessons learned being to utilize the knowledge gained from clustering to a greater degree and also to further refine our models using grid search.

# acknowledgements

- plotting functions inspired by udacitys unsupervised learning content
- SVM theory: https://course.ccs.neu.edu/cs5100f11/resources/jakkula.pdf
- AdaBoost theory: https://www.matec-conferences.org/articles/matecconf/pdf/2017/53/matecconf_icmite2017_00222.pdf
