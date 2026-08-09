\# Project 03 — Customer Segmentation Using Unsupervised Learning



\## DecodeLabs Data Science Internship — Batch 2026



\### Project Overview



This project focuses on customer segmentation using unsupervised machine learning techniques.



The objective is to analyze customer demographic, purchasing, campaign-response, and engagement-related data and discover meaningful customer groups without using predefined target labels.



The project applies data preprocessing, feature standardization, Principal Component Analysis (PCA), K-Means clustering, the Elbow Method, and Silhouette Score analysis to identify and evaluate customer segments.



The resulting clusters are then interpreted as actionable business personas that can support customer targeting and marketing decisions.



\---



\## Objectives



The main objectives of this project are:



\- Explore and understand customer data.

\- Identify missing values and duplicate records.

\- Analyze numerical and categorical variables.

\- Prepare features for machine learning.

\- Standardize numerical features.

\- Apply Principal Component Analysis (PCA).

\- Reduce the high-dimensional feature space into a smaller number of dimensions.

\- Determine the optimal number of K-Means clusters.

\- Evaluate cluster quality using the Elbow Method and Silhouette Score.

\- Perform K-Means customer segmentation.

\- Analyze the characteristics of each customer cluster.

\- Translate the identified clusters into actionable business personas.



\---



\## Dataset



The dataset contains customer-related information covering:



\- Demographic characteristics

\- Household information

\- Income

\- Product purchasing behavior

\- Deal and store purchases

\- Website activity

\- Campaign responses

\- Customer engagement



The dataset contains \*\*2,240 customer records and 29 variables\*\* before preprocessing.



The data was prepared and transformed during the analysis to make it suitable for clustering.



\---



\## Technologies and Libraries



The project was developed using Python and Jupyter Notebook.



\### Libraries Used



\- Pandas

\- NumPy

\- Matplotlib

\- Seaborn

\- Scikit-learn

\- Jupyter Notebook



\---



\## Project Workflow



\### 1. Data Loading



The customer dataset was loaded into a Pandas DataFrame and its basic structure was examined.



\### 2. Exploratory Data Analysis



The dataset was inspected using:



\- Dataset shape

\- Column names

\- Data types

\- First few records

\- Statistical summaries

\- Categorical value distributions



\### 3. Data Quality Assessment



The dataset was checked for:



\- Missing values

\- Duplicate records

\- Data inconsistencies

\- Categorical variable distributions



Missing values were identified and handled before model development.



\### 4. Feature Preparation



Relevant customer demographic, purchasing, campaign-response, and engagement variables were selected for clustering.



Categorical variables were converted into numerical representations where required.



\### 5. Feature Standardization



Numerical features were standardized before applying distance-based clustering algorithms.



This step is important because customer variables exist on different numerical scales.



\### 6. Principal Component Analysis



Principal Component Analysis (PCA) was applied to reduce the dimensionality of the prepared dataset.



The reduced representation makes the high-dimensional customer data easier to analyze and visualize while retaining important information from the original features.



\### 7. Determining the Optimal Number of Clusters



Two evaluation techniques were used:



\#### Elbow Method



The Within-Cluster Sum of Squares (WCSS) was calculated for different values of K.



The resulting curve was examined to identify the point where additional clusters provided diminishing improvements.



\#### Silhouette Score



Silhouette Scores were calculated for different cluster counts to evaluate how well customers were separated into distinct groups.



Both methods were considered when selecting the final number of clusters.



\### 8. K-Means Clustering



K-Means clustering was applied to segment customers into groups based on their similarities across the prepared feature space.



The final model assigned each customer to a cluster.



\### 9. Cluster Analysis



The resulting clusters were analyzed by examining:



\- Cluster size

\- Average income

\- Recency

\- Product spending

\- Purchase behavior

\- Website activity

\- Campaign responses

\- Overall customer engagement



\### 10. Business Persona Development



The statistical characteristics of each cluster were translated into practical customer personas.



These personas provide a business-oriented interpretation of the mathematical clusters and can help support targeted marketing strategies.



\---



\## Key Results



The final clustering analysis identified \*\*two major customer segments\*\*.



\### Cluster 0



This segment represents a larger customer group with comparatively lower average income and substantially lower spending across the analyzed product categories.



Customers in this group also show relatively lower purchasing activity and campaign response levels.



\### Cluster 1



This segment represents a smaller but higher-value customer group.



Customers in this cluster have substantially higher average income and significantly higher spending across multiple product categories.



They also demonstrate stronger purchasing activity, campaign engagement, and customer interaction.



\---



\## Business Interpretation



The clustering results indicate a clear difference between the two identified customer segments.



\### Persona 1 — Lower-Value / Less Engaged Customers



Characteristics:



\- Lower average income

\- Lower product spending

\- Lower purchasing activity

\- Lower campaign response

\- Relatively lower engagement



Possible business strategy:



\- Promotional offers

\- Discount campaigns

\- Re-engagement campaigns

\- Product recommendations

\- Personalized incentives



\### Persona 2 — High-Value Customers



Characteristics:



\- Higher average income

\- Higher product spending

\- Higher purchasing activity

\- Stronger campaign response

\- Greater customer engagement



Possible business strategy:



\- Premium offers

\- Loyalty programs

\- Cross-selling

\- Upselling

\- Personalized product recommendations

\- VIP customer campaigns



\---



\## Visualizations



The project includes visualizations for:



\- Feature distributions

\- Feature standardization comparison

\- Elbow Method

\- Silhouette Score

\- Cluster analysis

\- Customer segment distribution

\- PCA-based cluster visualization



The generated figures are stored in the project's `images` directory.



\---



\## Project Structure



```text

Project\_03\_Customer\_Segmentation/

│

├── Project\_03\_Customer\_Segmentation.ipynb

├── customer\_personality\_analysis.csv

├── clustered\_customer\_segments.csv

├── requirements.txt

├── README.md

│

└── images/

&#x20;   ├── before\_after\_standardization.png

&#x20;   ├── elbow\_method.png

&#x20;   ├── silhouette\_scores.png

&#x20;   ├── cluster\_distribution.png

&#x20;   └── pca\_clusters.png

