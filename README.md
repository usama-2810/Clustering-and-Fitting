# Effects of Alcohol on Student Performance

This project analyzes a student survey dataset to explore relationships between academic performance, social habits, and other factors. It utilizes various data visualization techniques and machine learning algorithms to gain insights from the data.

## Functionality

* **Data Loading and Cleaning**
    * Loads data from a provided URL using pandas (https://pandas.pydata.org/docs/).
    * Renames columns for clarity.
    * Handles missing values (if necessary) using scikit-learn's SimpleImputer (https://scikit-learn.org/stable/modules/impute.html).
* **Visualization**
    * Creates different plots using seaborn (https://seaborn.pydata.org/) to visualize relationships in the data:
        * Relational graphs (scatter plots) to explore relationships between variables (e.g., Overall GPA vs. Number of Drinks).
        * Categorical graphs (bar charts) to compare data across categories (e.g., Socializing Behavior by Gender).
        * Statistical graphs (heatmaps) to visualize correlations between numeric variables (e.g., correlation between GPA and number of drinks).
* **Clustering (KMeans)**
    * Groups students into clusters based on their overall GPA and number of drinks (features) using the KMeans algorithm from scikit-learn.
* **Fitting (Linear Regression)**
    * Fits a linear regression model using scikit-learn's LinearRegression to predict the number of drinks based on a student's overall GPA.
* **Additional Relationship Exploration**
    * Creates visualizations to explore other potential relationships within the data beyond the initial focus on GPA and drinks.

## Code Quality

* The code adheres to PEP-8 style guidelines for improved readability and maintainability.
* Separate functions with docstrings are used for each visualization type, ensuring clear and modular code.
* Each function generates only one plot, promoting clarity and organization.

## Machine Learning Techniques

This project incorporates two machine learning techniques for exploratory analysis:

* **KMeans Clustering:** This unsupervised learning algorithm groups data points (students) into clusters based on their similarities (e.g., similar GPA and number of drinks). The code includes functionality to perform clustering, but further exploration to determine the optimal number of clusters can be implemented using metrics like the silhouette score.
* **
