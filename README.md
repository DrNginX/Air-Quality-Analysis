# Air-Quality-Analysis
Basically, the project is based on the analysis of the air quality index, where I am performing the statistical analysis and checking the accuracy by applying the linear regression model as well as the multiple linear regression model. The overall project is based on analyzing the dataset and applying the transformation as needed. In this project, we first visualized the data to get some brief insight into it, and then we did a deep analysis of the data distribution, where I checked if the data is normally distributed or not. If not, then I apply the data transformation technique and check the performance with the help of a linear or multiple linear regression model and cross-validate it, and I also visualize the data before and after transformation to get a better idea of how data transformation works inside the data.

## About the Dataset
Embark on a journey through the air quality landscape of Hyderabad City with our meticulously curated dataset. This invaluable resource, derived from trusted government sources, presents a comprehensive view of the air quality index (AQI) alongside various pollutant parameters. With 72 rows and 11 columns of data at your disposal, including PM10, SO2, NOx, PM2.5, ammonia, O3, CO, benzene, and the AQI, you'll have the tools to explore and analyze the city's air quality patterns and trends.
Our dataset, inspired by the need for environmental awareness and analysis, offers an unrivaled opportunity for researchers, data scientists, and environmental enthusiasts. By examining the various pollutant concentrations, we aim to shed light on the factors contributing to air pollution and encourage sustainable initiatives to mitigate its impact. The inclusion of historical data spanning different months empowers you to observe seasonal variations and potential correlations between pollutant levels, enabling a deeper understanding of the city's air quality dynamics.
With a focus on transparency and reliability, the data has been sourced directly from reputable government sources. This ensures the accuracy and credibility of the information, providing a solid foundation for impactful research and data-driven decision-making. By leveraging this dataset, you can identify critical areas for intervention, devise targeted pollution reduction strategies, and contribute to the collective effort to create a cleaner and healthier environment.
In short, the data is taken through Kaggle dataset collection, and the data is related to Hyderabad city air quality, where it has 72 rows and 11 columns.
Table of Contents
1. Pre-Processing
2. Visualizatioin
3. Statistical Analysis
4. After data visualization

## Pre-Processing
Data pre-processing is an essential and foundational step in the journey from raw data to meaningful insights. It serves as a crucial bridge that ensures the quality, accuracy, and reliability of the subsequent analyses or machine learning models. This preliminary phase involves a series of techniques and transformations that clean, structure, and enhance the raw data, making it more amenable for downstream processing.
Data pre-processing is both an art and a science, demanding domain knowledge and analytical acumen. Choices made during this phase can profoundly impact the final outcomes.
Basically, in our project, after the extraction of data from Excel to CSV, I have tried to remove the duplicate data, clean the null values, and also replace them with their mean, median, or mode as needed. This is one of the basic process steps where all the projects of data science or data analysts have gone through it. After re-checking the null and duplicate values, I have tried to analyze the date-time of the dataset where I have revaluate in the correct order or sequence. Now the data is ready for further steps.
## Visualizatioin
Visualization is more than just aesthetics; it's a medium through which complex ideas are distilled into intuitive images. Effective visualization transcends language barriers, enabling data-driven storytelling that resonates with diverse audiences. Ultimately, this process bridges the gap between data and decision-making, enabling analysts to distill patterns, outliers, and relationships that might otherwise remain obscure, facilitating more informed choices and insights.
Visualization is the artistic and informative facet of data analysis, transforming raw numbers into visual narratives that facilitate understanding, reveal patterns, and unveil insights. This process involves selecting appropriate visualization techniques, crafting meaningful representations, and conveying complex information in a digestible manner.

