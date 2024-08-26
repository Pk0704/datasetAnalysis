This project leverages supervised and unsupervised machine learning techniques to analyze a dataset containing songs from Spotify aswell as socioeconomic factors of respondents. 
The goal is to uncover insights into the factors that influence song popularity and understand the relationships between various musical features.


Data Description
The dataset includes multiple features related to songs, such as:

Duration
Danceability
Energy
Loudness
Speechiness
Acousticness
Instrumentalness
Liveness
Valence
Tempo

Data Preprocessing:

Feature Selection: Specific features like 'duration', 'danceability', 'energy', etc., are targeted for analysis.
Imputation: Missing values are replaced with the mean of respective features to maintain dataset integrity.
Scaling: Features are standardized to have a mean of zero and a standard deviation of one, which is crucial for models like PCA and logistic regression that assume normally distributed data.
Principal Component Analysis (PCA):

Used to reduce dimensionality while capturing most variability in the data. This helps in visualizing high-dimensional data and can improve model efficiency and interpretability.
Statistical Testing and Visualization:

Histograms, scatter plots, and bar plots are employed to visualize distributions and relationships between features.
Pearson and Spearman correlation analyses assess linear and rank correlations between variables like 'popularity' and 'duration'.
Mann-Whitney U tests examine differences in distributions between groups, such as the popularity of explicit versus non-explicit songs.
Predictive Modeling:

Random Forest Regressor: Utilized to predict song popularity based on various features. The effectiveness of each feature is evaluated using the R² metric, which measures the proportion of variance in the dependent variable predictable from the independent variable.
Logistic Regression: Applied for binary classification tasks like predicting whether a song is in a major or minor key based on 'valence', a measure of musical positiveness.
Cross-Validation:

Used to estimate the model's performance and its variability, ensuring that the model is generalizable and not just fitted to a particular subset of data.
Feature Importance:

Examined through techniques like permutation importance to understand which features contribute most to predicting song popularity.
Advanced Statistical Methods:

ANOVA and Tukey's HSD tests identify whether differences in song popularity across different musical keys are statistically significant.


Tools Used
Python: Main programming language.
Pandas & NumPy: For data manipulation and numerical calculations.
Matplotlib & Seaborn: For data visualization.
Scikit-learn: For machine learning and statistical modeling.
SciPy: For advanced statistical functions.
