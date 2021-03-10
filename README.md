# NYC-Crashes

- Data preprocessing - NYC Motor Vehicle Crashes
- Repository: nyc-crashes
- Type of Challenge: Consolidation
- Duration: 2 days
- Deadline: 10/03/2021 05:00 PM
- Team challenge : solo

## Mission objectives

Be able to use pandas
Be able to clean a data set
Be able to do prepare a data set for a machine learning model

## The Mission
Bill de Blasio, mayor of New York City, is in a bit of a pickle. Indeed, his police department, the NYPD, collected information about all the traffic accidents that happened in New York City. However, they are too busy eating doughnuts to correctly encode each traffic indicent, and so it happens that the dataset that we got here is quite dirty, has a lot of missing values and can't be used by a machine learning model as is. Can you help Mr. de Blasio and shine a new light on his police department? What he wants exactly is to predict which streets are the most dangerous while visiting the city that never sleeps.


## Must-have features

- The dataset contains no missing values ("" or null)
- No duplicates
- Values are consolidated
- Data format is correct
- No blank spaces (ex: " I love python " => "I love python")

## Nice-to-have features

The more rows of data you use, the better. However, pay attention that the more data you have, the longer each operation needs to execute.
Add new features computed using the features present that you think are going to be useful.
Apply the preprocessing steps needed so that a future machine learning model can make the best use out of it (feature selection, feature engineering, feature normalization, and resampling)

## The Repository

In this repository there are different versions of cleaned data from the same origin .csv file:
1. Clean_Data_BAD
2. Clean_Data_GOOD_ENOUGH

Each of these contain a .ipynb file containing the cleaning process and a .csv file with the results of this cleaning process.

#### Description of the different versions

1. Clean_Data_BAD

In this version of the cleaned data, the main focus is on the "on_street_name", if this value is not present in a row in the dataframe, it will have been removed. The rest of the file is than processed as described in the .ipynb file. The results can be checked in the .csv file and contains 73,991 rows of data.

2. Clean_Data_GOOD_ENOUGH

In this version of the cleaned data, the main focus is also on the "on_street_name", but missing values which are present in the cross_street_name column are added. if there are still a missing value in a row, in the on_street_name column in the dataframe, it will have been removed. The rest of the file is than processed as described in the .ipynb file. The results can be checked in the .csv file and contains 99,958 rows of data.
