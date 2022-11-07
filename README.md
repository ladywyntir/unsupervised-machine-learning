## Module 20 - unsupervised-machine-learning

### Background
You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, your supervisor has asked you to explore this possibility by using unsupervised learning.

You have been provided with raw data, so you’ll first need to process it to fit the machine learning models. You will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, you’ll create a visualization to share your findings with your team and other key stakeholders.
<hr>

### Code Theory
**Part 1: Prepare the Data.**<br/>
1. Loaded the CSV and displayed the headers
2. Removed the "Myopic" column
3. Standardized the dataset to make it smaller.

**Part 2: Apply Dimensionality Reduction.**<br/>
1. Started up the PCA model
2. Used the pca transformed data variance to see the how varied the components are.
3. **How did the number of features change after performing the dimensionality reduction?**<br/>
The array carries 10 features now instead of 14.<br/>
4. Ran t-SNE to make the dimensions even smaller
5. Printed the dimensions to ensure we were down to 2
6. Set X, y, and the Myopic data and printed the headers to verify
7. Created scatter plots to show X, y and then X/y/Miopic<br/>
![image](/images/Xyscatter.png) 
![image](/images/XyMyopicScatter.png)<br/>
8. **After creating a scatter plot of the t-SNE output, are there distinct clusters?**<br/>
Yes, there seem to be three clusters.<br/>

**Part 3: Perform a Cluster Analysis with K-means.**<br/>
1. Loaded new dataset into a new DF and labeled the columns.
2. Calculated the inertia and range of K values with a for loop.
3. Created and plotted the Elbow curve
4. **If possible, determine where the elbow of the plot is, and at which value of k it appears.**<br/>
The Elbow seems to be at cluster 3 with an inertia of 6000<br/>

**Part 4: Make a Recommendation.**<br/>
**Based on your findings, write up a brief (one or two sentences) recommendation for your supervisor in your Jupyter Notebook. Can the patients be clustered? If so, into how many clusters?**<br/>
I would recommend the patients may be grouped into 3 different clusters.
<hr>


