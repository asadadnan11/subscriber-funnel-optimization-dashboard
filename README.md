# 📊 Subscriber Funnel Optimization Dashboard

A comprehensive data science project analyzing subscriber behavior and churn patterns for a news platform to optimize the subscriber funnel and improve retention rates.

## 🎯 Project Overview

This project demonstrates end-to-end data science workflow for subscriber funnel optimization, from data generation to predictive modeling and business insights. The analysis focuses on identifying key factors contributing to subscriber churn and developing actionable strategies to improve retention rates across different acquisition channels and subscription tiers.

### Key Objectives

- **Analyze subscriber acquisition channels** and their effectiveness in driving long-term retention
- **Identify factors contributing to subscriber churn** through comprehensive exploratory data analysis
- **Build predictive models** to forecast churn risk with high accuracy
- **Optimize funnel stages** for better conversion rates and reduced churn
- **Generate actionable business insights** for strategic decision-making

## 🔄 Workflow Summary

### 1. Synthetic Data Generation
- Generated 1,000 synthetic subscriber records with realistic behavior patterns
- Included key features: user demographics, acquisition channels, engagement metrics, subscription tiers
- Simulated realistic churn patterns based on engagement and behavioral factors

### 2. Data Preprocessing
- **Feature Engineering**: Created derived metrics (engagement per article, time per article, days since signup)
- **Categorical Encoding**: Label encoded acquisition channels and subscription tiers
- **Data Splitting**: 80/20 train-test split with stratification
- **Feature Scaling**: Standardized numerical features for model optimization

### 3. Exploratory Data Analysis (EDA)
- Comprehensive visualization dashboard analyzing subscriber behavior patterns
- Churn rate analysis by acquisition channel and subscription tier
- Engagement score distributions and correlation analysis
- Funnel stage conversion rate analysis

### 4. Model Development
- **Baseline Model**: Logistic Regression with original features
- **Enhanced Model**: XGBoost with engineered features achieving **18% accuracy improvement**
- Cross-validation and hyperparameter optimization
- Feature importance analysis for business insights

### 5. Funnel Visualization
- Multi-stage funnel analysis (Acquired → Engaged → Active → Loyal → Premium/Enterprise)
- Conversion rate calculation between funnel stages
- Revenue impact assessment for at-risk subscribers

### 6. Data Export for Tableau
- Processed dataset with predictions and confidence scores
- Ready-to-use format for advanced visualization and dashboard creation
- Business-friendly column naming and data structure

## 🛠️ Technologies Used

### Core Libraries
- **Python 3.8+**: Primary programming language
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing and array operations
- **matplotlib**: Static visualization and plotting
- **seaborn**: Statistical data visualization

### Machine Learning Stack
- **scikit-learn**: Machine learning algorithms and preprocessing
- **XGBoost**: Gradient boosting framework for advanced modeling
- **StandardScaler**: Feature scaling and normalization
- **LabelEncoder**: Categorical variable encoding

### Additional Tools
- **Jupyter Notebook**: Interactive development environment
- **datetime**: Date and time manipulation
- **warnings**: Error handling and code optimization

## 📈 Key Outcomes

### Model Performance
- **Baseline Logistic Regression**: Established performance benchmark
- **Enhanced XGBoost Model**: Achieved **18% accuracy improvement** over baseline
- **High Prediction Confidence**: Average confidence score of 85%+
- **Robust Feature Importance**: Clear identification of churn drivers

### Business Insights
- **Channel Performance**: Referral programs show lowest churn rates (15%), while Paid Ads show highest (35%)
- **Engagement Correlation**: Strong negative correlation between engagement scores and churn probability
- **Revenue Impact**: Identified potential monthly revenue at risk from predicted churners
- **Funnel Optimization**: Specific conversion bottlenecks identified for targeted improvement

### Actionable Recommendations
- Scale referral program investments
- Optimize paid advertising targeting strategies
- Implement early warning systems for low-engagement subscribers
- Develop tier-specific retention campaigns
- Deploy real-time churn prediction monitoring

## 📁 Project Structure

```
subscriber_funnel_optimization_dashboard/
├── subscriber_funnel_optimization_dashboard.ipynb  # Main analysis notebook
├── subscriber_funnel_data.csv                      # Exported data for Tableau
├── README.md                                       # Project documentation
└── requirements.txt                                # Python dependencies (if needed)
```

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

### Running the Analysis
1. Clone or download the repository
2. Open `subscriber_funnel_optimization_dashboard.ipynb` in Jupyter Notebook
3. Run all cells sequentially to reproduce the analysis
4. The processed data will be exported to `subscriber_funnel_data.csv` for Tableau visualization

## 📊 Visualization Examples

The notebook includes comprehensive visualizations:
- **Funnel Analysis Charts**: Multi-stage conversion visualization
- **Churn Rate Comparisons**: By acquisition channel and subscription tier
- **Engagement Distributions**: Retained vs. churned subscriber patterns
- **Model Performance Metrics**: ROC curves, confusion matrices, feature importance
- **Revenue Impact Analysis**: Financial implications of churn predictions

## 🔍 Model Details

### Feature Engineering
- **Interaction Features**: Engagement × time ratios, articles × engagement combinations
- **Risk Indicators**: Binary flags for low engagement, activity, and tenure
- **Composite Scores**: Weighted engagement metrics for holistic subscriber health

### XGBoost Configuration
- **Hyperparameters**: Optimized for balanced precision and recall
- **Cross-Validation**: 5-fold validation for robust performance estimation
- **Feature Selection**: Top predictive features identified through importance scoring

## ⚠️ Important Disclaimer

**This project uses entirely synthetic data generated for educational and demonstration purposes.** 

- All subscriber data, behavioral patterns, and business metrics are artificially created
- The dataset does not represent any real news platform or actual subscriber base
- Model performance and business insights are simulated for learning objectives
- Results should not be used for actual business decision-making without real data validation

The synthetic data is designed to mimic realistic patterns found in subscription-based businesses, making it valuable for educational purposes and methodology demonstration.

## 🤝 Contributing

This project is designed as a portfolio demonstration and educational resource. Suggestions for improvements or additional analysis approaches are welcome through issues or pull requests.

## 📄 License

This project is available for educational and non-commercial use. Please provide attribution when using or adapting the methodology.

---

**Author**: Data Science Team  
**Date**: December 2024  
**Version**: 1.0 