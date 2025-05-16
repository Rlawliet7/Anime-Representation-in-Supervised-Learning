![Uploading image.png…]()



# 🧠 CatBoost vs Random Forest: A Supervised Learning Battle Inspired by Jujutsu Kaisen

This project presents a comparative study between two powerful supervised learning algorithms—CatBoostClassifier and RandomForestClassifier—through a narrative lens inspired by the anime *Jujutsu Kaisen*. Just as Gojo Satoru and Ryomen Sukuna fight for dominance, this project pits CatBoost and Random Forest against each other in a series of machine learning experiments.

## 🔍 Project Motivation

In supervised learning, model selection and optimization play a key role in achieving high performance. This project draws an analogy between:
- **CatBoost** as **Gojo Satoru** – naturally dominant, powerful without much tuning.
- **Random Forest** as **Ryomen Sukuna** – potential hidden until fully awakened through tuning.

The aim is to highlight not only the raw power of default model settings but also how fine-tuning can drastically affect performance.

## 📊 Methodology

- **Datasets**: 4 real-world datasets were used.
- **Conditions**: Each dataset was tested in two versions:
  - **D1**: Original dataset (with potential outliers).
  - **D2**: Cleaned dataset (outliers removed via IQR method).
- **Split**: 80% training, 20% testing.
- **Models**:
  - CatBoostClassifier (default parameters).
  - RandomForestClassifier (default and tuned versions).
- **Tuning**:
  - Manual tuning of `n_estimators`, `max_depth`, and `min_samples_split`.
  - Additional exploration of `random_state` to test Random Forest's sensitivity.
- **Metrics**:
  - **Accuracy**
  - **F1-Score**

## ⚔️ Results

- **CatBoost** consistently performed better in default settings, showing strength in both raw and cleaned datasets.
- **Random Forest**, while initially behind, matched or outperformed CatBoost after careful hyperparameter tuning.
- `random_state` significantly influenced Random Forest performance and should not be overlooked.

## 📈 Key Insights

- **CatBoost** is highly efficient with minimal preprocessing.
- **Random Forest** requires more effort to unleash its full potential.
- Hyperparameter tuning can bridge performance gaps, especially in ensemble methods.
- The choice of model depends not only on default power but also on willingness to optimize.

## 📚 Requirements

- Python 3.7+
- `pandas`
- `numpy`
- `matplotlib`
- `catboost`
- `scikit-learn`

Install dependencies with:

```bash
pip install -r requirements.txt
