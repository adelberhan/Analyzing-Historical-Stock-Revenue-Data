# Analyzing-Historical-Stock-Revenue-Data

This project analyzes Tesla's stock and revenue data, providing insights through data visualization and analysis.

## 📌 Requirements
Ensure you have the following dependencies installed before running the project:

### **🔹 Required Packages**
- `pandas` (For data manipulation)
- `matplotlib` (For data visualization)
- `seaborn` (For enhanced plotting)
- `numpy` (For numerical operations)
- `requests` (For fetching data from APIs)
- `jupyter` (If running in a Jupyter Notebook)

To install all dependencies, run:
```sh
pip install pandas matplotlib seaborn numpy requests jupyter
```

## 🚀 How to Run the Project

### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

### **2️⃣ Open the Jupyter Notebook**
If using Jupyter Notebook, run:
```sh
jupyter notebook
```
Then open the file `Final Assignment-v2.ipynb` and execute the cells.

### **3️⃣ Run the Python Script**
If you prefer running a Python script, create a new file (e.g., `main.py`) and add:
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np

# Load the data
tesla_revenue = pd.read_csv('tesla_revenue.csv')

# Clean and process data
tesla_revenue["Revenue"] = tesla_revenue["Revenue"].str.replace(r'[,|$]', '', regex=True).astype(float)

# Plot data
plt.figure(figsize=(10,5))
sns.lineplot(data=tesla_revenue, x='Date', y='Revenue')
plt.title("Tesla Revenue Over Time")
plt.show()
```
Then run:
```sh
python main.py
```

## 📊 Features
- Data cleaning and preprocessing
- Revenue trend visualization
- Stock price vs. revenue correlation analysis

## 🤝 Contributing
Feel free to submit pull requests to improve the project!

## 📝 License
This project is open-source under the MIT License.

