# OnlineGameAnxiety
Analysis and simple model built on Online Game Anxiety Dataset on kaggle.com

Link: https://www.kaggle.com/datasets/divyansh22/online-gaming-anxiety-data?resource=download

Survey information: https://osf.io/vyr5f

Personal Insights about the Dataset:

In general, it is a very good dataset to work on, but firstly it is cruical to check the survey first, analyze it, and understand why this dataset was initially created and how.
The most problematic part with this dataset was the missing values, especially since the whole column was filled with NaN, so I just dropped it. Seems like this question in the survey was very unnecessary, or maybe the dataset was corrupted. With other features, there were no such huge problems.
Another annoying part was the presence of the 'Other' field in the survey, so they were a lot of unique answers in the categorical type of columns, so I needed to manage these too.
With missing data, I mostly used mean in numerical ones and mode in categorical ones, or if the size was less than 100, then I just dropped the rows with NaN (the dataset is large enough to allow this decision).
I used MinMaxScaler for numerical data, and LabelEncoder for categorical data. These are pretty common and efficient in use with small-average datasets.
