# 🏠 Housing Price Prediction Using Deep Learning

## 🎯 Objective
Build a Neural Network that predicts the **median house price** of a California district based on demographics, location, and housing features.

---

## 📊 Dataset
**California Housing Dataset** — a classic real-world regression dataset.

| Property | Detail |
|----------|--------|
| Source | `housing.csv` |
| Total Records | 20,640 rows |
| Features | 8 input features |
| Target | Median House Value (`MedHouseVal`) |
| Train Set | 16,512 rows (80%) |
| Test Set | 4,128 rows (20%) |

### 📋 Features Used

| Feature | Description |
|---------|-------------|
| `MedInc` | Median income of the district |
| `HouseAge` | Average age of houses |
| `AveRooms` | Average number of rooms |
| `AveBedrms` | Average number of bedrooms |
| `Population` | Population of the district |
| `AveOccup` | Average house occupancy |
| `Latitude` | Geographic location |
| `Longitude` | Geographic location |

---

## 🧠 Model Architecture

| Layer | Details |
|-------|---------|
| Input | 8 features |
| Dense | 64 neurons, ReLU activation |
| Dense | 64 neurons, ReLU activation |
| Output | 1 neuron (predicted house price) |

---

## ⚙️ Tech Stack
- Python
- TensorFlow / Keras
- Pandas
- Scikit-learn (StandardScaler, train_test_split)
- Matplotlib
- Google Colab

---

## 🔍 Key Concepts Used
- **StandardScaler** → Normalizes all features to the same scale for better learning
- **ReLU Activation** → Helps the model learn non-linear patterns
- **MSE Loss** → Measures average squared error between predicted and actual prices
- **Adam Optimizer** → Efficient and adaptive learning rate optimization
- **R2 Score** → Measures how well predictions match actual values (1.0 = perfect)

---

## 📈 Results

| Metric | Score |
|--------|-------|
| Loss (MSE) | 0.2495 |
| MAE | 0.3419 |
| **R2 Score** | **0.81 (81%)** ✅ |

---

## 📉 Visualizations

### 1. Actual vs Predicted House Prices
Compares the model's predicted house prices against the real prices. Points closer to the red line indicate more accurate predictions.

<img width="698" height="547" alt="image" src="https://github.com/user-attachments/assets/d865dddf-14e8-4b40-bc4f-44b88a7e85d2" />


---

### 2. Model Loss Over Epochs
Shows how the model improved with each training cycle. A decreasing loss means the model is learning and getting better over time.

<img width="708" height="470" alt="image" src="https://github.com/user-attachments/assets/5fdfd43a-1bef-468b-a187-131ba5557fb6" />


---

### 3. Feature Correlation with House Price
Displays which features have the most impact on house prices. Higher correlation means that feature influences the price prediction more strongly.

<img width="728" height="470" alt="image" src="https://github.com/user-attachments/assets/97cc42ad-db6d-4a89-b122-13e0e440a5e4" />


---

## 💡 Key Insights
- 🔥 **Median Income (MedInc)** is the strongest predictor of house prices at **~0.70 correlation** — richer neighborhoods = higher prices
- **AveRooms & Latitude** are the next most influential features at ~0.15
- **Population & AveOccup** have very little effect on price
- The model achieves **81% accuracy (R2)** — solid performance for a real-world regression problem
- A few outliers exist where the model struggles, indicating room for further tuning

