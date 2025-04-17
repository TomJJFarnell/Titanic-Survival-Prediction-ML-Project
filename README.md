🚢 Titanic Survival Prediction – Ensemble Modeling Approach

In this notebook, we tackle the classic Titanic survival prediction problem using a structured and model-driven approach. Rather than relying on a single algorithm, we compare multiple machine learning models and ultimately combine them through ensembling to improve accuracy and generalization.

⸻

🧠 Key Steps in This Notebook:

🧹 Data Cleaning & Feature Engineering
	•	Extracted meaningful features such as Title, FamilySize, IsAlone, and CabinLetter
	•	Encoded categorical variables using label encoding
	•	Handled missing values (e.g., imputing Age and Fare with the mean)

🤖 Model Training

Trained and evaluated three high-performing tree-based models:
	•	Random Forest – A classic ensemble of decision trees using bagging
	•	XGBoost – A gradient boosting model optimized for speed and performance
	•	HistGradientBoosting (HGB) – A fast, histogram-based gradient boosting algorithm built into scikit-learn

🔗 Model Ensembling (Stacking)

After comparing the performance of individual models, we combined them using a stacking ensemble:
	•	The predictions of the base models (Random Forest, XGBoost, and HGB) were fed into a Logistic Regression meta-model
	•	This stacked model learned to leverage the strengths of each base learner to produce a final prediction

📤 Final Prediction & Submission
	•	Trained the ensemble model on the full training dataset
	•	Predicted outcomes on the test set
	•	Submitted results in the required format for the Titanic Kaggle competition
✅ Current best accuracy: ~75%

⸻

🔍 What’s Next

To improve the accuracy score, I’ve been researching other approaches and plan to refine this solution in a future notebook. Specifically:
	•	Use MICE imputation for more accurate handling of missing data (instead of mean imputation or dropping rows)
	•	Switch to One-Hot Encoding to simplify categorical variable handling
	•	Focus on a single strong model, most likely Random Forest, to reduce complexity and boost interpretability

