# Twitter Influence Analysis using Graph Theory

## 📌 Overview
This project analyzes Twitter user influence using graph theory techniques. The analysis involves two primary graphs:
1. **Tweet-Word Bipartite Graph:** Represents the relationship between tweets and words.
2. **User-Following Graph:** Represents the network of Twitter users and their follow relationships.

Additionally, we apply **HITS (Hyperlink-Induced Topic Search) Algorithm** and **PageRank Algorithm** to determine the importance of tweets and users in the network.

## 🔧 Technologies Used
- Python
- Pandas
- NetworkX
- NLTK
- Scikit-learn
- Matplotlib

## 📂 Dataset
The project uses two datasets:
1. `twitter_dataset.xlsx` - Contains tweets with `Tweet_ID`, `Username`, and `Text`.
2. `users_following.xlsx` - Contains `Username` and a list of `Following` users.

## 🛠 Steps in the Project
### 1️⃣ **Data Preprocessing**
- Load Twitter dataset and user-following data.
- Perform text preprocessing (tokenization, stopword removal, lemmatization).
- Handle missing values and duplicates.

### 2️⃣ **Graph Construction**
- **Tweet-Word Graph:** Connects tweets to words.
- **User-Following Graph:** Connects users based on their follow relationships.

### 3️⃣ **Applying HITS Algorithm**
- Computes **authority scores** for tweets and **hub scores** for words.
- Determines user importance by summing up their tweet authority scores.

### 4️⃣ **Applying PageRank Algorithm**
- Uses PageRank to rank users based on the influence of their followers.
- Saves the results in `pagerank_output.xlsx`.

## 📊 Results
- The **most influential tweets** and **users** are identified using **HITS and PageRank**.
- The influence of users is **propagated** from tweets to the user-following graph.
- The final ranked users are stored in an **Excel file** for further analysis.


