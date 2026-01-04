# 💳 Credit Card Customer Segmentation (PCA & K-Means)

**Author:** Shokoufeh Naseri  
**Year:** 2024  

## Project Overview
This project applies **unsupervised learning** to segment credit card customers based on usage behavior.
Using **Principal Component Analysis (PCA)** and **K-Means clustering**, it identifies meaningful customer groups that support **marketing, risk analysis, and business strategy**.

---

## Dataset
- Source: Kaggle – CC GENERAL Dataset  
- ~9,000 active credit card holders  
- 18 behavioral features (purchases, balance, cash advances, payments)

---

##  Data Preparation
- Median imputation for missing values  
- Removed non-numeric identifier (`CUST_ID`)  
- Standardized numeric features  
- Removed highly correlated variables  

---

## Dimensionality Reduction (PCA)
- Reduced features from **17 → 10**
- First **6 principal components explain 83% of variance**
- Improved representation after removing correlated features

---

## Clustering (K-Means)
- Optimal clusters selected using **Elbow Method**
- **K = 3** customer segments identified:

**Cluster 1 – Loan-Oriented Users**  
High balance and cash advances, low full payment rate  

**Cluster 2 – Active Spenders**  
High purchase frequency, low balance and cash advance  

**Cluster 3 – Low-Usage Users**  
Minimal activity across all features  

---

## Key Takeaways
- Removing correlated variables improves PCA performance  
- PCA + K-Means produces clear, interpretable segments  
- Results support customer profiling and targeted strategies  

---

## Tools & Technologies
- **R**
- PCA
- K-Means Clustering
- Unsupervised Learning
- Data Visualization

---

## How to Run This Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/shokoufehnaseri/credit-card-customer-segmentation.git

2. **Install required R packages**

## Install Required R Packages

```r
install.packages(c(
  "factoextra",
  "corrplot",
  "ggplot2",
  "dplyr",
  "gridExtra"
))
```
3. **Download the dataset**

 - Download CC GENERAL.csv from Kaggle

 - Place it in the project directory

4. **Run the analysis**

 - Open the .Rmd file in RStudio

 - Click Knit to generate the HTML report


## Project Type
Unsupervised Learning | Customer Segmentation | Data Analytics

