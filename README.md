# Customer Segmentation Using K-mean Clustering 

*Customer Segmentation is the process of dividing the customers of an enterprise into different groups(or clusters) based on shared characteristics such as demographics, purchasing habits, spending habits or preferences.*

**Objective**: This segmentation helps in understanding the customers of an enterprise to help business grow, tailor marketing strategies and improve sales.

**Dataset Description:** The dataset contains the following columns

**Customer_id:** Unique identifier for each customer.

**Gender:** Gender of the customer (e.g., Male/Female).

**Age:** Age of the customer.

**Annual_income:** Annual income of the customer in some currency.

**Spending_score:** A score (typically 1–100) indicating the customer’s spending behavior

**Process:**

**1.Data Collection:** The Data has been collected directly from Kaggle. 

**2.Loading and Exploring:**
	a. The dataset is loaded into pandas dataframe. 
	b. Basic Data Exploration like analyzing first 10 rows, renaming the columns names into simpler ones has been done. 

**3.Pre-Processing:**
	a. Missing values are checked. 
	b. Standardization of numerical values like age, annual_income and spending score to produce best results and no one feature dominates the result. 

**4.Exploratory Data-Analysis**
	a. Gender Distribution: Females is observed to be the maximum number of customers. 
	b. Spending_score - Gender: Females Spending score founds to be more than males. 
	c. Age Distribution: Maximum customers are found to be in the age group of 30-35 and minimum in 60+ age group.
	d. Annual_income - Spending_score: Maximum customers whose spending_score is between 40-60 there age lies between 40-70. 

**5.Feature Engineering:** This is done to create meaningful insights for the segementation
	a. Selected Features are Age, Annual_income, Spending_score.

**6.Determining optimal clusters**
	a. Elbow-Method is used to determine optimal number of clusters.

**7.K-means Clustering** 
	a. K-means Clustering is applied and the model is trained with the optimal numbers of cluster determined from elbow method. 
	b. Each cluster was assigned a label(0,1,2,3).

**8.Visualization**
	a. The cluster data points are visualized in a scatter plot. 
	b. The First plot shows the relationship between AGE and SPENDING SCORE for each cluster. 
	c. The Bar graph shows the Average Spending Score for each cluster. Highest Spending score was found to be by cluster 1 where the age mean is found to be 30 and most common gender
	founds to be female. 