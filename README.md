## Algorithms and Big Data in Chemistry and Material Science project

#### Short description:
In this repository you can find the main .ipynb file, which consist of answers to a few question we were asking during this course, and the initial dataset as .csv file.
___

#### Wide description:

1. Perform each data cleansing step (validation, handling of missing values, detection of outliers, handling of duplicates, data transformation and normalization). Each step is shown with a code and is accompanied by a text box explaining the step performed on it.

On the first sted we checked the data for the missing values, detected and deleted the outliers, delete the duplicates and normalized data.

2. Using chemical libraries, complete the dataset with molecule descriptors. Describe the descriptors you have chosen.

On this point we complite our dataset with new features using two chemical libraries (Mordred and RDkit) by using their API. The dataset became 20236 rows × 1348 columns from innitial 20236 rows × 14 columns.

3. Make a visual analysis of the data and its distribution. Create at least 3 different types of statistical graphs to analyze the data. Draw conclusions and explain why these graphs are useful for analyzing data. 

On this step we creating some visualization instruments like box-plots, distribution graphs, violin plots and the pairplot. For making all this graphs more readable we applied PCA method to decrease out dimentionality. Number of features decreased from 1348 to 19.

4. Calculate correlation coefficients for your dataset and investigate multicollinearity. Visualize and interpret your results.

Here we created a heatmap with Pearson coefficients to look for some multicollinearity if it is present. As we can see all our features are independent.

5. Select the dataset parameters using the correlation coefficients from the last step with the limit you have chosen. Which descriptors have fallen out of the dataset and why?

Based on the coefficients calculated above and the constructed heatmap with built-in Pearson coefficients, we can conclude that there is no multicollinearity in the 19 descriptors obtained by the PCA method (from the 1300+ previously present). It follows from this that we can use all the received descriptors in the future.
