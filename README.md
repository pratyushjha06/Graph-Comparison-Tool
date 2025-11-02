# 🧠 Graph Comparison Tool — Fraud & Legit Transaction Analysis

## 📘 Project Overview

The **Graph Comparison Tool** is a Python-based analytical project that visualizes and compares the structure of two transaction networks — **Legitimate** and **Fraudulent** — using the **Elliptic Bitcoin Dataset**.  
It aims to detect structural differences between fraud and non-fraud transaction graphs by applying **network analysis** techniques such as centrality, clustering, and degree distribution.

This project demonstrates how **graph theory** and **data science** can be combined to identify potential fraud patterns within large-scale financial networks.

---

## ⚙️ Tech Stack

- **Language:** Python  
- **Libraries Used:**  
  - `pandas` — data handling  
  - `networkx` — graph creation and analysis  
  - `matplotlib` — data visualization  
  - `numpy` — numerical operations  
  - `scikit-learn` — support for statistical analysis  
- **Environment:** Google Colab or Jupyter Notebook

---

## 🗂 Dataset

- **Dataset Used:** [Elliptic Bitcoin Transaction Dataset]([elliptic_txs_edgelist.csv - Google Drive](https://drive.google.com/file/d/1Fu4wmLDHHl-z6TXaTeiC21IH3-XQ-QfP/view?usp=sharing))
- **Description:**  
  Contains directed transaction edges (`txId1`, `txId2`) representing the flow of Bitcoin between wallets.  
  The dataset also includes labels marking transactions as **Legit (1)** or **Fraud (2)**.

---

## 🧩 Project Workflow

### **Step 1: Setup Project Directory**

Create the project folder and install required libraries.

### **Step 2: Load Dataset**

Download the dataset from Google Drive and verify its structure.

### **Step 3: Data Exploration**

Check column names, missing values, and sample data.

### **Step 4: Build Graph**

Use `networkx.from_pandas_edgelist()` to construct a transaction graph.

### **Step 5: Visualization**

Display a random 600-node subgraph using a spring layout for visual clarity.

### **Step 6: Split Graphs**

Divide the dataset into **Legit** and **Fraud** subgraphs based on transaction labels.

### **Step 7: Compute Graph Metrics**

Calculate:

- Number of Nodes  
- Number of Edges  
- Graph Density  
- Average Clustering Coefficient  
- Average Degree  

### **Step 8: Centrality Analysis**

Compute **degree centrality** and plot its distribution for both graphs.  
This helps identify the most influential (highly connected) nodes.

### **Step 9: Compare Metrics**

Display and visualize structural differences between the two graphs using bar plots.

---

## 🚀 How to Run

1. Open **Google Colab**.
2. Upload the notebook or copy the code cells.
3. Run cells step-by-step.
4. Choose whether to save metrics (local or Google Drive).
5. View visual outputs and CSV results.

---

## 🎯 Objectives

- Compare Legitimate and Fraudulent transaction graphs.
- Analyze graph structure, connectivity, and centrality.
- Detect distinctive fraud patterns using graph metrics.

---

#### 📈 Final Graph Metrics Comparison Results

| Metric         | Legit Transactions Graph | Fraud Transactions Graph |
| -------------- | ------------------------ | ------------------------ |
| Nodes          | 101,884                  | 101,885                  |
| Edges          | 58,856                   | 58,431                   |
| Density        | 0.000011                 | 0.000011                 |
| Avg Clustering | 0.006328                 | 0.005687                 |
| Avg Degree     | 1.155353                 | 1.146999                 |

### **Observations**

- Legit graph has **slightly higher clustering and connectivity**, implying more trusted relationships.
- Fraud graph is **less interconnected**, showing more isolated and sparse patterns.
- Both graphs are **extremely sparse**, typical for blockchain networks.

---

## 🧑‍💻 Author

**Project By:** Pratyush Jha (13718002724) 

                     Khushi Kumari (14318002724) 

                     Aayush Kumar Jha (14418002724)

                     Sunidhi Singh (14918002724)

---

## 🧾 Contributions Summary

| Member               | Contributions                                                                                              |
| -------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Sunidhi Singh**    | Imported and preprocessed dataset, handled data cleaning, built the initial NetworkX graph from edgelist.  |
| **Pratyush Jha**     | Implemented metric functions, performed graph metric and centrality analysis, and designed visualizations. |
| **Khushi Kumari**    | Compared Legit vs Fraud metrics, created comparative charts, and assisted in visual interpretation.        |
| **Aayush Kumar Jha** | Analyzed results, interpreted differences between graphs, and prepared the final documentation and report. |

---

## 📚 References

1. [GeeksforGeeks — NetworkX Tutorials](https://www.geeksforgeeks.org/python-networkx-tutorial/)  
2. [Javatpoint — Python Libraries](https://www.javatpoint.com/python-tutorial)  
3. [NetworkX Documentation](https://networkx.org/documentation/stable/)  
4. [Matplotlib Official Docs](https://matplotlib.org/stable/contents.html)  
5. [Elliptic Dataset Info](https://www.kaggle.com/ellipticco/elliptic-data-set)  
6. [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)

---

## 🏁 Conclusion

This project effectively demonstrates the use of **graph theory** for identifying fraudulent behavior in financial networks.  
By comparing two transaction graphs — Legit vs Fraud — the system highlights clear structural differences that can aid in **cybersecurity and financial risk analysis**.






