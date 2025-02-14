# 📌 SDSC3002: Apriori Algorithm Optimization

## 🔍 Overview
This repository contains an **Apriori algorithm implementation** for **frequent itemset mining**, developed as part of the **SDSC3002 Data Mining** course assignment. 

The goal is to:
- Find **frequent itemsets** in a dataset using the **Apriori algorithm**.
- Implement an **acceleration technique** to improve performance.
- Compare the execution time of the **original** vs. **optimized** methods at different **minimum support** thresholds.

---

## 📂 Repository Structure
```
📁 SDSC3002_Apriori_Optimization/
│── 📄 README.md                # Project documentation
│── 📄 requirements.txt         # Required Python dependencies
└── 📄 Apriori_Implementation.ipynb # Jupyter Notebook (Original & Optimized)
```

---

## 🚀 Getting Started

### 1️⃣ Install Dependencies
Ensure you have Python installed, then install the required libraries using:

```bash
pip install efficient-apriori
```

If you are using Jupyter Notebook, install it within the notebook:

```python
!pip install efficient-apriori
```

### 2️⃣ Run the Notebook
Open the Jupyter Notebook:

```bash
jupyter notebook Apriori_Implementation.ipynb
```

### 3️⃣ Required Imports
Ensure the following libraries are imported in your Python code:

```python
from time import process_time
import pandas as pd
import numpy as np
from efficient_apriori import apriori, itemsets_from_transactions
```

---

## ⚡ Performance Comparison
| Min Support | Original Time (s) | Optimized Time (s) | Improvement (s) |
|------------|------------------|------------------|----------------|
| 0.0001     | 26.2             | 14.9             | **11.3**       |
| 0.0002     | 14.3             | 8.5              | **5.8**        |
| 0.0003     | 10.3             | 5.8              | **4.5**        |
| 0.0004     | 8.2              | 4.8              | **3.4**        |
| 0.0005     | 7.2              | 4.0              | **3.2**        |


The optimized Apriori method **significantly reduces execution time** while identifying **more frequent patterns**.

---

## 📊 Key Findings
- The acceleration method improved execution time by **28.2 seconds** in the general case.
- Performance gains were **higher at lower minimum support levels** (e.g., **11.3s faster at 0.0001**).
- The optimized method found **more frequent patterns** compared to the original.

---

## 📜 License
This project is for academic purposes and follows an **open-source MIT License**.