### In Project Visualization
In this project, I have done two visualizations: one before the statistical analysis and the second after the analysis. The first visualization, which is done before analysis, is used to understand the data in depth. It elaborates on the whole dataset in a wide manner or gives a better understanding of the data inside the dataset. This visualization is generally used to find patterns or anomolies that help the analyst check the nature of the data. After the statistical analysis, visualization is used to find the difference between the before and after analysis graphs. after visualization.
Before and after the application of statistical analysis and visualization, data remains a sea of potential insights, awaiting translation into actionable knowledge. The "before" phase encompasses raw data—a labyrinth of numbers and attributes that lack coherent structure or meaning. At this stage, patterns and trends are hidden beneath layers of complexity, making it difficult for even seasoned analysts to discern meaningful information.
Enter statistical analysis visualization, the transformative "after" phase. This is where data gains a visual voice, speaking in the language of graphs, charts, and interactive plots. The abstract becomes tangible as relationships and trends emerge from the visual representations. Complex statistics find resonance in these visual cues, enabling immediate comprehension and deep insights.
The "before" is a realm of potential, and the "after" is where potential is realized. Visualizations distill intricate statistical results into a form that is accessible to a wider audience, transcending the barriers of technical jargon. Decision-makers, stakeholders, and experts from various domains can all grasp the story told by the data.
I use multiple visualization libraries for this, such as
1. Seaborn
2. Matplotlib
3. Plotly
4. Scipy.stat

### Seaborn 
Seaborn is a prominent Python data visualization library that enhances the visual storytelling of data analysis. Built on top of Matplotlib, Seaborn offers a higher-level interface, making it effortless to generate informative and aesthetically pleasing visualizations. With its elegant and concise syntax, Seaborn simplifies the creation of complex plots, from basic scatter plots and histograms to advanced statistical visualizations like heatmaps, violin plots, and pair plots.

One of Seaborn's distinctive strengths lies in its seamless integration of statistical functions into visualizations. This feature allows users to effortlessly display underlying relationships, correlations, and distributions within the data. Seaborn's color palettes, themes, and customization options further elevate the quality of visual outputs, ensuring that each plot is not only insightful but also visually appealing.

Whether for exploratory data analysis, explanatory visualizations, or presentations, Seaborn serves as a versatile tool in the data analyst's arsenal. Its ability to quickly generate sophisticated plots with minimal code empowers users to delve into data complexities and extract valuable insights efficiently. With Seaborn, the process of translating raw data into compelling narratives becomes a seamless and creative endeavor.

### Matplotlib
Matplotlib stands as a cornerstone in the realm of data visualization libraries. With its origins dating back to 2003, it remains one of the most widely used and foundational tools for creating static, interactive, and publication-quality visualizations in Python. Matplotlib's versatility lies in its ability to generate a wide array of visualizations, from basic line plots to intricate heatmaps and complex 3D graphs. Its intuitive syntax and vast customization options provide users with granular control over every aspect of their visualizations. Despite its rich feature set, Matplotlib also serves as a stepping stone for other libraries like Seaborn and Pandas, building upon its foundation to offer specialized visualizations with streamlined workflows. Matplotlib's enduring popularity within the data science and scientific communities underscores its significance as an essential instrument for translating raw data into insightful, informative, and visually appealing representations.

### Plotly
Plotly is a dynamic and interactive data visualization library that empowers users to create compelling visualizations with ease. Offering both open-source and commercial versions, Plotly supports a range of programming languages, including Python, R, and JavaScript. One of its standout features is its ability to generate interactive plots and dashboards where users can explore data, zoom in on specific sections, and toggle between different views.
Plotly's versatility shines through its diverse chart types, which encompass everything from basic scatter plots to intricate 3D surface plots and geographical maps. Its integration with Jupyter notebooks and web applications allows for seamless data exploration and presentation. Additionally, Plotly Express, a high-level interface built on top of Plotly, simplifies the creation of complex visualizations with concise syntax.
One of Plotly's hallmarks is its emphasis on aesthetics and interactivity, fostering a user-friendly experience for both creators and consumers of visualizations. With its ability to produce visually appealing and responsive graphs, Plotly has become a valuable tool for data scientists, analysts, and researchers seeking to communicate insights effectively. Whether used for exploratory data analysis or for crafting interactive dashboards, Plotly's impact on the data visualization landscape is significant and continues to evolve.

### Scipy
The probability plot functionality within the `scipy.stats` module offers a powerful tool for assessing the distributional characteristics of data and comparing them against theoretical probability distributions. This feature allows users to visualize how closely a dataset aligns with a chosen distribution, aiding in the selection of an appropriate model for statistical analysis. By plotting the quantiles of the observed data against the quantiles of the theoretical distribution, deviations from linearity can indicate departures from the chosen distribution. This method is particularly useful in identifying outliers, skewness, and overall goodness-of-fit. The probability plot functionality in `scipy.stats` serves as a valuable diagnostic tool for statisticians and data analysts, enabling them to make informed decisions about the suitability of specific distributions for their datasets and refine their statistical modeling approaches accordingly.

