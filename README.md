# Alter Diaper Review Analysis Dashboard

This project presents an end-to-end natural language processing (NLP) analysis of customer reviews for **Alter Diapers**, collected from Amazon. The data was analyzed using various NLP techniques and visualized in Power BI to generate actionable insights regarding customer sentiments, emotions, and product perceptions.

---

## Data Source

The data for this project was collected by scraping customer reviews from the Amazon product page for Alter Diapers. All data used was publicly accessible at the time of extraction.

---

## NLP Techniques Applied

Several NLP techniques were applied to transform unstructured review text into meaningful and structured insights:

### 1. Adjective Extraction
Descriptive adjectives were extracted to identify common attributes and product feedback, such as "soft", "comfortable", "absorbent", etc.

### 2. Named Entity Recognition (NER)
Used to extract specific entities such as quantities, materials, or notable terms (e.g., "Material", "10/10", "CARDINAL") mentioned in the reviews.

### 3. Emotion Detection
Emotion analysis was performed to detect and rank the top emotions expressed in the reviews. The top three detected emotions were:
- Neutral
- Joy
- Sadness (also present but in smaller proportion)

### 4. Empathy Review Classification
Reviews were classified into categories reflecting empathy-related tones such as concern, care, and relatability. The most common categories were:
- Neutral (48.1%)
- Joy (22.79%)
- Others included sadness, anger, fear, and disgust

### 5. Sentiment Analysis
Each review was categorized as either positive, neutral, or negative using sentiment classification models:
- Positive: 207 reviews
- Neutral: 15 reviews
- Negative: 83 reviews

---

## Visualization with Power BI

The processed results were visualized using Power BI in an interactive dashboard. Key features of the dashboard include:

- Total Reviews: 305
- Average Rating: 3.79
- Sentiment Distribution: Positive (207), Neutral (15), Negative (83)
- Filters for Diaper Type and Size
- Line Chart of Average Ratings over Time (2019–2024)
- Adjective Frequency Bar Chart (e.g., helpful, soft, comfortable)
- Empathy Emotion Donut Chart and Highlight of Top 2 (Neutral and Joy)
- Named Entity Recognition (NER) Table with entities such as material and quantity
- Review Viewer Panel with original customer review snippets

---

## Key Insights

- Most commonly used adjectives were "helpful", "good", "soft", and "comfortable", indicating customer satisfaction with usability and comfort.
- Majority of reviews showed a neutral or joyful emotional tone, with minimal presence of anger, fear, or disgust.
- Sentiment analysis showed approximately 68% of reviews were positive, suggesting high overall satisfaction.
- Empathy-based analysis revealed a large number of customers related to the product in a neutral or caring way, with joy being the most dominant emotional expression.
- NER extraction helped identify patterns in review structure, such as frequent mentions of product features and numerical ratings (e.g., "10/10").

---

## Repository Contents

- scraper – Scripts for scraping Amazon reviews
- nlp analyse – Jupyter notebooks for NLP tasks (adjective extraction, NER, sentiment, emotion, empathy)
- power bi dashboard – Power BI dashboard (.pbix file)
- datasets – Cleaned and processed datasets
- read me – Project documentation
