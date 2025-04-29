
# Personalized News Feed Agent

## Overview
This project implements a **Personalized News Feed Agent** using a hybrid recommendation system based on **Collaborative Filtering** and **Content-Based Filtering**. The agent suggests relevant news articles to users based on their preferences and past interactions. 

It leverages pre-trained embeddings and a collaborative filtering model to generate recommendations and continuously adapts to user feedback. The solution uses **SentenceTransformers** for embeddings, **scikit-learn** for cosine similarity, and **pandas** for data manipulation.

## Objective
To build an AI agent that can recommend news articles tailored to individual user preferences. The recommendation engine uses collaborative filtering and fine-tuned embeddings for better content matching and personalization.

## Approach
- **Data**: A news dataset with headlines, short descriptions, and categories is used. We preprocess the data by cleaning text and tokenizing it.
- **Embeddings**: We generate article embeddings using the `SentenceTransformer` model, which encodes the articles into high-dimensional vectors.
- **Recommendation Models**:
  - **Collaborative Filtering**: Based on user interactions with articles, we use cosine similarity to find similar users and recommend articles they have interacted with.
  - **Content-Based Filtering**: For each user, recommendations are based on article similarity to the user's profile (generated from their past interactions).
  - **Hybrid Model**: A combination of both models that adapt based on weights.

## Features
- **Personalized Recommendations**: The agent suggests top 5-10 articles based on the user's past interactions.
- **Adaptability**: The agent updates the user profile after each feedback (clicks, skips) to generate more accurate future recommendations.
- **Visualizations**: Visualize user preferences and recommended article categories.
  
## Requirements
To run this project, make sure to install the following dependencies:

### Dependencies
- pandas
- numpy
- sentence-transformers
- scikit-learn
- matplotlib
- nltk

You can install them using pip:

```bash
pip install -r requirements.txt
```

## Setup Instructions

### 1. **Download Dataset**
Ensure you have a news dataset. If you're using the sample dataset (`News_Category_Dataset_v3.json`), place it in the `data` directory.

### 2. **Running the Code**
To run the code:
1. Place the dataset (`News_Category_Dataset_v3.json`) in the `data/` directory.
2. Run the Python script or Jupyter notebook.

```bash
python personalized_news_feed.py
```

### 3. **Expected Outputs**
- **News Feed for Users**: Personalized top 5–10 article recommendations for each user.
- **Visualizations**: Bar plots showing user preferences and recommended categories.

## Files Structure
- `personalized_news_feed.py`: Main script to generate recommendations.
- `data/`: Contains dataset, preprocessed data, interaction matrix, embeddings, and user profiles.
- `plots/`: Visualizations of user preferences and recommended categories.
- `requirements.txt`: List of required dependencies.
- `README.md`: This file containing project details and instructions.

## Evaluation Criteria
The project will be evaluated based on:
1. **Clarity and structure of code**: Clear and well-commented code.
2. **Model performance**: Effective use of collaborative filtering and fine-tuned embeddings.
3. **Quality of recommendations**: Relevant and diverse recommendations.
4. **Adaptability**: How well the agent adapts to changing user preferences.
5. **Presentation**: Quality of the demonstration video.

## Conclusion
This project provides a personalized recommendation engine using both collaborative and content-based filtering techniques. It adapts to user preferences over time and can be extended to more sophisticated recommendation approaches.

---

**PurpleMerit Recruitment Team**  
Thank you for reviewing my work! I look forward to your feedback.
