# HealthPulse: Modeling the Relationship Between Air Conditions and Flu Index Using Time-Series Machine Learning

## Abstract

HealthPulse is a data-driven research project that investigates the relationship between **air condition indicators** and **flu index trends** through systematic data preprocessing, exploratory analysis, and machine learning–based time-series modeling.  
The study applies **XGBoost regression** with both standard and time-aware validation strategies to evaluate predictive performance and temporal generalization.

---

## 1. Research Motivation

Seasonal influenza exhibits strong temporal patterns and is influenced by environmental factors such as air conditions.  
Understanding and modeling these relationships can support:
- Public health monitoring
- Early warning systems
- Data-informed policy decisions

This project explores whether machine learning models—particularly **gradient boosting methods**—can effectively capture temporal dependencies in flu index data when combined with environmental features.

---

## 2. Data Description

The dataset consists of:
- Time-indexed **flu index measurements**
- Corresponding **air condition indicators**
- Observations spanning multiple temporal periods

Key preprocessing steps ensure data consistency and suitability for time-series modeling.

---

## 3. Methodology

### 3.1 Data Preprocessing
- Handling missing and inconsistent values
- Feature type normalization
- Temporal feature alignment
- Sorting and indexing by time to prevent data leakage

---

### 3.2 Exploratory Data Analysis (EDA)

Visualization techniques are applied to:
- Examine long-term and seasonal trends
- Identify correlations between air conditions and flu index
- Detect anomalies and distribution shifts

---

### 3.3 Modeling Approach

#### Baseline Model
- **XGBoost Regression**
- Random train–test split
- Used as a benchmark to assess predictive capacity

#### Time-Series–Aware Model
- **XGBoost with TimeSeriesSplit**
- Ensures chronological integrity in training and validation
- Hyperparameter tuning via randomized search
- Reduces over-optimistic performance estimates caused by temporal leakage

---

## 4. Experimental Setup

- Model training and evaluation conducted in Python
- Cross-validation adapted for time-series data
- Performance assessed using regression error metrics
- All experiments implemented in a single reproducible notebook

---

## 5. Results and Discussion

Key findings include:
- Clear temporal structure in flu index trends
- Improved robustness when using time-series cross-validation
- Evidence that environmental variables contribute to predictive performance
- Standard random splits may overestimate real-world performance in temporal data

These results highlight the importance of **time-aware evaluation** in health-related predictive modeling.

---

## 6. Limitations

- Limited feature diversity (no demographic or behavioral variables)
- Single-model family explored (tree-based boosting)
- No causal inference claims; findings are correlational

---

## 7. Future Work

Potential extensions include:
- Incorporating additional environmental and socio-demographic data
- Comparing with deep learning approaches (e.g., LSTM, Temporal CNN)
- Applying causal inference or intervention analysis
- Deploying the model in a real-time public health monitoring system

---

## 8. Technologies

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

---

## 9. Author

**Yichen Qu**  

This project is conducted for academic and research purposes.

