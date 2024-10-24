
# **Predictive Maintenance for Healthcare Equipment**

## **Project Overview**
This project aims to predict equipment failures in healthcare facilities by analyzing various operational metrics like usage hours, temperature, vibration levels, and maintenance history. Using machine learning models, this project provides a way to implement predictive maintenance strategies, reducing downtime and maintenance costs.

## **Dataset**
The dataset used for this project is `healthcare_equipment_data.csv` (or the Excel version `healthcare_equipment_data.xlsx`). It contains the following features:

- **equipment_id**: Unique ID for each equipment.
- **usage_hours**: Number of hours the equipment has been used.
- **temperature**: Operating temperature of the equipment (in degrees).
- **vibration_level**: Vibration intensity level of the equipment.
- **pressure_level**: Operating pressure level.
- **last_maintenance**: Hours since the last maintenance.
- **failure**: Binary target variable indicating if a failure occurred (1 = Yes, 0 = No).

## **Project Files**

- **notebook.ipynb**: Jupyter notebook containing the complete code for data preprocessing, visualization, model building, and evaluation.
- **healthcare_equipment_data.csv**: The CSV file containing the dataset (mock data provided).
- **healthcare_equipment_data.xlsx**: The Excel version of the dataset (optional).
- **README.md**: This file, providing an overview of the project.

## **Steps in the Jupyter Notebook**

### 1. **Import Libraries**
- The notebook begins by importing necessary libraries like `pandas`, `numpy`, `matplotlib`, `seaborn`, and machine learning tools from `sklearn`.

### 2. **Data Loading and Exploration**
- The dataset is loaded using `pd.read_csv()` or `pd.read_excel()`.
- Initial data exploration includes checking the structure of the dataset (`.info()`, `.describe()`), handling missing values, and visualizing feature distributions.

### 3. **Data Visualization**
- Histograms and correlation heatmaps are generated using `matplotlib` and `seaborn` to explore feature relationships.

### 4. **Data Preprocessing**
- Handling missing values, encoding categorical features (if applicable), and splitting the dataset into training and testing sets.
- Features are standardized using `StandardScaler()` to normalize data for machine learning models.

### 5. **Model Building**
- A **Random Forest Classifier** is used for the predictive task.
- The model is trained on the training set, and predictions are made on the test set.

### 6. **Model Evaluation**
- The model is evaluated using a confusion matrix, accuracy score, and a classification report. These metrics help assess the model's performance in predicting equipment failures.

### 7. **Feature Importance**
- Feature importance is plotted to understand the impact of each feature on the prediction of failures.

### 8. **Conclusion**
- A summary of the model's performance is provided, along with insights into which factors are most critical in predicting equipment failures.

## **How to Use This Project**

1. **Clone the repository** or download the files.
   
2. **Install dependencies**:
   Ensure that you have the required Python libraries installed. You can install them using the following command:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. **Run the Jupyter Notebook**:
   - Open the `notebook.ipynb` file in a Jupyter environment and run the cells step-by-step.
   - You can use either the CSV or Excel version of the dataset by changing the appropriate file path in the `pd.read_csv()` or `pd.read_excel()` functions.

## **Requirements**

- Python 3.x
- Jupyter Notebook
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

## **Conclusion**

Predictive maintenance is crucial for reducing equipment downtime and improving reliability in healthcare settings. By analyzing operational data, this project demonstrates how machine learning can be used to predict equipment failures, allowing for more efficient maintenance scheduling.

