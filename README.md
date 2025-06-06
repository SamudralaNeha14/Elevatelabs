# Elevatelabs
**Task-1**
The Titanic dataset undergoes a structured preprocessing pipeline to ensure data quality and facilitate effective machine learning modeling.

1. **Data Loading**: The dataset, titled *Titanic-Dataset.csv*, is read into a pandas DataFrame, allowing for further manipulation and analysis.

2. **Initial Inspection**: A preliminary review of the dataset is conducted to assess data types, detect inconsistencies, and quantify missing values across all columns.

3. **Handling Missing Values**: Missing data is systematically addressed. The `Age` column is imputed with the median to maintain numerical integrity, while the categorical feature `Embarked` is filled using the mode to preserve its most frequent category. Additionally, absent values in the `Cabin` column are replaced with "Unknown" to retain information without introducing bias.

4. **Encoding Categorical Features**: To facilitate machine learning algorithms that require numerical input, categorical variables—namely `Sex`, `Embarked`, `Cabin`, and `Pclass`—are transformed using encoding techniques. `Label Encoding` is applied where categorical values have an inherent order, whereas `One-Hot Encoding` is used for nominal categories to prevent unintended ordinal relationships.

5. **Scaling Numerical Features**: Numerical columns (`Age`, `SibSp`, `Parch`, and `Fare`) are normalized using `MinMaxScaler`, which scales values to a fixed range. This standardization ensures feature comparability and prevents models from disproportionately weighting certain variables.

6. **Outlier Visualization**: Boxplots are generated to examine the distribution of numerical variables, identifying extreme values that may affect model performance.

7. **Outlier Removal**: The *Interquartile Range (IQR) Method* is employed to detect and eliminate outliers from the dataset, enhancing data quality by reducing statistical noise.

**Task-2**


 ### **Exploratory Data Analysis (EDA) Summary**

1. **Data Loading & Inspection**: The dataset is imported, and its structure, data types, and missing values are analyzed.  
2. **Handling Missing Values**: `'Age'`, `'Cabin'`, and `'Embarked'` are imputed appropriately, ensuring no gaps remain.  
3. **Summary Statistics**: Key numerical features are examined using mean, median, and standard deviation.  
4. **Visualizations**: Histograms and boxplots reveal feature distributions and detect outliers.  
5. **Feature Relationships**: Pairplots and correlation heatmaps highlight dependencies between variables.  
6. **Feature-Level Inferences**: Survival rates are assessed across passenger class, gender, age, fare, and family size, revealing significant trends.  

