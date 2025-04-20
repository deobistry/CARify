
# 🚗 Used Car Price Prediction Web App

This is an interactive web application for predicting the **resale price of used cars** based on multiple attributes. Built with **Streamlit**, **scikit-learn**, and other powerful Python libraries, it uses machine learning models to estimate a car's value accurately.

---

## 📌 Key Features

- 🧠 **Machine Learning Models**
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
  - Best model is automatically selected based on RMSE

- 🧹 **Data Preprocessing**
  - Cleans pricing and distance-driven columns
  - Removes outliers based on domain knowledge
  - Combines brand and model into `BrandModel` for feature enrichment

- 📊 **Interactive Dashboard**
  - Select brand, model, fuel type, ownership type, etc.
  - Get instant prediction based on user input
  - Visualize actual vs predicted car prices

- 📈 **Evaluation Metrics**
  - RMSE (Root Mean Square Error)
  - MAE (Mean Absolute Error)
  - R² Score

---

📷 Screenshots
---

![alt image](https://github.com/deobistry/CARify/blob/main/Screenshot%20(40).png)
![alt image](https://github.com/deobistry/CARify/blob/main/Screenshot%20(41).png)

---


## 🧠 Tech Stack

| Layer       | Tools & Libraries |
|-------------|-------------------|
| Frontend    | Streamlit         |
| Backend     | Python            |
| ML Models   | scikit-learn      |
| Data        | pandas, numpy     |
| Visuals     | matplotlib, seaborn |

---

## 📂 Project Structure

```
.
├── car_price_prediction_2.py      # Main Streamlit application
├── used_car_dataset.csv           # Dataset used for training
├── actual_vs_predicted.png        # Visual output (generated)
├── README.md                      # Documentation (you are here)
```

---

## 💻 Installation and Running the App

### 🧾 Requirements

- Python 3.7 or above

### 📦 Install Dependencies

```bash
pip install pandas numpy scikit-learn streamlit matplotlib seaborn
```

### ▶️ Launch the App

```bash
streamlit run car_price_prediction_2.py
```

This will open the app in your default browser at `http://localhost:8501`.

---

## 📊 Dataset Description

Dataset: `used_car_dataset.csv`

| Column Name  | Description                          |
|--------------|--------------------------------------|
| Brand        | Car manufacturer (e.g., Hyundai)     |
| model        | Specific car model                   |
| Year         | Manufacturing year                   |
| Age          | Age of the car in years              |
| kmDriven     | Total kilometers driven              |
| Transmission | Type of transmission (Manual/Auto)  |
| Owner        | Ownership status (First/Second etc.) |
| FuelType     | Type of fuel used                    |
| AskPrice     | Price at which the car is listed     |

---

## 🧪 How It Works

1. **Load Data**: Reads `used_car_dataset.csv`
2. **Clean Data**: Cleans currency symbols, removes NA, filters outliers
3. **Train Models**: Trains 3 different ML models
4. **Evaluate Models**: Selects the best based on RMSE
5. **User Prediction**: User enters car info → model predicts price
6. **Visualization**: Scatter plot of Actual vs Predicted prices

---

## 🌐 Future Enhancements

- 🔧 Save/Load trained models (joblib)
- ☁️ Deploy on Streamlit Cloud or Heroku
- 📬 Allow users to submit new car entries
- 📈 Add analytics and model comparison dashboard

---

## 🪪 License

This project is licensed under the **GNU General Public License v3.0**.

You are free to:
- Share — copy and redistribute the material
- Adapt — remix, transform, and build upon it

Under the following terms:
- Attribution — You must give appropriate credit.
- ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license.
- NonCommercial — Not applicable for commercial use without permission.

See [LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) for full details.

---

## 👤 Author

**Divyanshu Bansal**  
B.Tech CSE | Data Science Enthusiast  
[GitHub](#) | [LinkedIn](#)

---

> Made with ❤️ using Streamlit and scikit-learn
