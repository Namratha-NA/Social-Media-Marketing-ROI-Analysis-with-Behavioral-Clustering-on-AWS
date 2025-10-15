# Social-Media-Marketing-ROI-Analysis-with-Behavioral-Clustering-on-AWS

This project focuses on measuring and optimizing the performance of social media marketing campaigns specifically Facebook and Instagram using a cloud-native analytics pipeline. It includes ROI analysis, funnel metrics, attribution modeling, and KMeans-based user segmentation.

**Use Case**

Businesses struggle to evaluate which marketing channels generate the highest return. This project addresses the problem by analyzing ad performance metrics and user behavior to optimize ad spend and targeting strategies.

**Project Highlights**

-> Platforms Analyzed: Facebook and Instagram

-> Tech Stack: AWS S3, Glue, Athena, SageMaker, Python, SQL, Pandas, Seaborn

**Key Techniques:**

-> ROI computation per platform

-> Funnel analysis by device type

-> First-touch and last-touch attribution

-> KMeans clustering for user segmentation

**Dataset Preparation**

Started with social_media_ad_optimization.csv

Augmented it using Python to simulate ad spend and revenue

Normalized into 3 structured tables:

-> users.csv

-> campaigns.csv

-> customer_journey.csv

**AWS Architecture**

-> Amazon S3: Storage for preprocessed CSVs

-> AWS Glue: Crawled and cataloged CSVs

-> Athena: Queried marketing data with SQL

-> SageMaker Notebook: Visualized data and performed clustering

**Analysis Performed**

1. ROI Calculation

Calculated platform-wise ROI to determine the cost-effectiveness of Facebook and Instagram.

2. Funnel Metrics

Analyzed impressions → clicks → conversions segmented by device type. Computed CTR and CVR.

3. Attribution Models

First-Touch: Identified the first user interaction

Last-Touch: Captured the final ad touch before conversion

4. Demographic Insights

Studied performance across gender, age, and device combinations.

5. Clustering (KMeans)

Segmented users based on engagement patterns and demographics. Identified:

-> High converters

-> Passive viewers

-> High clickers, low converters

**Results**

-> Facebook had ~3.2 ROI, Instagram had ~1.8 ROI

-> Desktop users had 7.4% CVR vs mobile users at 5.2%

-> First-touch attribution favored Facebook; last-touch leaned towards Instagram

-> 3 behavioral user clusters supported targeted campaign strategies


**Future Improvements**

-> Add multi-touch attribution modeling

-> Integrate real-time dashboards via QuickSight

-> Forecast campaign performance with time series models


Folder Structure
|-- data/
|   |-- users.csv
|   |-- campaigns.csv
|   |-- customer_journey.csv
|
|-- scripts/
|   |-- preprocessing.py
|   |-- clustering.py
|
|-- notebooks/
|   |-- SageMaker_Analysis.ipynb
|
|-- Report.pdf
|-- README.md


