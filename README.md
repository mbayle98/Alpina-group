## Group project: Real or Not? NLP with Disaster Tweets

![Banner](https://raw.githubusercontent.com/mbayle98/DMML2020-Alpina/main/Documents/Banner_project_alpina.png)


### 🕵️ Project description

Twitter has become a popular social network for many users. However, it is also used to relay fake news.  

The goal of this project is to build a machine learning model that predicts which Tweets are about real disasters and which one’s aren’t.  

To train the model, we have access to a dataset of 6,471 Tweets that were already classified (0 = fake news, 1 = real news). The aim is to use the different techniques seen in class to perform the EDA and the data cleaning in a first step before testing different classifiers to determine which one provides the best accuracy.  

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

💻 **Github**

- Sych repo 
- README updated

📊 **EDA**

- Plot the Top 50 keywords (entire training set, distinction between fake/real news Tweets)
- Plot the Top 50 locations (entire training set, distinction between fake/real news Tweets)
- Plot the most common words and word types in Tweets

#### Week 3

- EDA completed
- WIP: cleaning the features
- WIP: testing different classifers
- TODO: cross validation

#### Week 4

- Different classifiers tested: Logistic regression, kNNeighbours, Decision Tree, Random Forest
- Hyper-parameter optimization with GridSearch

### 🥇 Results

- 1<sup>st</sup> submission (basic model): 0.811
- To complete

### 📹 Video

To be added later 😁
