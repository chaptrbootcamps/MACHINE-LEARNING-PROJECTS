# ml_classification_pet-adoption

In this classification problem you will use your knowledge of feature transformation and model tuning to achieve the best prediction metric for the two categorical target variables provided in the dataset. 

**Problem Statement**
A leading pet adoption agency is planning to create a virtual tour experience for their customers showcasing all animals that are available in their shelter. To enable this tour experience, you are required to build a Machine Learning model that determines type and breed of the animal based on its physical attributes and other factors.

[Download the dataset](https://he-s3.s3.ap-southeast-1.amazonaws.com/media/hackathon/hackerearth-machine-learning-challenge-pet-adoption/pet-adoption-9-5838c75b/a01c26dcd27711ea.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=b9073251ef111206aec9fa4be54c94753b17093b091b974f0223dc4231c6fa71&X-Amz-Date=20210831T175517Z&X-Amz-Credential=AKIA6I2ISGOYH7WWS3G5%2F20210831%2Fap-southeast-1%2Fs3%2Faws4_request)


Once you achieved the highest level of accuracy metric, you will be expected to make a submission for evaluation in the folllowing format. 

Data Description:
The data folder consists of 2 CSV files
| col_name |desc |
| -----|-----|
| issue_date	| Date on which the pet was issued to the shelter|
| listing_date	| Date when the pet arrived at the shelter|
| X1 and X2| Anonymous columns|

train.csv - 18834 x 11

test.csv - 8072 x 9

sample_submission:
| pet_id|breed_category|pet_category|
| ------|-----|-----|
ANSL_69903|0|1|
ANSL_66892|0|2|
ANSL_69750|2|4|
ANSL_71623|0|2|
ANSL_57969|0|1|

**Evaluation metri**

s1 = ${f1\_score(actual\_values['pet\_category'],predicted\_values['pet\_category'],average = 'weighted')}$ \\ s2 = { f1\_score(actual\_values['breed\_category'],predicted\_values['breed\_category'],average = 'weighted')}\\ score = 100\times \frac{s1+s2}{2}


