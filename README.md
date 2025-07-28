# Principal Component Analysis (PCA) on Wine Dataset
This project demonstrates the implementation of Principal Component Analysis (PCA) to reduce dimensionality, visualize patterns, and prepare the data for machine learning. PCA is particularly useful for high-dimensional datasets like the Wine dataset used here.

🧠 What is Principal Component Analysis?
Principal Component Analysis (PCA) is a linear dimensionality reduction technique that transforms a dataset into a new coordinate system such that the greatest variance lies on the first axis (called the first principal component), the second greatest variance on the second axis, and so on.

🔸 Why PCA?
Reduces dimensionality while retaining as much variance as possible.

Helps in visualizing high-dimensional data in 2D or 3D.

Removes multicollinearity and noise.

Speeds up training time and reduces overfitting.

📁 Dataset Overview
File Used: wine.csv

Dataset Description:

Contains 13 continuous chemical analysis features of wine samples

Includes a class label Type (1, 2, or 3)

Features include Alcohol, Malic acid, Ash, Magnesium, Phenols, Flavanoids, etc.

🔍 Project Workflow
1. Data Loading and Exploration
Loaded the dataset using pandas

Explored dataset structure with .head(), .info(), .describe()

Checked for missing values and data distribution

2. Preprocessing
Dropped the target variable Type to apply PCA on feature space

Scaled features using StandardScaler to standardize variance across dimensions

3. Applying PCA
Applied PCA using sklearn.decomposition.PCA

Calculated:

Explained Variance

Explained Variance Ratio

Visualized cumulative variance to decide optimal number of components

4. Dimensionality Reduction
Reduced dimensions from 13 to 2 or 3 components for visualization

Plotted 2D scatter plots using principal components to observe clustering patterns

📊 Key Observations
The first few principal components explained the majority of variance in the dataset

2D and 3D plots of principal components showed visible separation between wine classes

PCA helped in feature reduction while preserving essential information

🛠️ Tools & Libraries Used
pandas – data handling

numpy – numeric computations

matplotlib, seaborn – visualization

sklearn.preprocessing.StandardScaler – data scaling

sklearn.decomposition.PCA – dimensionality reduction

📂 Files
PCA.ipynb – Main notebook with full PCA implementation and visualizations

wine.csv – Dataset used for analysis

📌 Takeaways
PCA is a powerful tool to simplify datasets while retaining structure.

It’s useful for visualization, noise reduction, and improving model efficiency.

Always standardize data before applying PCA for meaningful components.
