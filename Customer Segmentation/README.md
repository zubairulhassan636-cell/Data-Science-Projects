# Project 3 — Unsupervised Learning (Customer Segmentation)
**DecodeLabs Data Science Internship | Batch 2026**

## 📌 Overview
Yeh project ek complete **unsupervised learning pipeline** implement karta hai jo unlabeled
retail customer data mein hidden mathematical groupings discover karta hai aur unhe
actionable business **personas** mein translate karta hai.

## 🎯 Goal
Distance-based algorithms (K-Means) use karke retail data mein customer segments dhoondna —
bina kisi labeled target ke, sirf behavioral aur demographic patterns ke through.

## 🧱 IPO Architecture
| Step | Technique | Purpose |
|------|-----------|---------|
| 1. Scale | `StandardScaler` | Sab features ko equal mathematical voting power dena |
| 2. Compress | `PCA` | 23 features ko 95% variance retain karte hue kam dimensions mein reduce karna |
| 3. Cluster | `K-Means` + Elbow Method + Silhouette Score | Optimal K mathematically prove karna aur clusters banana |
| 4. Translate | Inverse Transform + Business Rules | Clusters ko real-world Personas mein convert karna |

## 📂 Files
- `Project3_Customer_Segmentation.ipynb` — Main notebook (fully executed, sab outputs/plots ke sath)
- `retail_customers.csv` — Input dataset (1200 customers, 23 unlabeled behavioral/demographic features)
- `customer_segments_labeled.csv` — Output: har customer ke sath Cluster number + Persona label
- `persona_summary.csv` — Har cluster ka average profile + recommended business action

## 📊 Dataset
Synthetic retail dataset (aap isay apne real dataset se replace kar sakte hain — pipeline
same rahega):
- Demographics: Age, Gender
- Financial: Annual Income, Loyalty Points
- Behavioral: Spending Score, Purchase Frequency, Recency, Tenure, Online Ratio, Basket Size,
  Cart Abandon Rate, Discount Usage, Returns Rate
- Engagement: Email Open Rate, App Sessions, Wishlist Items, Social Engagement, Referrals
- Category Spend: Electronics, Fashion, Grocery, Travel

## 🧩 Results
Pipeline ne **K = 4** optimal clusters mathematically prove kiye (Elbow Method + Silhouette
Score dono se confirm), jo 4 meaningful personas mein translate hue:

| Persona | Profile | Recommended Action |
|---------|---------|---------------------|
| **High-Value Trendsetters** | High Income + High Spending | Exclusive perks, early access, experiential marketing |
| **Affluent Conservatives** | High Income + Low Spending | High-touch support, warranties, loyalty programs |
| **Budget-Conscious Explorers** | Low Income + High Spending | Influencer campaigns, flash sales, buy-now-pay-later |
| **Conservative Minimizers** | Low Income + Low Spending | Minimize spend, clear price-value, basic utility |

## 🛠️ Key Skills Demonstrated
- Dimensionality reduction (PCA)
- K-Means clustering
- Distance metrics & standardization
- Elbow Method + Silhouette Score for cluster validation
- Reverse-engineering PCA/Scaler transforms (inverse_transform)
- Business intelligence translation (data → persona → action)

## ▶️ How to Run
1. `pip install pandas numpy matplotlib seaborn scikit-learn kneed`
2. Open `Project3_Customer_Segmentation.ipynb` in Jupyter
3. Run all cells top to bottom
4. To use your own dataset: replace `retail_customers.csv` and update `feature_cols`
   in the notebook accordingly

---
*Batch 2026 | Powered by DecodeLabs*
