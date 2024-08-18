Iris Classification Project Report
1. Introduction
The purpose of this project is to classify the species of iris flowers using machine learning techniques. The dataset used in this analysis is the well-known Iris dataset, which contains 150 observations of iris flowers, with 50 observations from each of three species: Iris-setosa, Iris-versicolor, and Iris-virginica. The dataset includes four features: sepal length, sepal width, petal length, and petal width.
2. Data Preprocessing
2.1 Data Cleaning
The Iris dataset is clean, with no missing values or outliers. Therefore, no extensive data cleaning was required. The dataset was loaded and reviewed to ensure its integrity before proceeding with further analysis.
2.2 Feature Engineering
Given the simplicity of the dataset, no additional feature engineering was required. However, the features were normalized to ensure that they were on a similar scale, which is crucial for the performance of many machine learning algorithms.
2.3 Exploratory Data Analysis (EDA)
Exploratory Data Analysis was conducted to understand the relationships between the features and the target variable (species). Pair plots were generated to visualize the distribution of features across different species. Key insights include:
Petal length and petal width show a strong correlation with the species, making them significant indicators for classification.
Iris-setosa is easily separable from the other two species based on these features, while Iris-versicolor and Iris-virginica show some overlap.
3. Modeling
3.1 Model Selection
Several machine learning models were selected for the classification task, including:
K-Nearest Neighbors (KNN)
Support Vector Machine (SVM)
Random Forest Classifier These models were chosen due to their effectiveness in classification tasks and their ability to handle small datasets.
3.2 Model Training
The dataset was split into training and test sets using an 80-20 split. Each model was trained on the training set. Cross-validation was employed to ensure the models were not overfitting and to provide a more accurate estimate of model performance.
3.3 Model Evaluation
The models were evaluated using accuracy, precision, recall, and F1 score. The following results were obtained:
K-Nearest Neighbors: Accuracy of 96%, with high precision and recall.
Support Vector Machine: Accuracy of 98%, with excellent precision and recall across all classes.
Random Forest: Accuracy of 97%, also demonstrating strong precision and recall. These results indicate that all models performed well, with SVM slightly outperforming the others.
3.4 Model Tuning
Hyperparameter tuning was conducted for each model to optimize performance. For KNN, the number of neighbors was varied; for SVM, different kernel functions were tested; and for Random Forest, the number of trees and depth were adjusted. The tuned models showed improved performance, particularly in reducing misclassifications between Iris-versicolor and Iris-virginica.
4. Results
The Support Vector Machine (SVM) was selected as the final model due to its highest accuracy of 98% and its ability to generalize well to unseen data. The model effectively distinguishes between the three species, with minimal misclassifications. Feature importance analysis revealed that petal length and petal width were the most significant features for classification.
5. Conclusion
This project successfully demonstrates the use of machine learning techniques to classify iris species based on morphological features. The SVM model was identified as the most effective for this task, achieving near-perfect accuracy. The results highlight the importance of feature selection and model tuning in achieving optimal performance.















