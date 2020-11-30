# Group project: Real or Not? NLP with Disaster Tweets
## Data Mining & Machine Learning 2020 - University of Lausanne
## Group Alpina [AIcrowd]

### 🕵️ Project description

Twitter has become a popular social network for many users. However, it is also used to relay fake news.  

The goal of this project is to build a machine learning model that predicts which Tweets are about real disasters and which one’s aren’t.  

To train the model, we have access to a dataset of 6,471 tweets that were already classified (0 = fake news, 1 = real news).  

### 🚀 Progress of the project

#### Week 1

💻 **Github**

- Repo initialisation
- Setting up the repo structure
- Git push ressources: training_set, test_set
- Draft README

💾 **Data**

- Import the inital database into the notebook
- Calculate the base rate on the original dataset
- Distribution of the data in the inital database: 3,701 fake news & 2,770 real news
- Train the model on the original dataset without any modification to set the base benchmark accuracy (basic model)

🧹 **Text preprocessing**

- Size of the database after removing the duplicates: 3,676 fake news & 2,711 real news
- Preproceesing the text to remove irrevelant information
- Run some predictions

#### Week 2

💻 **Github**

- Sych repo 
- README updated

📊 **EDA**

- Plot the Top 10 keywords (entire training set, distinction between fake/real news tweets)
- Plot the Top 10 locations (entire training set, distinction between fake/real news tweets)
- Plot the most used words to improve the text preprocessing

#### Week 3

- EDA completed
- WIP: cleaning the features
- WIP: testing different classifers
- TODO: implement cross validation

### 🥇 Results

- 1<sup>st</sup> submission (basic model): 0.811

### 📹 Video

To be added later 😁
