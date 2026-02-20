# Mall Customer Segmentation: Unsupervised Learning 🛍️

This project focuses on **Customer Segmentation** using the K-Means Clustering algorithm. By grouping customers based on their annual income and spending habits, businesses can design targeted marketing strategies to increase engagement and revenue.

## 📌 Project Overview

In this analysis, we explore a dataset of mall customers (https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python From Udemy's Machine Learning A-Z course.) to identify distinct "Personas." Unlike supervised learning, we do not have a pre-defined target; instead, we allow the data to reveal its own natural groupings through mathematical proximity.

## 🛠️ Tech Stack

* **Languages:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib
* **Algorithm:** K-Means Clustering

## 🚀 Key Features & Methodology

* **Exploratory Data Analysis (EDA):** Visualized distributions of Age, Income, and Spending Scores to check for skewness and outliers.
* **Data Preprocessing:** Implemented **Standard Scaling** to ensure that features with larger numerical ranges (Income) did not disproportionately influence the distance-based algorithm.
* **The Elbow Method:** Calculated the **Within-Cluster Sum of Squares (WCSS)** for  values 1 through 10 to identify the "elbow" point, determining that **5 clusters** was the optimal number for this dataset.
* **Cluster Profiling:** Computed the mean attributes of each cluster to define clear business archetypes.

## 📊 Final Customer Segments

Our model identified 5 distinct types of shoppers:

| Cluster | Persona | Description | Strategy |
| --- | --- | --- | --- |
| **0** | **Standard Class** | Average income and average spending. | Reliable shoppers; use standard advertising. |
| **1** | **VIP Class** | High income and high spending. | Focus on luxury, exclusivity, and loyalty rewards. |
| **2** | **Impulsive** | Low income but high spending (mostly younger). | Use "Gen-Z" social media marketing and flash sales. |
| **3** | **Picky Shoppers** | High income but very low spending. | Needs a reason to buy; focus on quality and status. |
| **4** | **Budget Shoppers** | Low income and low spending. | Focus on "Value for Money" and bulk discounts. |

## 📂 Repository Structure

* `customer.ipynb`: The complete Jupyter Notebook including EDA, Elbow Method, and final visualizations.
* `Mall_Customers.csv`: The dataset containing CustomerID, Gender, Age, Annual Income, and Spending Score.

## 💻 How to Run

1. Clone the repository.
2. Install dependencies:
```bash
pip install pandas scikit-learn seaborn matplotlib

```


3. Open `customer.ipynb` and run all cells to reproduce the clusters and analysis.
