# Task 04: Dimensionality Reduction & Unsupervised Clustering

## Project Overview
This project demonstrates dimensionality reduction and unsupervised clustering using Python and the Iris dataset. Principal Component Analysis (PCA) reduces the dataset's dimensions, while K-Means groups similar flower measurements into clusters.

## Objectives
- Load and explore a dataset.
- Standardize numerical features.
- Apply Principal Component Analysis (PCA).
- Plot explained variance and cumulative explained variance.
- Use the Elbow Method to help select the number of clusters.
- Calculate and compare Silhouette Scores.
- Visualize clusters in two dimensions using PCA.

## Dataset
The project uses the Iris dataset available through `scikit-learn`.

- **Number of observations:** 150
- **Numerical features:** 4
  - Sepal length
  - Sepal width
  - Petal length
  - Petal width

The flower species labels are not used as inputs for K-Means, so clustering is performed without using the known labels.

## Technologies and Libraries
- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

## Methods Implemented
1. **Standardization:** Scales the four numerical features to a comparable scale.
2. **PCA:** Transforms the original features into principal components.
3. **Scree plot:** Displays the explained variance ratio of each principal component.
4. **Cumulative explained variance plot:** Shows the accumulated variance explained by the components.
5. **Elbow Method:** Compares within-cluster sum of squares for different values of K.
6. **Silhouette Score:** Evaluates how well-separated the resulting clusters are.
7. **K-Means clustering:** Groups observations into clusters.
8. **2D visualization:** Displays cluster assignments using the first two principal components.
9. **Cluster count plot:** Shows the number of observations assigned to each cluster.

## Results
In the notebook output, **K = 2 achieved a Silhouette Score of 0.5818**, the highest score among the tested values shown (K = 2 through K = 10). The notebook also visualizes a three-cluster K-Means solution for comparison.

The best cluster count should be chosen by considering the Silhouette Scores, the Elbow Method, and the purpose of the analysis rather than relying on one metric alone.

## How to Run
1. Install Python and Jupyter Notebook, for example through Anaconda.
2. Open `Dimensionality_Reduction_Clustering.ipynb`.
3. Run this command in a notebook cell if the libraries are not installed:

   ```python
   %pip install pandas numpy matplotlib seaborn scikit-learn
   ```

4. Run the notebook cells from top to bottom.
5. Review the generated plots, scores, and final findings.

## Conclusion
This project demonstrates how PCA can reduce the dimensionality of numerical data and how K-Means can group observations without using known labels. The Elbow Method and Silhouette Score provide complementary ways to assess cluster quality, while PCA plots help visualize the groups in two dimensions.

## Project Files
- `Dimensionality_Reduction_Clustering.ipynb` — notebook containing the code, plots, scores, and conclusion.
- `README_Task_04.md` — project overview and instructions.

## Author
Add your name here.