Basically, this project is totally based on statistical analysis, so the visualization is also based on statistical analysis. In the beginning of the visualization section, I visualize the box whisker chart, where we try to understand what column of data is scaled on what range.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/f2484017-9928-4c52-9d6e-968639024f27)

Now we get the rough statistical measurement or assumption that the PM10 data is in between 80 and 127 or that SO2 has many outliers, as well as that the range of SO2 is in between 10 and 18. I am again repeating that it is just an assumption, not an accurate value. So with the help of this, we just got an idea of how much we have to pre-process or refine the data.
Then, after we have performed the histogram chart, which gives the basic idea of skewness or data skewness,
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/86c86549-8469-445b-ad17-300e91afa223)

At the very basic level, we do not have a proper skewness idea, but after viewing this, we have a rough estimation that the NH13 data is equally distributed, and CO has right skewed data as well as messing. So this graph is generally used for this.
Our next graph is a scatter plot, where at once I have done and visualized the data, where each data point is just like matrix multiplication, or in easy language, when each row is multiplied with each column, and I generate the scatter plot.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/23ec92c7-8c94-4eb0-80d5-e0b7e06d0adb)

In this image, the scatter plot is formed with the help of the matics concept, where once the X-axis changes with the column, the Y-axis randomly changes as per the matrices or column numbers.
Just after this graph, the next graph or visualization is also the same, but there is a little change inside it. The scatter of the plot is generated according to the year. This graph shows how much increment or decrement is done inside the AIQ as per the year.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/17ddb23d-f418-4eb1-9f35-b0ef2fb0d6c8)

Then I visualize the Vilon plot, line plot, and separate scatter plot for better understanding.

## Statistical Analysis
Statistical analysis is the systematic process of extracting insights and making sense of data through mathematical and computational techniques. It encompasses a wide range of methods, from summarizing and describing data to inferring relationships and patterns. By applying statistical techniques, data analysts and researchers can uncover hidden trends, validate hypotheses, and make informed decisions. This involves measures such as mean, median, and standard deviation, as well as more advanced techniques like regression analysis, hypothesis testing, and ANOVA. Statistical analysis enables the quantification of uncertainty, helping to assess the reliability of conclusions drawn from data. It plays a pivotal role across various fields, from scientific research and economics to healthcare and the social sciences. The goal is to transform raw data into meaningful information, providing valuable insights that guide understanding, decision-making, and policy formulation.
Statistical analysis with regression is a cornerstone of data science that delves into the relationships between variables, aiming to understand how one or more predictors influence a target outcome. Regression models provide a structured framework for quantifying these relationships, enabling us to make predictions, infer causal links, and uncover underlying patterns. Whether it's linear regression for simple relationships or more complex variants like multiple regression, polynomial regression, or logistic regression for classification tasks, these models allow us to quantify the impact of independent variables on the dependent variable. Through techniques like parameter estimation and hypothesis testing, statistical analysis with regression provides insights into the strength, direction, and significance of associations, allowing data scientists and analysts to draw meaningful conclusions from their data. This approach has applications across various fields, from economics and social sciences to healthcare and engineering, guiding decision-making and fostering a deeper understanding of the intricate connections that drive real-world phenomena.
After the statistical analysis portion is done, I have to start visualizing the transformation and without transformation data with the help of the Scipy library, where it gives results like:
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/ce50db0e-b11d-4796-bb2f-00d3bfb40f32)

I also visualized the 3rd dimension graph to understand more clearly the nature of the data, and the output is like:
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/d9f2325e-1e71-43df-b88b-584222ff9809)
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/f0c3180c-b835-4cde-8199-ec380deb3659)
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/ea8ffe9a-a660-4d81-be96-866a311b3202)
Then, after we have done more comparisons with before and after transformations of data, we can find which transformation is best for data skewness.

