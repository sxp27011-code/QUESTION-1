SREE RAM CHARAN TEJA PUDARI 700762701
# Decision Tree Classifier on Iris Dataset

##  Project Overview
This project demonstrates the use of **Decision Trees** for classification using the famous **Iris dataset**.  
We train models with different `max_depth` values and compare their performance in terms of training and testing accuracy.  
The goal is to understand the concepts of **underfitting** and **overfitting** in decision trees.

---

##  Technologies Used
- Python 3
- scikit-learn
- pandas
- numpy
- matplotlib (optional, for visualization)

---

## Dataset
- **Iris Dataset** (available directly in scikit-learn)
- 150 samples, 4 features (sepal length, sepal width, petal length, petal width), 3 classes (Setosa, Versicolor, Virginica)

---

##  Steps Performed
1. Loaded the Iris dataset from `sklearn.datasets`.
2. Split the dataset into training (80%) and testing (20%) sets using `train_test_split`.
3. Trained **DecisionTreeClassifier** with different `max_depth` values:
   - Depth = 1
   - Depth = 2
   - Depth = 3
4. Evaluated model performance on both training and testing sets.
5. Compared results to discuss **underfitting vs overfitting**.

---

## Results

| Max Depth | Train Accuracy | Test Accuracy |
|-----------|----------------|---------------|
| 1         | ~0.68          | ~0.67         |
| 2         | ~0.95          | ~0.93         |
| 3         | ~0.98          | ~0.97         |

*(Exact numbers may vary depending on train-test split randomization.)*

---

## 🔎 Observations
- **Depth = 1**: Model is too simple → **Underfitting** (poor accuracy on both train & test).
- **Depth = 2**: Balanced performance → captures key patterns without overfitting.
- **Depth = 3**: Very high accuracy, still generalizes well.  
- **Higher depths (not shown)**: Risk of **overfitting** (memorizing training data instead of learning general patterns).

---
