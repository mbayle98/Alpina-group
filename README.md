## Group project: Real or Not? NLP with Disaster Tweets

![Banner](https://raw.githubusercontent.com/mbayle98/DMML2020-Alpina/main/Documents/Banner_project_alpina.png)


### 🕵️ Project description

Twitter has become a popular social network for many users. However, it is also used to relay fake news.  

The goal of this project is to build a machine learning model that predicts which Tweets are about real disasters and which one’s aren’t.  

To train the model, we have access to a dataset of 6,471 Tweets that were already classified (0 = fake news, 1 = real news). The aim is to use the different techniques seen in class to perform the EDA and the data cleaning in a first step before testing different classifiers to determine which one provides the best accuracy.  

### ⚙️ Models & Parameters

| **Model** | **Parameters**                        | **Accuracy** |
|------------------|----------------------------------------|-------------|
| **Logistic regression:** |                  |   |  
| *X = tweet(1)*           | no hyper, max iter = 100K      | 0,804  |
| *X = tweet(2)*           | c = 3.6,n gram range = (1,3), norm = l1      | **0,823**|
| *X = location*           | c = 1                           | 0,59  |
| *X = lexical categories (all)*           | c = 1  | 1  |
| *X = lexical categories (reduced)*       | c = 2  | 0,676 |
| *X = lexical categories (std)*           | c = 2  | 0,676 |
| *X = lexical categories (std + PCA)*          |   |0,676  |
| *X = keywords*           | c = 1     | 0.59 |
| *combined features:*     |     |  |
| *X = lexical + location*           |     | 0,662 |
| *X = lexical + keyword*            |     | 0,654   |
| *X = location + keyword*           |     | 0,579 |
| *X = all features*                 |     | 0,654 |
| **KNN:**          |                          |   |
| *non optimized*          | X = text           | 0,762 |
| *optimized*          | n gram range (1,3), norm = l2, p =2, weight = distance, n neighboor = 17, leaf_size = 1  | **0,779**  |
| *lexical categories*         | p=1, weight = distance, n neighboor = 19, leaf_size = 1  | 0,728  |
| **Decision tree:**       |                 |   |
| *non optimized*          | n gram range (1,3), norm l2 | 0,755  |
| *optimized*          | max_depth = 71, min_sample_split = 15 | **0,762** |
| **Random forest:**           |                              |  |
| *non optimized*           | n gram range (1,3), norm l2    | 0,792  |
| *optimized*           | criterion = entropy    | **0,793**  |
| *lexical categories*           | bootstrap = true, criterion = gini, 11, n_estimator = 10 | 0,667 |
|

### 🚀 Progress of the project

#### Week 1

💻 **Github**

- Repo initialisation
- Setting up the repo structure
- Ressources uploaded: training_set, test_set
- Draft README

💾 **Data**

- Import the inital database into the notebook
- Calculate the base rate on the original dataset
- Distribution of the data in the inital database: 3,701 fake news & 2,770 real news
- Train the model on the original dataset without any modification to set the base benchmark accuracy (basic model)

🧹 **Text preprocessing**

- Word cloud of the dataset to determine the type of words contained in the Tweets
- Preproceesing the text to remove irrevelant information 
- Run an elementar model

#### Week 2

📊 **EDA**

- Plot the Top 50 keywords (entire training set, distinction between fake/real news Tweets)
- Plot the Top 50 locations (entire training set, distinction between fake/real news Tweets)
- Plot the most common words and word types in Tweets

#### Week 3

📊 **EDA** + ⚙️ **Optimization**

- EDA completed
- Cleaning the features in progress
- Testing different classifers
- Cross validation to be done

#### Week 4

⚙️ **Optimization**

- Different classifiers tested: Logistic regression, kNNeighbours, Decision Tree, Random Forest
- Hyper-parameter optimization with GridSearch

### 🥇 Results

10 subsmissions on AIcrowd:
- 1<sup>st</sup> submission (basic model): 0.57
- 2<sup>nd</sup> submission (Logistic regression model): 0.811
- 3<sup>rd</sup> submission (Logistic regression optimized model): 0.816
- 4<sup>th</sup> submission (Logistic regression optimized numbers removal model): 0.818




![Graphic AIcrowd](Documents/AICROWD.PNG)

### 📹 Video

To be added later 😁
