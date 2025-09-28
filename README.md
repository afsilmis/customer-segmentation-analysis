# Customer Personality Analysis for Enhanced Marketing Campaigns

## Description

This project analyzes customer data to identify distinct personality segments and inform targeted marketing strategies. By understanding the unique behaviors and preferences of different customer groups, we can move from a one-size-fits-all approach to personalized campaigns that boost engagement, conversion rates, and ROI.

This analysis identified four key customer segments and provides data-driven recommendations to optimize marketing spend and strategy for each.

## Problem Statement

The company's marketing efforts were inefficient due to a lack of detailed customer segmentation, leading to poorly targeted campaigns with low conversion rates. This generalized approach resulted in suboptimal resource allocation and difficulty in identifying and catering to high-value customer segments.

## Objectives

The primary goal is to leverage data insights to drive personalized marketing strategies, thereby increasing customer engagement and revenue. The key objectives include:

  * Identifying distinct customer segments based on demographics and shopping behavior.
  * Understanding the product and channel preferences for each identified segment.
  * Developing tailored marketing recommendations for each customer group.

## Key Insights

### Customer Demographics

  * The customer base is predominantly Gen X, aged 35-50, with a university degree.
  * Most customers have a monthly income of IDR 50-60 million and typically have two family members.
  * Despite high purchasing power, spending on shopping is minimal, accounting for only 0.01% of income.

### Spending Behavior

  * **Presence of Children:** Customers without children spend, on average, six times more than customers with children.
  * **Income Levels:** High-income customers are stable premium spenders, while low-income customers, though mostly frugal, have the most high-spending outliers.
  * **Product Categories:** Sales are heavily concentrated, with "Coke" (50.2%) and "Meat Products" (27.6%) accounting for nearly 78% of total sales.
  * **Purchase Channels:** Offline stores are the most popular channel (39.0%), followed by the web (27.5%). There is a strong synergy between web, catalog, and store channels.

## Methodology

### 1\. Data Preparation

  * **Data Cleaning:** Handled missing values by imputing with column medians and removed duplicate entries.
  * **Feature Engineering:** Created new features such as `Age`, `Is_Parent`, `Total_Spent`, and `Online_Purchase_Ratio` to enrich the dataset.
  * **Data Transformation:** Mapped categorical variables and applied one-hot encoding. Scaled numerical features using `RobustScaler` for modeling.

### 2\. Dimensionality Reduction

  * Principal Component Analysis (PCA) was used to reduce dimensionality. It was found that 2 components could capture 90% of the variance in the dataset, allowing for effective visualization and efficient modeling.

### 3\. Clustering

  * Several clustering algorithms were explored, including K-Means, Agglomerative Clustering, DBSCAN, and Gaussian Mixture Models (GMM)[cite: 185].
  * The optimal number of clusters was determined to be four using the Elbow Method[cite: 182].
  * **Final Model:** K-Means was selected as the final model due to its efficiency, scalability, and clear centroid-based representation, making it suitable for production environments. The model achieved a Silhouette Score of 0.62.

## Results: Customer Segments

Four distinct customer clusters were identified:

| Cluster | Segment Name | Key Characteristics |
| :--- | :--- | :--- |
| **Cluster 3** | **Priority Customers** | Middle-aged, high income, selective high spenders with a strong preference for shopping in-store. They favor sweet products and gold items. |
| **Cluster 0** | **Promo Seekers** | Middle-aged, often with children, low income, and minimal spending. They are highly responsive to promotions and browse online frequently but have low conversion rates. |
| **Cluster 2** | **Affluent Selectives** | The oldest segment, with upper-middle income and moderate spending. They respond well to campaigns, are active online, and prefer Coke and meat products. |
| **Cluster 1** | **Frugal Families** | The largest segment, middle-aged and mostly childless, with the highest income but focused on affordability. They are heavy purchasers of Coke and gold items. |

## Strategic Recommendations

Based on the segment analysis, the following strategies are recommended:

  * **Priority Customers:** Nurture this high-value group with exclusive loyalty programs, early access to new products, and personalized offers to enhance their loyalty.
  * **Promo Seekers:** Engage this deal-driven segment with frequent discounts, "Buy 1 Get 1" offers, bundled packages, and a point-based loyalty program.
  * **Affluent Selectives:** Focus marketing on product quality and uniqueness rather than discounts. Utilize content marketing, such as healthy recipes, to build a connection.
  * **Frugal Families:** Retain this large segment by offering essential products at fair prices, with family packs and bulk discounts to encourage repeat purchases.

## Potential Impact

Targeted implementation of these strategies is projected to significantly increase revenue:

  * A **5%** increase in spending from **Frugal Families** could generate an additional **\~58.2 million** in revenue.
  * A **20%** increase from **Promo Seekers** could add **\~32 million** in revenue.
  * A **15%** increase from **Priority Customers** could result in an additional **\~20 million** in revenue.
  * A **10%** increase from **Affluent Selectives** could yield an extra **\~3 million** in revenue.

## Get in Touch

  * **Email:** afsilmis@gmail.com 
  * **LinkedIn:** https://www.linkedin.com/in/az-zukhrufu-fi-silmi-suwondo
  * **Source Code:** https://github.com/afsilmis/customer-segmentation-analysis
