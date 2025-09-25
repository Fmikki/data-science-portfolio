# 🐦 Twitter vs X: Moderation, Sentiment, and Freedom of Speech

## 📌 Overview
This project investigates how **Twitter’s transition to X under Elon Musk** affected sentiment, moderation discourse, and freedom of speech.  
We analyzed **300,000+ tweets** from both the Twitter (pre-Elon) and X (post-Elon) eras using **natural language processing (NLP)** to compare sentiment polarity, topic diversity, and moderation-related discussions.  

This study builds on prior academic work and contributes to understanding how **platform governance shapes online discourse**.

---

## 🔧 Tools & Libraries
- **Python**: Pandas, NumPy, Matplotlib, Seaborn  
- **NLP**: CardiffNLP RoBERTa, VADER, BERTopic  
- **Visualization**: WordCloud, matplotlib  
- **Statistical Tests**: Chi-Square test for sentiment differences  

---

## 📊 Methods
1. **Data Collection**
   - Pre-Elon: ~300K tweets from Kaggle archives & scrapers  
   - Post-Elon: ~300K tweets from APIs & Hugging Face datasets  
   - Filtered tweets using **80+ moderation-related keywords**  

2. **Preprocessing**
   - Removed duplicates & retweets  
   - Tokenization, stopword removal, lemmatization  

3. **Sentiment Analysis**
   - **VADER** → baseline lexicon scores  
   - **RoBERTa** → transformer-based sentiment classification  

4. **Topic Modeling**
   - Applied **BERTopic** for thematic clustering of moderation-related tweets  
   - Generated **word clouds** for comparison  

5. **Statistical Testing**
   - Chi-Square test on sentiment distribution across platforms  

---

## ✅ Results
- **Sentiment**  
  - Twitter → Positive-heavy, conversational tone  
  - X → More neutral/ideological, slight rise in negativity (not statistically significant, p = 0.89)  

- **Topic Shifts**  
  - Twitter → Personal/emotional discourse (ban, harassment, jokes, anecdotes)  
  - X → Ideological/policy-driven (free speech, decentralization, crypto, tech)  

- **Key Finding**  
  - Platform governance changes **did not cause a significant rise in toxicity**, but **shifted discourse tone** toward ideology and policy.  

---

## 📸 Visualizations
![Sentiment Distribution](https://github.com/Fmikki/data-science-portfolio/blob/main/Sentiment%20Distribution.png)
*Sentiment comparison between Twitter and X (RoBERTa results)*  

![Moderation Word Cloud](https://github.com/Fmikki/data-science-portfolio/blob/main/Moderation%20Word%20Cloud.png)  
*Keyword-driven topic contrast in moderation tweets*  

---

## 🔗 Files
- `(https://github.com/Fmikki/data-science-portfolio/blob/main/Twitter_X.ipynb)` → Preprocessing, sentiment, and BERTopic code  
- `(https://github.com/Fmikki/data-science-portfolio/blob/main/Final_Labeled_X_Tweets.csv)` → Example dataset  
- `(https://github.com/Fmikki/data-science-portfolio/blob/main/Sentiment%20Distribution.png)`, `(https://github.com/Fmikki/data-science-portfolio/blob/main/Moderation%20Word%20Cloud.png)` → Visuals  

---

## 📖 Insights
- **Transformer models > Lexicon models**: RoBERTa handled sarcasm and politics better than VADER  
- **Discourse shift**: Twitter = emotional/personal; X = ideological/policy-driven  
- **Governance matters**: Rule changes subtly shifted tone and audience focus, but didn’t drastically raise negativity  

---

## 🚀 Future Work
- Expand dataset to 2024–25 for longitudinal tracking  
- Fine-tune DistilBERT for moderation-specific sentiment  
- Network analysis of misinformation & toxic communities  
