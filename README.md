# AllLife Bank Personal Loan Campaign

## Problem Statement

### Context

AllLife Bank is a US bank with a growing customer base. The majority of these customers are liability customers (depositors) with varying sizes of deposits. The number of customers who are also borrowers (asset customers) is quite small, and the bank is interested in expanding this base rapidly to bring in more loan business and earn more through interest on loans. In particular, the management wants to explore ways of converting its liability customers to personal loan customers (while retaining them as depositors).

A campaign that the bank ran last year for liability customers showed a healthy conversion rate of over 9% success. This has encouraged the retail marketing department to devise campaigns with better target marketing to increase the success ratio.

### Objective

To predict whether a liability customer will buy personal loans, to understand which customer attributes are most significant in driving purchases, and identify which segment of customers to target more.

### Data Dictionary
* `ID`: Customer ID
* `Age`: Customer’s age in completed years
* `Experience`: #years of professional experience
* `Income`: Annual income of the customer (in thousand dollars)
* `ZIP Code`: Home Address ZIP code.
* `Family`: the Family size of the customer
* `CCAvg`: Average spending on credit cards per month (in thousand dollars)
* `Education`: Education Level. 1: Undergrad; 2: Graduate;3: Advanced/Professional
* `Mortgage`: Value of house mortgage if any. (in thousand dollars)
* `Personal_Loan`: Did this customer accept the personal loan offered in the last campaign? (0: No, 1: Yes)
* `Securities_Account`: Does the customer have a securities account with the bank? (0: No, 1: Yes)
* `CD_Account`: Does the customer have a certificate of deposit (CD) account with the bank? (0: No, 1: Yes)
* `Online`: Do customers use internet banking facilities? (0: No, 1: Yes)
* `CreditCard`: Does the customer use a credit card issued by any other Bank (excluding All life Bank)? (0: No, 1: Yes)

## Getting Started

### Prerequisites

- Python 3.7 or above
- Jupyter Notebook
- Git

### Installation

1. Clone the repository
    ```bash
    git clone https://github.com/yourusername/AllLifeBank_PersonalLoanCampaign.git
    cd AllLifeBank_PersonalLoanCampaign
    ```

2. Create and activate a virtual environment
    ```bash
    python3 -m venv env
    source env/bin/activate
    ```

3. Install the required libraries
    ```bash
    pip install -r requirements.txt
    ```

## Project Workflow

### 1. Data Loading

- Load the data from `data/raw/Loan_Modelling.csv`.
- Perform an initial overview of the dataset.

### 2. Exploratory Data Analysis (EDA)

- Conduct a thorough analysis of the data to understand the distribution of variables, detect outliers, and identify patterns.
- Visualize important features and their relationships using histograms, boxplots, and heatmaps.
- Notebooks: `notebooks/EDA.ipynb`

### 3. Data Preprocessing

- Handle missing values and outliers.
- Encode categorical variables.
- Standardize or normalize numerical variables if necessary.
- Notebooks: `notebooks/Preprocessing.ipynb`
- Scripts: `scripts/data_preprocessing.py`

### 4. Model Building

- Split the data into training and test sets.
- Build and train machine learning models (e.g., Decision Tree, Random Forest).
- Use techniques like GridSearchCV for hyperparameter tuning.
- Notebooks: `notebooks/Model_Building.ipynb`
- Scripts: `scripts/model_training.py`

### 5. Model Evaluation

- Evaluate the models using metrics like accuracy, precision, recall, and F1-score.
- Visualize the performance using confusion matrices and ROC curves.
- Notebooks: `notebooks/Model_Evaluation.ipynb`
- Scripts: `scripts/model_evaluation.py`

### 6. Model Deployment

- Save the best model to `results/models/decision_tree_model.pkl`.
- Use the saved model for making predictions on new data.

## Results

### Key Findings

- Income, credit card spending, family size, and education level are significant predictors of personal loan acceptance.
- High-income customers with moderate to high credit card spending are more likely to accept personal loans.

### Visualizations

- [Correlation Heatmap](results/figures/correlation_heatmap.png)
- [Feature Importances](results/figures/feature_importances.png)
- [Decision Tree Visualization](results/figures/decision_tree.png)

## Actionable Insights and Business Recommendations

Based on the analysis and modeling of the personal loan campaign data for AllLife Bank, here are several actionable insights and recommendations for the bank to enhance its marketing strategies and improve the conversion rate of liability customers to personal loan customers:

1. **Target High-Income Customers with High Credit Card Spending:** Personalized loan offers with attractive terms could be provided to these customers to increase the likelihood of loan acceptance.
2. **Focus on Customers with Higher Education Levels:** Tailor marketing campaigns to highlight the benefits of personal loans for educational advancement or other professional development opportunities.
3. **Leverage Family Size in Marketing:** Emphasize financial security and support for families. Highlight how personal loans can help in meeting family needs, such as education, healthcare, or housing.
4. **Promote Loans to Customers with Existing Relationships:** Utilize cross-selling strategies to promote personal loans to customers who already have other types of accounts with the bank.
5. **Age-Specific Marketing:** Develop age-specific marketing strategies that address the unique financial needs and goals of different age groups.
6. **Reevaluate Credit Card Offers:** Investigate the reasons why customers prefer credit cards from other banks and address these gaps.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to AllLife Bank for providing the dataset and the opportunity to work on this project.
- Thanks to the contributors and the open-source community for the libraries and tools used in this project.

