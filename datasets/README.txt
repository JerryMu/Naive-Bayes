These datasets were downloaded from the UCI Machine Learning Repository
https://archive.ics.uci.edu/ml/index.php

Some datasets have been reformatted to make them easier to read.

Each dataset consists of a pair of files: the .data file contains the data and the .names file provides extra information about the dataset. The .data files are comma-separated value files with no headers. The nominal attributes (include the class labels) may be either numbers or strings/chars. A summary of each dataset is provided below.

---------------------------------------

NOMINAL ATTRIBUTES DATASETS

breast-cancer-wisconsin
  Instances: 699
  Attributes: 9 (the first column is an ID code which should not be used as an attribute)
  Task: predict diagnosis (2=benign, 4=malignant) 
  Class: last column (11)
  Missing values: marked as ?

mushroom
  Instances: 8124
  Attributes: 22
  Task: predict poisonous (p) or edible (e)
  Class: first column
  Missing values: marked as ?

lymphography
  Instances: 148
  Attributes: 18
  Task: predict diagnosis (normal find, metastases, malign lymph, fibrosis)
  Class: first column
  Missing values: none

---------------------------------------

NUMERIC ATTRIBUTES DATASETS

wdbc
  Instances: 569
  Attributes: 30 (the first column is an ID code which should not be used as an attribute)
  Task: predict diagnosis (M=malignant, B=benign)
  Class: second column
  Missing values: none

wine
  Instances: 178
  Attributes: 13
  Task: predict wine cultivar (1, 2, 3)
  Class: first column
  Missing values: none

---------------------------------------

ORDINAL ATTRIBUTES DATASETS

car
  Instances: 1728
  Attributes: 6
  Task: predict car quality (unacc, acc, good, v-good)
  Class: last column (7)
  Missing values: none

nursery
  Instances: 12960
  Attributes: 8
  Task: predict nursery recommendation (not_recom, recommend, very_recom, priority, spec_prior)
  Class: last column (9)
  Missing values: none

somerville
  Instances: 143
  Attributes: 6
  Task: predict happy (1) or unhappy (0)
  Class: first column
  Missing values: none

---------------------------------------

DATASETS WITH A MIX OF ATTRIBUTE TYPES

adult
  Instances: 32561
  Attributes: 14
  Task: predict income (<=50K or >50K)
  Class: last column (15)
  Missing values: marked as ?
  Attribute types (0=nominal, 1=ordinal, 2=numeric):
    [2, 0, 2, 1, 1, 0, 0, 0, 0, 0, 2, 2, 2, 0]

bank
  Instances: 45211
  Attributes: 14
  Task: predict purchase (yes, no)
  Class: last column (15)
  Missing values: none
  Attribute types (0=nominal, 1=ordinal, 2=numeric):
    [2, 0, 0, 1, 0, 2, 0, 0, 0, 2, 2, 2, 2, 0]

university 
  Instances: 231
  Attributes: 16 including class* (the first column is an ID code which should not be used as an attribute)
  Task: predict academic score*
  Class: column 14*
*this dataset doesn't have a defined task, so you could predict any of the nominal/ordinal variables (e.g., social score (col 15) or expenses (col 9))
  Missing values: marked as 0
  Attribute types (0=nominal, 1=ordinal, 2=numeric), including the "class" attribute:
    [0, 0, 1, 2, 2, 2, 2, 1, 2, 1, 2, 2, 1, 1, 1, 0]