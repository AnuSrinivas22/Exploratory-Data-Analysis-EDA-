# AI/ML Internship - Task 2: Exploratory Data Analysis (EDA) - Titanic Dataset

## Objective
The main objective of this task was to perform Exploratory Data Analysis (EDA) on the Titanic dataset. This involved understanding the data's characteristics, identifying patterns, trends, and anomalies using statistical summaries and various visualizations.

## Dataset
The dataset used for this task is the original [Titanic Dataset](https://www.kaggle.com/c/titanic/data).

## Tools and Libraries Used
* **Python**
* **Pandas:** For data loading and manipulation.
* **NumPy:** For numerical operations.
* **Matplotlib:** For creating static visualizations.
* **Seaborn:** For making enhanced statistical graphics.
* **Plotly (Optional, not explicitly used in provided code but mentioned in task description):** For interactive visualizations.

## Exploratory Data Analysis (EDA) Steps Performed:

### 1. Generate Summary Statistics
* Used `df.describe()` to get a quick overview of numerical features (count, mean, std, min, max, quartiles).
* **Key Insight:** Identified missing values in 'Age', 'Cabin', and 'Embarked', and understood the range and distribution of numerical features.

### 2. Create Histograms and Boxplots for Numeric Features
* Generated histograms to show the distribution shape (e.g., skewness for 'Fare', 'SibSp', 'Parch').
* Created boxplots to visualize central tendency, spread, and identify outliers (prominently in 'Age', 'Fare', 'SibSp', 'Parch').
* **Key Insight:** Confirmed skewness and identified the extent of outliers in key features.

### 3. Use Correlation Matrix for Feature Relationships
* Calculated the pairwise correlation matrix for all numerical features.
* Visualized the correlation matrix using a heatmap.
* **Key Insight:** Observed significant correlations like the negative correlation between 'Pclass' and 'Fare', and positive correlations between 'Survived' and 'Fare', and negative correlation between 'Survived' and 'Pclass'.

### 4. Identify Patterns, Trends, or Anomalies
* Used `groupby()` and `crosstab()` to reveal survival patterns based on 'Sex', 'Pclass', and 'Embarked' port.
* **Key Insight:** Females had a significantly higher survival rate than males across all classes. Passengers in 1st class had a much higher survival rate than those in 3rd class.

### 5. Make Basic Feature-Level Inferences from Visuals
* Created targeted boxplots (e.g., 'Age' by 'Survived', 'Fare' by 'Pclass') to confirm visual inferences.
* Calculated survival rates by age groups.
* **Key Insight:** Children showed a higher survival rate. Higher fare generally correlated with higher survival, and this was concentrated in higher passenger classes.

## Visualizations Included:
* `numerical_histograms.png`
* `numerical_boxplots.png`
* `correlation_heatmap.png`
* `age_survival_boxplot.png`
* `fare_pclass_boxplot.png`

## What Was Learned:
Through this task, I gained practical experience in data visualization, computing descriptive statistics, identifying patterns and trends, and recognizing anomalies within a dataset. This fundamental understanding is critical for preparing data for machine learning models.
