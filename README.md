# JioMart Product Price and Rating Analysis Using Machine Learning

## 1. Project Overview

This project focuses on analyzing JioMart product data to understand product pricing patterns, discount strategies, product categories, and customer rating trends using Python and Machine Learning.

The project uses Exploratory Data Analysis (EDA), data visualization, and machine learning algorithms to analyze product information and predict customer ratings.

## 2. Objectives

- Analyze JioMart product information.
- Study product categories and product types.
- Compare market prices and sale prices.
- Calculate product discount percentages.
- Analyze customer rating distributions.
- Identify relationships between product prices and ratings.
- Implement machine learning algorithms for rating prediction.
- Evaluate and compare machine learning model performance.

## 3. Dataset Description

**Dataset:** JioMart Product Dataset

**Source:** Dataset provided for the project.

**Total Records:** 1,026 products.

**Total Features:** 7 columns.

### Dataset Features

| Feature | Description |
|---|---|
| Index | Unique product identification number |
| Product | Product name and description |
| Category | Main product category |
| Sale Price | Actual selling price in INR |
| Market Price | Original market price |
| Type | Product subcategory |
| Rating | Customer rating out of 5 |

### Data Preprocessing

- Checked missing values and duplicate records.
- Converted price and rating columns into numerical formats.
- Calculated discount amount and discount percentage.
- Identified 314 mean-imputed rating values based on the supplied literature review and dataset.
- Excluded these mean-imputed ratings from supervised machine learning evaluation to avoid misleading results.

## 4. Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 5. Exploratory Data Analysis

The following analyses are performed:

- Product category distribution.
- Sale price distribution.
- Market price comparison.
- Discount percentage analysis.
- Customer rating distribution.
- Category-wise average ratings.

## 6. Machine Learning Algorithms

The following algorithms are implemented:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

A Dummy Regressor is also used as a baseline for comparison.

### Model Evaluation Metrics

- **MAE:** Mean Absolute Error.
- **RMSE:** Root Mean Squared Error.
- **R² Score:** Coefficient of Determination.

## 7. Project Results

The models are evaluated using an 80:20 training and testing split.

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Random Forest | 0.4671 | 0.7117 | 0.0001 |
| Dummy Baseline | 0.4851 | 0.7118 | 0.0000 |
| Decision Tree | 0.4603 | 0.7236 | -0.0335 |
| Linear Regression | 0.5217 | 0.8061 | -0.2824 |

**Observation:** Random Forest achieved the lowest RMSE, but its performance was only marginally better than the baseline. This indicates that the available product features have limited predictive power for customer ratings.

## 8. Literature Review Comparison

The project refers to existing research related to:

- Online customer reviews.
- Product rating prediction.
- E-commerce pricing analysis.
- Customer behavior.
- Product recommendations.

The experiment extends this project-level analysis by combining JioMart product prices, discounts, categories, and ratings in one structured dataset.

Since the reviewed studies use different datasets and methods, direct numerical comparison is not possible.

## 9. Project Structure

```text
JioMart-Product-Price-Rating-Analysis/
│
├── data/
│   └── jiomart.csv
│
├── notebooks/
│   └── JioMart_Analysis.ipynb
│
├── outputs/
│   ├── model_evaluation.csv
│   ├── category_analysis.csv
│   ├── cross_validation_results.csv
│   └── visualizations/
│
├── docs/
│   ├── methodology.md
│   └── literature_comparison.md
│
├── README.md
└── requirements.txt
```

## 10. How to Run the Project

1. Download or clone this repository.
2. Open Google Colab.
3. Upload the JioMart dataset.
4. Open the project notebook.
5. Install the required Python libraries.
6. Execute the notebook cells sequentially.
7. View the generated graphs, analysis, and model evaluation results.

## 11. Conclusion

This project analyzes JioMart product pricing, discounts, categories, and customer ratings using data analytics and machine learning.

The results demonstrate that product pricing and category information alone have limited ability to predict customer ratings. Additional information, such as customer reviews, product descriptions, and purchase history, may improve future prediction models.

## 12. Future Enhancements

- Include customer review text for sentiment analysis.
- Explore advanced machine learning algorithms.
- Incorporate product images and additional product information.
- Develop a product recommendation system.
- Use larger datasets for improved analysis and evaluation.

## 13. References

The project uses the ten research papers listed in the supplied JioMart Product Price and Rating Analysis Literature Review.

## Author

**KANNAIAHGARI THARUN**

**USN:** 23BTRCO043
