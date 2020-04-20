--Run jupyter notebook file from top to bottom will get most of data in the report.

--If want to test other datasets.
Change dataset need these steps:
1. Edit id_column if there is id column in dataset.
2. Edit missing_values to datasets' missing value.
3. Change first input of preprocess function to the dataframe you want.
4. Change Global variables
	1. Change datasets_type(datasets_types can be 
    				NOMINAL: NOMINAL ATTRIBUTES DATASETS, 
    				UMERIC: NUMERIC ATTRIBUTES DATASETS, 
    				ORDINAL: ORDINAL ATTRIBUTES DATASETS, 
    				MIX: DATASETS WITH A MIX OF ATTRIBUTE TYPES)
	2. If it's MIX dataset change feature_types list
	3. Change feature_types as the column of class feature for example the 15th row 
	   of adult is class feature _types should be 14

Example: for bank dataset ()

bank = pd.read_csv("datasets/bank.data", header = None)
id_column = None
missing_values = None
train_data = preprocess(bank, missing_values, id_column)
datasets_types = "MIX"
feature_types = [2, 0, 0, 1, 0, 2, 0, 0, 0, 2, 2, 2, 2, 0]
class_column = 14

Nothing else should change


--While useing calc_outcome(train_data, test_data = None, interesting_class = None): function to evaluate model.

train_data is training set

test_data is test set (default testing set is the same as training set)

interesting_class is optional (input which class is interesting class) for interesting class this function will calculate it's recall and precision