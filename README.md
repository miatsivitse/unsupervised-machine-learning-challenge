# unsupervised-machine-learning-challenge


Background:

You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, your supervisor has asked you to explore this possibility by using unsupervised learning.

You have been provided with raw data, so you’ll first need to process it to fit the machine learning models. You will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, you’ll create a visualization to share your findings with your team and other key stakeholders.

Process:

Part 1: Prepare the Data
After uploading imports, I loaded the myopia.csv dataset into a pandas dataframe. Next, I dropped the 'MYOPIC' column and assigned to value x. I also assigned the 'MYOPIC' values to 'labels'.

I then used StandardScaler to stamdardize the data so that columns that contain larger values do not influence the outcome more than columns with smaller values.

Part 2: Apply Dimensionality Reduction

I performed the dimensionality reduction with PCA by inaitilizing the PCA model and getting principal components for the data. 

Then, I further reduced the dataset dimensions with t-SNE and visually inspected the results. To do this, I ran the t-SNE on the principal components and created a scatter plot of the t-SNE output. There do not appear to be any distinct clusters.

Part 3: Perform a Cluster Analysis with K-means
I created an elbow plot to identify the best number of clusters. To accomplish this, I used a for loop to determine the inertia for each k between 1 through 10.

Part 4: Make a Recommendation
After running the K-Means model, The elbow curve does not indicate indicates clear potential clusters. Additionally, the plot generated after running the t-sne indicates there is not a clear seperation of the data to inform the decision to cluster patients together.
