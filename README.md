# Practical-Data-Science-As2

Marks: 35/35

# Abstract:

The aim of this report is to determine whether a person earns over $50k using classification
methods based on 1994 United States Census Data which is also commonly known as the
“Adult” dataset. To do so, we started off with sanitising the data, generating visualisations to
look for relationships between attributes, then performing data modelling was performed with
K-nearest Neighbour Classifier and Decision Tree Classifier using ​scikit-learn library. Finally,
feature selection was performed to help answering the research question. As a result, it has
been proven that for dealing with data modelling, Decision Tree Classifier is the better
choice for this particular dataset as it produces a higher accuracy score and a lower error
rate than using K-nearest Neighbour Classifier. Therefore, it is recommended that Decision
Tree Classifier should be used when performing classification with the “Adult” dataset.

# Dataset:
https://archive.ics.uci.edu/ml/datasets/Adult

# Introduction:

The “1994 United States Census Income” dataset, also known as the “Adult” dataset contains 14
attributes including one class attribute and 32561 instances. Thanks to its donors, Ronny and Barry
who both graciously donated the dataset in 1996, it has been one of the most popular datasets that is
used for predicting whether a person’s income exceeds US$50k per year based on the census data
collected in 1994 in the United States of America ​[1]​. It has been chosen due to its high success rate
to perform data modelling with classification methods as recommended by the UCI Machine learning
Repository website ​[1]​. The aim of the report is to explore the dataset using visualisations, model the
given data using classification methods with K-nearest Neighbour Classifier and Decision Tree
Classifier, analyse the performance of each classifier and provide recommendation for which classifier
should be used.

Attributes of the dataset are as follow​:

- age​: an individual’s age. Continuous. Min: 17, Max: 90

- workclass​: an individual’s employment status. Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay,
Never-worked.

- fnlwgt​: final weight, the sampling weight of each entry. Continuous. Min: 12285​, Max: 1484705

- education​: an individual’s highest level of education achieved. Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.

- education-num: an individual’s highest level of education achieved represented in numerical values. Ordinal numbers: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16

- marital-status​ : an individual’s marital status. Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.

- occupation​: an individual’s occupation field. Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty,
Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.

- relationship​: a representation of what the individual is relative to others. Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.

- race​: an individual’s race. White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.

- sex​: an individual’s sex. Female, Male.

- capital-gain​: an individual’s capital gain. Continuous. Min: 0, Max: 99999

- capital-loss​: an individual’s capital loss. Continuous. Min: 0, Max: ​4356

- hours-per-week​: an individual’s working hours per week. Continuous. Min: 1, Max: 99

- native-country​: an individual’s native country. United-States, Cambodia, England, Puerto-Rico, Canada, Germany,
Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras,
Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France,
Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala,
Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong,
Holand-Netherlands.

- income​: ​label/target​ for if an individual makes over $50k or under. >50K, <=50K.


The dataset contains missing values and errors as stated on the UCI Machine Learning Repository
website, which was handled appropriately and will be discussed in the next section of the report.
