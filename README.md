# Topic-Modeling-on-Mental-Health-Related-Tweets

## **📌 Project Overview**
This project explores **mental health discussions on Twitter** using **Natural Language Processing (NLP) and Machine Learning (ML)** techniques. By implementing **Latent Dirichlet Allocation (LDA) and BERTopic**, we extract key themes, trends, and insights from tweets to analyze public sentiment and engagement in mental health-related conversations.

## **🎯 Objectives**
- Extract dominant **topics** from mental health-related tweets.
- Compare the effectiveness of **LDA** and **BERTopic** in topic modeling.
- Evaluate topic coherence and structure through **visualizations and metrics**.
- Provide valuable insights for **mental health awareness and intervention**.

## **📂 Dataset Information**
- **Source:** Kaggle (Mental Health Twitter Dataset)
- **Size:** 2,000+ tweets
- **Key Features:**
  - `post_id`: Unique tweet identifier.
  - `post_text`: Tweet content.
  - `post_created`: Timestamp of the tweet.
  - `user_id`: Unique user identifier.
  - `followers`, `friends`, `retweets`: Engagement metrics.
  - `label`: Indicates relevance to mental health.

## **🛠️ Implementation Details**
### **1️⃣ Data Preprocessing**
- **Text Cleaning**: Removed URLs, mentions, hashtags, special characters.
- **Tokenization & Lemmatization**: Standardized text representation.
- **TF-IDF Vectorization**: Converted text into numerical features for modeling.

### **2️⃣ Topic Modeling Approaches**
#### **📌 Latent Dirichlet Allocation (LDA)**
- Utilized **TF-IDF** for text vectorization.
- Set **10 topics** for categorization.
- Applied **Dirichlet distributions** to extract structured themes.

#### **📌 BERTopic**
- Used **CountVectorizer & Transformer-based embeddings**.
- Applied **UMAP for dimensionality reduction & HDBSCAN for clustering**.
- Initially extracted **289 topics**, later refined to **34 coherent topics**.

### **3️⃣ Model Evaluation & Visualization**
- **Coherence Score**: Assessed topic quality and interpretability.
- **Intertopic Distance Map**: Visualized topic relationships.
![image](https://github.com/user-attachments/assets/10c51e27-c67e-4747-bc3c-2c0c4e15e647)

- **Topic Similarity Heatmap**: Highlighted overlapping themes.
![image](https://github.com/user-attachments/assets/e688e799-4513-4ac4-90fd-d5bce38b7538)

- **Topic Distribution Bar Chart**: Identified dominant discussion points.
![image](https://github.com/user-attachments/assets/e0fd28d3-4589-4d7b-ba4a-0224c6447284)

- **Word Clouds**: Represented key terms for each topic.
![image](https://github.com/user-attachments/assets/39b8279f-9030-4aaf-9d85-b264cf83b298)


## **📊 Key Insights & Findings**
✅ **BERTopic provided superior results** compared to LDA, yielding clearer and more structured topics.
✅ **Key themes** included mental health awareness, anxiety, depression, therapy, and the impact of social media.
✅ **External influences** such as **COVID-19** and **political discourse** were detected.
✅ Reducing the number of topics **from 289 to 34 improved interpretability and coherence**.

## **⚠️ Limitations & Future Enhancements**
- **Data Quality**: Some tweets were irrelevant; improved filtering is needed.
- **Short-Text Challenge**: Contextual embeddings (e.g., **GPT-based models**) could enhance topic accuracy.
- **Overlapping Topics**: Future research could apply **automated topic merging** techniques.
- **Sentiment Analysis Integration**: Combining sentiment classification can offer **deeper emotional insights**.
- **Real-Time Monitoring**: Future studies can explore **live tracking of mental health discussions**.

## **🚀 How to Run the Project**
### **🔹 Prerequisites**
Ensure you have Python installed along with the required dependencies:
```bash
pip install pandas numpy nltk bertopic umap-learn hdbscan matplotlib seaborn
```

### **🔹 Running the Model**
1. Load and preprocess the dataset.
2. Train the **LDA** and **BERTopic** models.
3. Evaluate topics using visualization tools.
4. Analyze extracted insights.

## **👨‍💻 Author & Contributions**
Developed by **Saky**, this project aims to advance **NLP-driven mental health analysis** on social media platforms. Contributions and feedback are welcome!

