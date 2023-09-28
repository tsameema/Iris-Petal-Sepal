# Iris Dataset Clustering using K-Means
## Introduction
This project demonstrates the application of the K-Means clustering algorithm to the well-known Iris dataset. The main objectives are to determine the optimal number of clusters for the data and visually represent the clustered data points along with the centroids. This project was completed as part of The Sparks Foundation Internship Program under the Data Science & Business Analytics track.

## Task Description
The project follows a series of steps to achieve the clustering of the Iris dataset:

1. **Importing Libraries**
   
In this step, we import the necessary Python libraries required for data analysis, visualization, and K-Means clustering. Libraries used include pandas, sklearn.datasets, sklearn.cluster, and matplotlib.pyplot.

2. **Importing Dataset**

The Iris dataset is loaded using sklearn.datasets.load_iris(). It is then converted into a DataFrame for easier data manipulation. The dataset contains information about sepal and petal dimensions of three different Iris species.

3. **Data Preprocessing**

Data preprocessing involves checking for missing values and handling them if any are found. In this project, missing values are replaced with the mean of the respective columns using df.fillna(df.mean()).

4. **The Elbow Method**

The Elbow Method is used to determine the optimal number of clusters for the K-Means algorithm. It involves fitting K-Means to the data for a range of cluster numbers and plotting the sum of squared distances (inertia) for each number of clusters. The "elbow point" in the graph indicates the optimal number of clusters. In this project, the elbow point is found to be 3.

5. **Prediction based upon optimal number of clusters**

A K-Means model is created with the optimal number of clusters, which is 3 in this case. The KMeans class from sklearn.cluster is used for this purpose. The fit_predict method is used to cluster the data points based on the chosen number of clusters.

6. **Data Visualization**

The clustered data points and centroids are visualized using matplotlib. Different colors are assigned to different clusters to distinguish them visually. The scatter plot is created with sepal length on the x-axis and sepal width on the y-axis.

## Technologies Used
1. Python: The programming language used for data analysis and visualization.
2. Libraries:
    - pandas: Used for data manipulation and handling DataFrames.
    - sklearn.datasets: Used to load the Iris dataset.
    - sklearn.cluster: Used for implementing the K-Means clustering algorithm.
    - matplotlib.pyplot: Used for creating data visualizations.
## How to Run the Code
1. Ensure you have Python installed on your machine.
2. Install the required libraries using pip:

        pip install pandas scikit-learn matplotlib
3. Clone this GitHub repository or download the project files.
   
         git clone https://github.com/tsameema/Iris-Petal-Sepal.git
4. Open and run the Jupyter Notebook or Python script provided in the repository.

Feel free to expand on this README by adding more details, such as the project's objectives, results, and any additional visualizations or insights you gained from the analysis. Additionally, you can include information about the dataset itself and any relevant citations or references.
