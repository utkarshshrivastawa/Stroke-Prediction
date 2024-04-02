# Stroke-Prediction

## Library Imports: 
The script starts by importing necessary Python libraries for data manipulation, visualization, machine learning, and oversampling to handle imbalanced datasets.

## Data Loading and Initial Exploration: 
The stroke dataset is loaded from a CSV file, followed by basic explorations such as displaying the first few rows, checking for null values, and examining the dataset's structure.

## Preprocessing:

1. Irrelevant columns like 'id' are dropped.
2. The 'gender' column is cleaned by replacing 'Other' with 'Female'.
3. Missing values in the 'bmi' column are imputed with the median of the 'bmi' values.
4. The dataset's numeric attributes ('bmi', 'avg_glucose_level', 'age') are scaled using StandardScaler to bring them to the same scale.
6. Dummy variables are created for categorical attributes to prepare the data for machine learning models.

## Oversampling: 
Given the imbalance in the dataset (only 4.9% of instances have a stroke), the minority class is oversampled using RandomOverSampler to balance the dataset for better model performance.

## Data Visualization: 
Various visualizations are created to explore the relationship between different attributes and the target variable 'stroke'. This includes pie charts, bar graphs, and count plots for gender distribution, work type, smoking status, residence type, and more.

## Model Training:
A Random Forest Classifier is trained on the oversampled dataset. The model's accuracy is evaluated using a test set and further validated through k-fold cross-validation to ensure its reliability and robustness.

## Model Evaluation: 
The trained model's performance is assessed through accuracy metrics, and a confusion matrix is plotted to understand its true positives, false positives, false negatives, and true negatives.

## Sample Prediction: 
The script demonstrates how to use the trained model to make a prediction based on manually inputted feature values, providing a practical example of how the model can be applied for stroke prediction.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or create a pull request.
