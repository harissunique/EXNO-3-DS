## EXNO-3-DS

# AIM:
To read the given data and perform Feature Encoding and Transformation process and save the data to a file.

# ALGORITHM:
STEP 1:Read the given Data.
STEP 2:Clean the Data Set using Data Cleaning Process.
STEP 3:Apply Feature Encoding for the feature in the data set.
STEP 4:Apply Feature Transformation for the feature in the data set.
STEP 5:Save the data to the file.

# FEATURE ENCODING:
1. Ordinal Encoding
An ordinal encoding involves mapping each unique label to an integer value. This type of encoding is really only appropriate if there is a known relationship between the categories. This relationship does exist for some of the variables in our dataset, and ideally, this should be harnessed when preparing the data.
2. Label Encoding
Label encoding is a simple and straight forward approach. This converts each value in a categorical column into a numerical value. Each value in a categorical column is called Label.
3. Binary Encoding
Binary encoding converts a category into binary digits. Each binary digit creates one feature column. If there are n unique categories, then binary encoding results in the only log(base 2)ⁿ features.
4. One Hot Encoding
We use this categorical data encoding technique when the features are nominal(do not have any order). In one hot encoding, for each level of a categorical feature, we create a new variable. Each category is mapped with a binary variable containing either 0 or 1. Here, 0 represents the absence, and 1 represents the presence of that category.

# Methods Used for Data Transformation:
  # 1. FUNCTION TRANSFORMATION
• Log Transformation
• Reciprocal Transformation
• Square Root Transformation
• Square Transformation
  # 2. POWER TRANSFORMATION
• Boxcox method
• Yeojohnson method

# CODING AND OUTPUT:
```py
import pandas as pd
df=pd.read_csv("Encoding Data.csv")
df
```
![alt text](<Screenshot 2024-09-27 161706.png>)
```py
from sklearn.preprocessing import LabelEncoder,OrdinalEncoder
pm=['Hot','Warm','Cold']
e1=OrdinalEncoder(categories=[pm])
e1.fit_transform(df[["ord_2"]])
```
![alt text](<Screenshot 2024-09-27 161711.png>)
![alt text](<Screenshot 2024-09-27 161722.png>) ![alt text](<Screenshot 2024-09-27 161728.png>) ![alt text](<Screenshot 2024-09-27 161740.png>) ![alt text](<Screenshot 2024-09-27 161748.png>) ![alt text](<Screenshot 2024-09-27 161755.png>) ![alt text](<Screenshot 2024-09-27 161800.png>) ![alt text](<Screenshot 2024-09-27 161807.png>)![alt text](<Screenshot 2024-09-27 161933.png>) ![alt text](<Screenshot 2024-09-27 161813.png>) ![alt text](<Screenshot 2024-09-27 161828.png>) ![alt text](<Screenshot 2024-09-27 161834.png>) ![alt text](<Screenshot 2024-09-27 161859.png>) ![alt text](<Screenshot 2024-09-27 161905.png>) ![alt text](<Screenshot 2024-09-27 161910.png>) ![alt text](<Screenshot 2024-09-27 161922.png>) ![alt text](<Screenshot 2024-09-27 161927.png>)![alt text](<Screenshot 2024-09-27 161941.png>) ![alt text](<Screenshot 2024-09-27 161946.png>) ![alt text](<Screenshot 2024-09-27 161952.png>) ![alt text](<Screenshot 2024-09-27 162006.png>) ![alt text](<Screenshot 2024-09-27 162044.png>)


# RESULT:
       Finally, perform Feature Encoding and Transformation process is executed successfully.
       
