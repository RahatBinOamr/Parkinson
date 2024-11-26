# Parkinson's Disease Analysis

This repository contains an analysis of a dataset related to Parkinson's disease. The dataset includes audio-based features extracted from voice recordings, which can be used to distinguish between individuals with Parkinson's disease and those who are healthy. The analysis explores key patterns, correlations, and distributions within the data.

---

## **Dataset**

The dataset can be accessed from the following link:  
https://github.com/RahatBinOamr/Parkinson/blob/main/parkinsons.csv

### **Dataset Features**

1. **`status`**: The target variable indicating the presence of Parkinson's disease.  
   - `1`: Patient with Parkinson's disease.  
   - `0`: Healthy individual.  

2. **Voice Metrics**:
   - **Jitter Features**: Measure frequency variations.
     - `MDVP:Jitter(%)`, `MDVP:RAP`, `MDVP:PPQ`, `Jitter:DDP`.
   - **Shimmer Features**: Measure amplitude variations.
     - `MDVP:Shimmer`, `MDVP:Shimmer(dB)`, `Shimmer:APQ3`, `Shimmer:DDA`.
   - **Harmonics-to-Noise Ratio (HNR)**: Ratio of harmonic sound to noise in the voice.
   - **Spread1 & Spread2**: Measures related to amplitude and frequency spread.
   - **PPE (Pitch Period Entropy)**: Indicates irregularities in pitch.
   - Other features include `DFA`, `NHR`, `RPDE`.

3. **Number of Records**: 195  
4. **Number of Features**: 24

---

## **Exploratory Data Analysis (EDA)**

We explored the dataset through various questions and visualizations.

### **Questions Explored**

#### 1. **What is the distribution of Parkinson's disease status in the dataset?**
   - We analyzed the count of healthy vs. Parkinson's patients.
   - Result: A majority of individuals in the dataset are Parkinson's patients, indicating a class imbalance.
   - Visualization: Bar chart.

#### 2. **Which features are most correlated with Parkinson's disease status?**
   - We calculated the correlation of features with the `status` column.
   - Top Features: `Spread1`, `PPE`, and `DFA`.
   - Visualization: Bar chart of the most correlated features.

#### 3. **How do jitter values differ between healthy and Parkinson's patients?**
   - Comparison of jitter features (`MDVP:Jitter(%)`, `MDVP:RAP`, etc.) between the two groups.
   - Result: Higher jitter values in Parkinson's patients.
   - Visualization: Bar chart of mean jitter values.

#### 4. **How do shimmer values differ between healthy and Parkinson's patients?**
   - Comparison of shimmer features (`MDVP:Shimmer`, `Shimmer:APQ3`, etc.) between the two groups.
   - Result: Higher shimmer values in Parkinson's patients.
   - Visualization: Bar chart of mean shimmer values.

#### 5. **How does the Harmonics-to-Noise Ratio (HNR) vary between healthy and Parkinson's groups?**
   - Comparison of the distribution of HNR values.
   - Result: Healthy individuals have higher HNR values, indicating clearer voice quality.
   - Visualization: Histogram of HNR.

---

## **Results**

1. **Parkinson's patients**:  
   - Exhibit higher jitter and shimmer values, indicating instability in pitch and amplitude.  
   - Have lower HNR values, reflecting noisier voice signals.

2. **Key Features for Diagnosis**:  
   - `Spread1`, `PPE`, `DFA`, `Jitter`, and `Shimmer` are important indicators.

3. **Class Imbalance**:  
   - The dataset is imbalanced, with most samples belonging to Parkinson's patients.

---

## **Visualizations**

The repository contains visualizations for:
1. Distribution of Parkinson's disease status.
2. Top features correlated with the disease.
3. Comparison of jitter and shimmer metrics.
4. HNR distributions.

---

## **Challenges**

1. **Class Imbalance**:
   - The majority class (`status = 1`) can bias predictive models.
   - Addressed through appropriate model evaluation techniques.

2. **Small Dataset**:
   - Limited number of records (195) can lead to overfitting in machine learning models.

3. **Complex Features**:
   - Some features like `RPDE`, `DFA`, and `NHR` require domain expertise for interpretation.

---

## **Future Work**

1. **Machine Learning Models**:
   - Use the dataset to build classification models (e.g., Logistic Regression, Random Forest, etc.).
   - Evaluate using accuracy, precision, recall, and F1-score.

2. **Feature Selection**:
   - Focus on the most correlated features for improved model performance.

3. **Imbalance Handling**:
   - Use techniques like oversampling, undersampling, or class weighting.

---

## **How to Use**

1. Clone the repository:
   git clone https://github.com/RahatBinOamr/Parkinson



## Install dependencies
1. python install on your system
2. pip install pandas numpy matplotlib

