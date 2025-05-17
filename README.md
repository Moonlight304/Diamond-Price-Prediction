# 💎 Diamond Price Prediction

A polynomial regression model to predict diamond prices based on their features.  
Implemented from scratch using NumPy and optimized using the Adam optimizer.

---

## 📊 Dataset

This project uses the [Diamonds Dataset](https://www.kaggle.com/datasets/shivam2503/diamonds) from Kaggle, which contains:

- Carat (weight)  
- Cut, Color, Clarity (categorical)  
- Dimensions: x, y, z (length, width, depth in mm)  
- Table and Depth percentages  
- Price in USD  

---

## ⚙️ Features

- One-hot encoding for categorical features  
- Normalization of features and target variable  
- Polynomial feature expansion (degree 3)  
- Regression implemented from scratch using:
  - Gradient Descent  
  - Adam Optimizer  
  - L2 Regularization
- 5-fold cross-validation  

---

## 🚀 How to Use

1. Clone the repo:
    ```bash
    git clone https://github.com/Moonlight304/Diamond-Price-Prediction.git
    cd Diamond-Price-Prediction
    ```

2. Download `diamonds.csv` from Kaggle and place it in the root folder.

3. Install dependencies:
    ```bash
    pip install numpy pandas scikit-learn matplotlib
    ```

4. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

5. Open and run `main.ipynb`.

---

## 📈 Results



```
Average across 5 folds:
  Mean Mean Squared Error : 406228.34
  Mean Mean Absolute Error : 352.00
  Mean R² Score  : 0.9744
```

![Mean Squared Error curve](image.png)

- The model achieves an R² score of around **97%** on the test set. 
- Training loss decreases smoothly with Adam optimizer.
- Comparable performance to sklearn’s Polynomial Regression (approx 97.1%).

---


## Future Work

- Experiment with higher polynomial degrees or other regression methods.

- Build a user interface to input diamond attributes and get price predictions.

---

## License

MIT License
