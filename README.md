 Bank Marketing Purchase Prediction

## 1. Objective
Build a decision tree classifier to predict whether a customer will purchase a product or service (subscribe to a term deposit) based on their demographic and behavioral data.

## 2. Dataset
Bank Marketing Dataset (UCI Machine Learning Repository)

## 3. Tasks Performed
* Loaded the dataset using Pandas with the appropriate separator (`sep=';'`)
* Checked dataset information (`df.info()`) and structural dimensions
* Handled categorical variable formatting by converting text objects into numerical formats using `LabelEncoder`
* Handled dataset class imbalance using a stratified train-test split (`test_size=0.2`, `stratify=y`)
* Built and trained a `DecisionTreeClassifier` with regularized constraints (`max_depth=4`) to prevent overfitting
* Evaluated model predictions using Accuracy, Precision, Recall, and F1-Scores via a `classification_report`
* Extracted and evaluated relative feature importance rankings to understand key classification drivers

## 4. Visualizations
* **Confusion Matrix Heatmap**: A visual matrix showing the exact distribution of true positives, true negatives, false positives, and false negatives.
* **Feature Importance Bar Chart**: A clean bar chart ranking which customer attributes (e.g., duration, age, campaign) had the highest impact on the model's predictions.

## 5. Key Insights
* The model achieved an overall accuracy of **~91.58%**, proving highly reliable at identifying baseline non-purchasers.
* **Call Duration** was revealed to be the single most influential predictive feature; the longer a customer stays on a marketing call, the exponentially higher their likelihood of purchasing the product.
* Because the dataset is naturally imbalanced (far fewer people say "Yes" to bank offers), tracking precision and recall for the purchase class is far more insightful than looking at overall accuracy alone.

## 6. Tools Used
* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## 7. Author
Monika Mohandule
