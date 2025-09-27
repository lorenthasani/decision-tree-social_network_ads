# Decision Tree Classification on Social Network Ads Dataset

This project implements a Decision Tree Classifier to predict whether a customer will purchase a product based on their age and estimated salary. The model learns patterns in the data to classify new customers into "buy" or "not buy" categories.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Features](#model-features)
- [Results](#results)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The objective of this project is to build a Decision Tree model that can predict customer purchasing behavior using demographic features. Decision trees are particularly useful for this type of classification problem because they:

- Provide interpretable results
- Handle both numerical and categorical features
- Don't require feature scaling
- Can capture non-linear relationships

The dataset used is the "Social Network Ads" dataset, which includes information about users' ages, estimated salaries, and whether they purchased a product.

## Dataset

The dataset (`Social_Network_Ads.csv`) consists of the following columns:

- **User ID**: Unique identifier for each user
- **Gender**: Gender of the user (Male/Female)
- **Age**: Age of the user (numerical)
- **EstimatedSalary**: Estimated salary of the user in USD (numerical)
- **Purchased**: Target variable - whether the user purchased the product (1 for Yes, 0 for No)

### Dataset Statistics
- Total samples: 400 users
- Features: Age and Estimated Salary (primary predictors)
- Target classes: Binary classification (Purchased/Not Purchased)

## Installation

To run this project, ensure you have Python 3.7+ installed along with the following libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### Required Libraries
- `numpy`: For numerical computations
- `pandas`: For data manipulation and analysis
- `matplotlib`: For data visualization
- `seaborn`: For statistical data visualization
- `scikit-learn`: For machine learning algorithms
- `jupyter`: For running the notebook

## Usage

1. **Clone this repository:**
   ```bash
   git clone https://github.com/lorenthasani/decision-tree-social_network_ads.git
   cd decision-tree-social_network_ads
   ```

2. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

3. **Open and run `decision_tree.ipynb`** to explore the complete analysis

4. **The notebook includes:**
   - Data loading and exploration
   - Exploratory Data Analysis (EDA)
   - Data preprocessing
   - Model training and evaluation
   - Visualization of results

## Model Features

### Data Preprocessing
- Handling categorical variables (Gender encoding)
- Feature selection (Age and EstimatedSalary as primary predictors)
- Train-test split for model validation

### Decision Tree Implementation
- **Algorithm**: CART (Classification and Regression Trees)
- **Criterion**: Gini impurity or Entropy
- **Max Depth**: Optimized to prevent overfitting
- **Min Samples Split**: Configured for optimal performance

### Evaluation Metrics
- **Accuracy Score**: Overall model performance
- **Confusion Matrix**: Detailed classification results
- **Precision & Recall**: Class-specific performance
- **F1-Score**: Harmonic mean of precision and recall

## Results

The Decision Tree model achieves strong performance on the Social Network Ads dataset:

- **Training Accuracy**: ~95-98%
- **Test Accuracy**: ~90-93%
- **Key Insights**: 
  - Age and salary are strong predictors of purchase behavior
  - Clear decision boundaries separate buyers from non-buyers
  - Model shows good generalization with minimal overfitting

### Visualizations
- Decision boundary plots for both training and test sets
- Feature importance analysis
- Confusion matrix heatmaps
- ROC curve analysis

## File Structure

```
decision-tree-social_network_ads/
│
├── decision_tree.ipynb          # Main Jupyter notebook with complete analysis
├── Social_Network_Ads.csv       # Dataset file
├── .ipynb_checkpoints/          # Jupyter checkpoint files
└── README.md                    # Project documentation
```

## Key Learning Outcomes

This project demonstrates:
- **Data Science Pipeline**: From raw data to model deployment
- **Classification Techniques**: Binary classification using decision trees
- **Model Evaluation**: Comprehensive performance assessment
- **Data Visualization**: Effective presentation of results
- **Feature Engineering**: Working with demographic data

## Future Improvements

Potential enhancements to consider:
- Hyperparameter tuning using GridSearchCV
- Ensemble methods (Random Forest, Gradient Boosting)
- Cross-validation for more robust evaluation
- Feature engineering (age groups, salary brackets)
- Comparison with other algorithms (SVM, Logistic Regression)

## Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Dataset source: Social Network Ads dataset commonly used for machine learning education
- Built using scikit-learn and other open-source Python libraries
- Inspired by practical applications of decision trees in marketing analytics

---

**Author**: [Lorent Hasani](https://github.com/lorenthasani)  
**Project Link**: [https://github.com/lorenthasani/decision-tree-social_network_ads](https://github.com/lorenthasani/decision-tree-social_network_ads)
