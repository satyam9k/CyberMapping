# User Behavior Analysis Project

This project focuses on analyzing user behavior patterns using machine learning techniques. It processes data from multiple users, trains classification models, and evaluates their performance in identifying users based on their behavior.

## Table of Contents
1. [Dependencies](#dependencies)
2. [Data Preparation](#data-preparation)
3. [Feature Selection](#feature-selection)
4. [Model Training](#model-training)
5. [Model Evaluation](#model-evaluation)
6. [Results Visualization](#results-visualization)
7. [Prediction on New Data](#prediction-on-new-data)

## Dependencies

The project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install these dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Data Preparation

1. The script reads CSV files for 5 different users (`User0_BEHACOM.csv` to `User4_BEHACOM.csv`).
2. It selects 1100 random rows from each user's data.
3. The data from all users is combined into a single DataFrame.

## Feature Selection

The script selects 25 features related to user behavior, including:
- Keystroke patterns
- Word usage statistics
- Application usage metrics
- System resource utilization

## Model Training

Two models are trained on the prepared data:
1. Logistic Regression
2. Random Forest Classifier

The data is split into training (80%) and testing (20%) sets, and features are scaled using StandardScaler.

## Model Evaluation

The models are evaluated using the following metrics:
- Accuracy
- Precision
- Recall
- F1 Score

## Results Visualization

The script generates several visualizations:
1. Bar plots comparing the performance metrics of both models.
2. Confusion matrices for both models.

## Prediction on New Data

The trained models are used to predict user identities on a new dataset (`test_data.csv`). The predictions from both models are printed and compared with the actual user identities.

## Usage

To run the analysis:

1. Ensure all dependencies are installed.
2. Place the user data CSV files in the same directory as the script.
3. Run the script in a Jupyter notebook or Python environment.
4. Review the output, including performance metrics and visualizations.

## Note

This project is for educational and research purposes only. Ensure you have the necessary permissions to use and analyze user behavior data.
