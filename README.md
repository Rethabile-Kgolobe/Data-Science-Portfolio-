# Data-Science-Portfolio-
This portfolio showcases a collection of Data Science and Data Analysis projects I have undertaken for personal growth and passion-driven learning. It highlights my achievements and technical skills with regular updates to reflect my ongoing journey and progress in the field.
- Email:rethabilethuto3@gmail.com 
- LinkedIn:https://www.linkedin.com/in/rethabile-kgolobe-b82121265?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app
# Projects

# HexSoftwares Project: Exploratory Data Analysis, House Price Prediction, and Loan Approval Prediction

## Project Overview

This repository contains three distinct data analysis and machine learning projects:

1.  **Iris Dataset EDA:** An exploratory data analysis of the classic Iris dataset, focusing on understanding feature distributions and species differentiation.
2.  **House Price Prediction:** A project involving data preprocessing, feature engineering, and linear regression modeling to predict house prices using the House Price Prediction dataset.
3.  **Loan Approval Prediction:** Development of a robust machine learning tool to predict whether a loan application should be accepted based on applicant features.

## Project 1: Iris Dataset EDA

### Dataset Information

The Iris dataset is a classic dataset in machine learning and statistics. It contains 150 instances of iris flowers, with measurements of their sepal length, sepal width, petal length, and petal width (all in centimeters). The goal is to understand the underlying structure of the data, identify potential relationships between features, and gain insights into how these features differentiate the three Iris species: Setosa, Versicolor, and Virginica.

The Iris dataset includes the following features:

*   **Id:** A unique identifier for each flower sample.
*   **SepalLengthCm:** Length of the sepal in centimeters.
*   **SepalWidthCm:** Width of the sepal in centimeters.
*   **PetalLengthCm:** Length of the petal in centimeters.
*   **PetalWidthCm:** Width of the petal in centimeters.
*   **Species:** The species of the iris flower (Setosa, Versicolor, or Virginica).

### Steps Performed

1.  **Data Loading:** The Iris dataset was loaded from a CSV file (`iris.csv`) into a Pandas DataFrame.
2.  **Data Inspection:**

    *   The first few rows of the dataset were displayed to get a sense of the data.
    *   Descriptive statistics (mean, median, standard deviation, etc.) were calculated for each numerical feature to understand their distributions.
    *   The data types of each column were checked to ensure they were appropriate.
    *   Checked the number of rows and columns in the dataset.
3.  **Data Cleaning:**

    *   Checked for missing values using `.isnull().sum()`. No missing values were found.
    *   Removed the `Id` column as it is not relevant for analysis.
    *   Checked for duplicate entries. Duplicates were dropped to ensure data quality.
4.  **Exploratory Data Analysis (EDA):**

    *   **Univariate Analysis:** Examined the distribution of individual features using histograms and box plots.
    *   **Multivariate Analysis:**
        *   Scatter plots were created to visualize the relationships between pairs of features.
        *   A pair plot was generated to visualize all pairwise relationships in a single grid.
        *   A correlation matrix was calculated and visualized using a heatmap to identify highly correlated features.

### Tools Used

*   Python
*   Pandas
*   NumPy
*   Matplotlib
*   Seaborn

### Key Findings and Insights

*   **Species Differentiation:** The Iris species can be relatively well separated using petal measurements (length and width). Setosa is notably distinct from Versicolor and Virginica.
*   **Feature Correlations:**

    *   Strong positive correlations exist between petal length and petal width. This suggests that as petal length increases, petal width also tends to increase.
    *   Sepal length and sepal width show a weaker correlation compared to petal dimensions.
*   **Data Distributions:**

    *   Petal length and petal width exhibit clear differences across the three species, making them good candidates for classification.
    *   Sepal width has more overlap between the species, making it a less reliable feature for distinguishing between them.
*   **Outliers:**

    *   Box plots revealed some outliers in sepal width, indicating some flowers with unusually large or small sepal widths compared to the rest of the dataset.
*   **Observations on Species:**

    *   *Iris setosa* tends to have smaller petal lengths and widths but larger sepal widths.
    *   *Iris virginica* tends to have more considerable petal lengths and widths but smaller sepal widths.
    *   *Iris versicolor* falls in between *Iris setosa* and *Iris virginica* in terms of petal and sepal dimensions.

### Visualizations

*   **Pairplot:** Illustrates the relationships between all pairs of features, with different colors representing different species.

    (Ideally, you would embed the pairplot image here)

*   **Correlation Heatmap:** Displays the correlation coefficients between numerical features. Darker colors indicate stronger correlations (positive or negative).

    (Ideally, you would embed the heatmap image here)

### Conclusion

The Exploratory Data Analysis of the Iris dataset revealed significant insights into the characteristics of the different Iris species and the relationships between their sepal and petal dimensions. Petal length and petal width are beneficial for distinguishing between species, while sepal measurements are less discriminatory. The strong correlation between petal length and width suggests that these features are related and could be used together in predictive models. The insights gained from this EDA can inform the selection of appropriate features and models for classification tasks involving the Iris dataset. Further analysis could include building machine learning models to predict Iris species based on these measurements.

## Project 2: House Price Prediction

### Dataset Information

