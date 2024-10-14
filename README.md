# Titanic Survival Prediction Pipeline

## Predicting Survival on the Titanic

### History
The sinking of the Titanic remains one of the most tragic maritime disasters in history. On April 15, 1912, the Titanic, a British passenger liner, collided with an iceberg during its maiden voyage, leading to the deaths of 1502 out of 2224 passengers and crew members on board. The incident revealed various societal dynamics, as survival rates differed significantly based on factors such as gender, age, and social status. For example, women, children, and individuals from the upper-class had higher chances of survival compared to others. By analyzing these attributes, we can make predictions about who might have survived the disaster.

### Goals
The objective of this project is to develop a Machine Learning pipeline that processes the Titanic dataset, engineers relevant features, and predicts the likelihood of a passenger’s survival based on factors like:
- Gender
- Age
- Passenger class (social status)
- Fare paid
- Family size
- Port of embarkation, etc.

### File Structure
- `titanic_survival_pipeline.py`: This script contains the code for building, training, and evaluating the machine learning model for predicting survival on the Titanic.

### Steps in the Pipeline
1. **Data Loading**: Load the Titanic dataset (typically available from Kaggle).
2. **Data Preprocessing**:
   - Handle missing values (e.g., for age and embarked port).
   - Feature encoding (e.g., converting categorical variables like gender to numerical form).
   - Feature scaling for numerical columns such as fare.
3. **Feature Engineering**:
   - Create new features from existing data (e.g., family size from `SibSp` and `Parch`).
   - Group ages into bins for easier prediction.
4. **Model Building**: 
   - Choose and train a machine learning model (e.g., Logistic Regression, Random Forest, etc.).
   - Use cross-validation to ensure the model's reliability.
5. **Model Evaluation**:
   - Evaluate the model using metrics like accuracy, precision, recall, and F1-score.
   - Tune hyperparameters using techniques such as grid search.

### Requirements
To run this pipeline, you will need the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

You can install the necessary packages using the following command:

```bash
pip install -r requirements.txt
```

### Instructions for Running
1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the Titanic dataset from Kaggle (if necessary) and place it in the `data/` directory.
4. Run the `titanic_survival_pipeline.py` script:
   ```bash
   python titanic_survival_pipeline.py
   ```

### Output
- The script will output a trained machine learning model.
- It will also display model evaluation metrics such as accuracy and confusion matrix.

### Conclusion
This project not only builds a predictive model for Titanic survival but also provides insights into how different societal factors influenced survival rates during the disaster. By analyzing these trends, we gain a glimpse into the priorities and privileges that shaped the outcome of one of the most infamous tragedies in history.