## Description
Basically, the statistical analysis is totally based on the statistics where lots of things came into the scenario. In statistical analysis, we perform hypothesis testing, the chi-square test, and regression analysis to perform some predictive analysis and get some patterns. In normal data analysis, we use machine learning algorithms for prediction, but in statistical analysis, we use statistical concepts that help in the prediction process. So I use regression, which is a basic as well as a vast method. This machine learning as well as statistical algorithm finds the relationship between the dependent and independent variables.

### Dependent variable:-
The dependent variable, also known as the response variable or outcome variable, is the variable in a research or statistical analysis that you're trying to explain, predict, or understand. In a cause-and-effect relationship, the dependent variable is the one that changes in response to changes in the independent variable(s).
For example, let's consider a simple scenario: you're studying the effect of studying time on exam scores. In this case, the exam score would be the dependent variable. You want to determine how changes in the amount of time spent studying (an independent variable) influence the outcome, which is the exam score.

### Independent Variable:-
An independent variable, also known as a predictor variable or explanatory variable, is a variable in research or statistical analysis that is manipulated or observed to understand its effect on the dependent variable. In other words, it's a variable that is hypothesized to influence or cause changes in the dependent variable.
In a cause-and-effect relationship, the independent variable is the one that you're changing or varying in order to observe its impact on the dependent variable.
Continuing with the example of studying time and exam scores:
Independent Variable: The amount of time spent studyingDependent Variable: Exam Scores
In this scenario, you're interested in understanding how changes in the independent variable (studying time) lead to changes in the dependent variable (exam scores). You might gather data by varying the amount of time students spend studying and then measuring their resulting exam scores.
Here are some common types of regression:

1. Linear Regression: This is the simplest form of regression, where the relationship between the dependent variable and independent variables is modeled as a linear equation. It's used when there's a linear relationship between the variables.

2. Multiple Regression: This extends linear regression to multiple independent variables. It's used when you have more than one predictor variable affecting the dependent variable.

3. Polynomial Regression: When the relationship between variables isn't linear, polynomial regression fits a polynomial equation to the data.

4. Ridge Regression: Also known as Tikhonov regularization, it's a form of linear regression that includes a penalty term for the coefficients to prevent overfitting.

5. Lasso Regression: Like ridge regression, lasso regression adds a penalty term, but in this case, it uses the absolute values of the coefficients. It can be used for feature selection as well.

6. Elastic Net Regression: This is a combination of ridge and lasso regression, incorporating both L1 and L2 regularization terms. It aims to balance their strengths.

7. Logistic Regression: Despite its name, logistic regression is used for binary classification problems. It models the probability of a binary outcome as a function of predictor variables.

8. Poisson Regression: This is used when the dependent variable represents counts and follows a Poisson distribution, commonly seen in count data like the number of occurrences of an event.

9. Negative Binomial Regression: Similar to Poisson regression, this is used when the data exhibits overdispersion, which means it has more variability than a Poisson distribution can accommodate.

10. Time Series Regression: When dealing with time-ordered data, time series regression models help capture the relationship between variables over time.

11. Robust Regression: It's used when the assumptions of ordinary least squares (OLS) regression are violated, such as the presence of outliers or heteroscedasticity (unequal variance).

12. Nonlinear Regression: When the relationship between variables is not linear, nonlinear regression models, such as exponential or power equations, are used.

13. Bayesian Regression: It incorporates Bayesian statistical principles into regression analysis, providing a distribution of possible model parameters rather than just point estimates.

14. Quantile Regression: Instead of modeling the mean of the dependent variable, quantile regression models different quantiles, helping to understand the relationship across the entire distribution.

where, among all, I have only used linear and multiple-linear regression.
## The final conclusion of this analysis is:
There are several reasons for negative values arriving when we perform the cross-validation score, and those are:
Scoring FunctionData 
PreprocessingModel 
ImplementationModel 
HyperparametersData 
LeakageFeature Selection and 
EngineeringModel Complexity
Insufficient Data
Model Validationand 
I personally believe and think that the negative values of the cross-validation score occurred due to the insufficient data during the model training, and I think it is an important factor to consider that sometimes, or in some cases, negative scores can occur when the data is not sufficient to train the model effectively. and for that, we will try to consider obtaining more data or using data augmentation techniques if possible.
