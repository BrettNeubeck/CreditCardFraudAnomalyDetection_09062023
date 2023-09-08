# CreditCardFraudAnomalyDetection_09062023
Anomaly Detection Practice On Credit Card Fraud Using SMOTE

This project serves as a comprehensive demonstration of anomaly detection techniques applied to a credit card fraud dataset. In the realm of machine learning, unbalanced datasets present a prevalent challenge, characterized by a significant disparity in the number of instances between different classes. This disparity often results in a skewed model performance, wherein the algorithm exhibits a preference for the majority class while striving to minimize overall error.

To effectively tackle this issue, various methodologies have been developed, with minority oversampling and majority undersampling being prominent strategies. These techniques are routinely leveraged to rectify dataset imbalances, enhancing the model's capacity to precisely classify instances belonging to the minority class.

**Minority Oversampling:**
In minority oversampling, the goal is to increase the representation of the minority class by generating synthetic instances. One prominent method for this purpose is the Synthetic Minority Over-sampling Technique (SMOTE). SMOTE works by creating synthetic samples for the minority class by interpolating between existing data points. It selects a minority instance, identifies its k nearest neighbors, and generates new instances along the line segments connecting the chosen instance to its neighbors. This effectively augments the minority class and helps balance the dataset.

**Majority Undersampling:**
On the other hand, majority undersampling involves reducing the number of instances in the majority class to match the minority class. This can be done randomly or through more sophisticated techniques that carefully select instances to maintain the dataset's representativeness.

**Challenges with Measurement:**
Evaluating models trained on imbalanced datasets poses its own set of challenges. Traditional metrics like ROC AUC (Receiver Operating Characteristic Area Under the Curve) may not be the most appropriate choice in such cases because they can be overly optimistic. ROC AUC evaluates a model's ability to discriminate between classes across different thresholds, which can lead to inflated performance scores when the dataset is imbalanced.

**Brier Score Loss:**
Instead of ROC AUC, the Brier Score Loss is a more suitable metric for evaluating models on imbalanced datasets. The Brier Score measures the mean squared difference between the predicted probabilities and the actual outcomes. It rewards models for assigning high probabilities to the true positive instances, making it sensitive to class imbalance.

**Confusion Matrix:**
In addition to the Brier Score, the confusion matrix is a valuable tool for assessing model performance on unbalanced datasets. It breaks down the model's predictions into categories like true positives, true negatives, false positives, and false negatives, providing a clearer picture of how well the model is performing for each class. Metrics like precision, recall, and F1-score can be derived from the confusion matrix, offering a more balanced view of the model's accuracy across classes.

In summary, unbalanced datasets are a common challenge in machine learning, and addressing this issue through techniques like SMOTE, majority undersampling, and appropriate evaluation metrics like the Brier Score Loss and the confusion matrix is crucial for building models that perform well on imbalanced data, especially when ROC AUC is not suitable due to class imbalance.