The House Price Prediction dataset contains information about various features of houses and their corresponding sale prices. The goal is to build a model that can accurately predict the sale price of a house based on its features.

Key features in the dataset include:

*   **MSSubClass:** The building class
*   **MSZoning:** The general zoning classification
*   **LotArea:** Lot size in square feet
*   **LotConfig:** Lot configuration
*   **BldgType:** Type of dwelling
*   **OverallCond:** Overall condition rating
*   **YearBuilt:** Original construction date
*   **YearRemodAdd:** Remodel date
*   **Exterior1st:** Exterior covering on house
*   **BsmtFinSF2:** Type 2 finished square feet
*   **TotalBsmtSF:** Total basement square feet
*   **SalePrice:** The property's sale price (target variable)

### Steps Performed

1.  **Data Loading:** The House Price Prediction dataset was loaded from a CSV file (`HousePricePrediction.csv`) into a Pandas DataFrame.
2.  **Data Inspection:**

    *   The first few rows of the dataset were displayed to get a sense of the data.
    *   Descriptive statistics (mean, median, standard deviation, etc.) were calculated for each numerical feature to understand their distributions.
    *   The data types of each column were checked to ensure they were appropriate.
    *   Checked the number of rows and columns in dataset.
3.  **Data Cleaning:**

    *   Checked for missing values using `.isnull().sum()`. Missing values were handled appropriately (dropping the target variable with missing values).
    *   Removed any unnecessary columns (e.g., 'Id').
4.  **Feature Engineering:**

    *   Converted categorical features into numerical using one-hot encoding with `pd.get_dummies()`.
    *   Handled multicollinearity and dimensionality reduction via correlation analysis
5.  **Data Scaling:**

    *   Scaled the numerical features using `MinMaxScaler` to ensure all features are on the same scale.
6.  **Model Training and Evaluation:**

    *   Split the data into training and testing sets.
    *   Trained a Linear Regression model on the training data.
    *   Evaluated the model's performance on the testing data using Mean Absolute Error (MAE).  Also, a Lasso regression model was trained and evaluated.

### Tools Used

*   Python
*   Pandas
*   NumPy
*   Seaborn
*   Matplotlib
*   Scikit-learn (sklearn)

### Key Findings and Insights

*   One-hot encoding of categorical variables significantly expands the feature space.
*   Scaling numerical features improves the performance and stability of linear regression models.
*   The linear regression model achieved a sure MAE, indicating the average absolute difference between predicted and actual sale prices.  *This needs to be replaced with the actual MAE you observed*.
*   The Lasso Regression model was added to reduce the impact of less relevant features on the overall model and provided an improved MAE value.

### Model Performance

*   **Linear Regression MAE:** 0.04

### Conclusion

This project demonstrated the building of a linear regression model to predict house prices. Data preprocessing, feature engineering, and data scaling were crucial to improving model performance. The model can be further enhanced by exploring other regression algorithms, feature selection techniques, and hyperparameter tuning.  Also, it is essential to consider the impact of missing data the importance of investigating missingness, and the potential introduction of bias that the missingness implies.

## Project 3: Loan Approval Prediction

### Overview

Loans are a significant source of income for banks and play a critical role in the economy and individuals managing expenses, purchasing luxuries, etc. However, banks must examine many factors to assess whether the candidate is granted a loan. Since there are many features, banks can automate this process using machine learning tools to reduce the time taken for decision-making.

### Objective

- To develop a robust machine learning tool to determine whether a loan application should be accepted based on the applicant's features, such as marital status, education level, income, etc.

### Methods

1.  **Data Preprocessing:**

    *   **Handling Missing Values:** Missing values were identified and appropriately handled.
    *   **Handling Outliers:** Outliers were detected and managed to ensure data quality.
    *   **Feature Engineering:** New features were created or transformed to enhance model performance.
2.  **Models Development:**

    *   **Random Forest:** Implemented for its robustness and ability to handle complex interactions.
    *   **Gradient Boosting:** Used for handling large datasets and feature interactions efficiently.
    *   **XG Boosting:** Utilized for its speed and performance in handling sparse data.
3.  **Evaluation:**

    *   Model performance was evaluated using accuracy, precision, recall, and F1 score.
4.  **Hyperparameter Tuning:**

    *   The best-performing model, Random Forest, was tuned using Grid Search combined with cross-validation to optimize its parameters.

### Results

*   **Model Performance:**

    | Model | Accuracy |
    |-------|----------|
    | Random Forest (Before Tuning) | 0.8698 |
    | Random Forest (After Tuning)  | 0.8835 |

### Conclusion

This project demonstrated the effectiveness of machine learning in automating loan approval decisions. Random Forest performed well, followed by XG Boosting. Hyperparameter tuning significantly improved the accuracy of the Random Forest model. The results highlight the potential for machine learning to streamline and enhance the loan approval process by reducing manual evaluation time and improving decision accuracy.


4. **Hyperparameter tuning**:
   - The best-performing model, Random Forest, was tuned to optimize its performance.
   - The tuning process utilizes Grid search to search for the best parameters combined with cross-validation.
     
## Results
- Random Forest performed well compared to the other two models, followed by XG Boosting with 0.8698 accuracy.
- Hyperparameter tuning was performed on Random forest to improve its accuracy from 0.8698 to 0.8835.
