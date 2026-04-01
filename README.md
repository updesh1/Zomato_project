# 🍽️ Zomato Restaurant Analytics: Customer Behavior & Rating Prediction

## 📌 Project Overview
This project analyzes Zomato restaurant data by combining restaurant metadata and customer reviews to extract actionable business insights and build a machine learning model to predict restaurant ratings.

The objective is to understand customer behavior, identify factors influencing ratings, and help businesses improve decision-making using data-driven insights.

---

## 📊 Dataset Description

The project uses two datasets:

### 1. Restaurant Metadata
- Name  
- Cost  
- Cuisines  
- Timings  
- Collections  

### 2. Customer Reviews
- Reviewer  
- Review  
- Rating  
- Time  
- Pictures  

After merging:
- **Rows:** 10,000  
- **Columns:** 13  

---

## 🧹 Data Preprocessing

- Merged datasets using restaurant name  
- Handled missing values:
  - Dropped `Collections` (50% missing)  
  - Filled `Cost` using median  
  - Filled `Timings` using mode  
- Removed duplicate records  
- Converted:
  - Rating → numeric  
  - Cost → numeric  
  - Time → datetime  

---

## 🧠 NLP (Text Processing)

Applied on `Review` column:
- Lowercasing  
- Remove punctuation  
- Remove URLs  
- Remove digit-containing words    
- Contraction expansion  

---

## 📈 Exploratory Data Analysis (EDA)

Visualizations performed:
- Rating Distribution  
- Cost vs Rating  
- Top Restaurants  
- Cuisine Analysis  
- Engagement Analysis (Pictures vs Rating)  
- Time-based Trends  
- Correlation Heatmap  
- Pair Plot  

---

## 🔍 Key Insights

- Most ratings lie between **3.5 – 4.5**  
- **Cost has very weak correlation with rating (~0.14)**  
- Customer engagement improves perception  
- Popular cuisines dominate demand  
- Peak hours can reduce service quality  

---

## 🧪 Hypothesis Testing

Statistical tests performed:

| Hypothesis | Test Used |
|----------|--------|
| Cost vs Rating | Spearman Correlation |
| Pictures vs Rating | Mann-Whitney U Test |
| Review Length vs Rating | Spearman Correlation |

---

## 🤖 Machine Learning Models

### ✅ Model 1: Linear Regression
- Baseline model  
- Easy to interpret  

### ✅ Model 2: Random Forest Regressor
- Handles non-linearity  
- Better performance  

### 🔧 Hyperparameter Tuning
- Used **GridSearchCV** to find optimal parameters  

---

## 📊 Model Evaluation Metrics

- MAE (Mean Absolute Error)  
- MSE (Mean Squared Error)  
- R² Score  

---

## 💼 Business Recommendations

- Focus on **quality & service instead of pricing**  
- Improve performance during **peak hours**  
- Encourage **photo uploads & detailed reviews**  
- Invest in **high-demand cuisines**  
- Use customer feedback for continuous improvement  

---

## 🚀 Tech Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- NLTK  

---

## 📂 Project Structure
