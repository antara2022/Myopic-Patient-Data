## Myopic Patient Data
Classify Myopia Patient Data using Unsupervised Machine Learning Models

## Objectives
### Step 1 - Prepare the Data
- Read myopia.csv into a Pandas DataFrame

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/79ee071a-25ed-40a0-8b35-35542171dd56)

- Remove the "MYOPIC" column from the dataset

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/e7c9485e-69cc-42c7-9e90-7d6db7b7425a)

- Standardize the dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values
- Sample Analysis: After examining the initial dataset, there are 15 features present in the data. After removing the "MYOPIC" column from the dataset, there are 14 features.

### Step 2 - Apply Dimensionality Reduction
- Perform dimensionality reduction with PCA

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/40eb87a7-e468-46eb-b36e-b851b4c0c36e)

- Sample Analysis: After performing dimensionality reduction with PCA, there are 10 features in the data. According to the explained variance, we have 92% of the information in the original dataset which is over the desired 90% explained variance.

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/bd128dc4-1803-4ecc-8c0c-4ddc7edf0367)

- Further reduce the dataset dimensions with t-SNE
- Create a scatter plot of the t-SNE output

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/19d43003-6477-49a6-8e26-361c2267e109)

- Sample Analysis: After performing dimensionality reduction with T-SNE, there are five clusters that can be identified.

### Step 3 - Perform a Cluster Analysis with K-means
- Create an elbow plot to identify the best number of clusters

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/7cc10a5c-da46-491a-af1b-14127e1921c5)

- Create a K-means model

![image](https://github.com/antara2022/Myopic-Patient-Data/assets/112270155/10aae9c0-b513-4242-9f36-e54ef364b322)

### Step 4 - Make a Recommendation
- Recommendation: The lowest elbow of the plot occurs at k = 5, indicating that the best number of clusters for the given data is 5. Therefore, it is recommended that the patients be grouped into five clusters.

Contact: antara.choudhury3000@gmail.com
