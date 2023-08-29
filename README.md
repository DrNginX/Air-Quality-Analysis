# Air-Quality-Analysis
Basically, the Project is based on the analysis of the air quality index, where I am performing the statistical analysis and checking the accuracy by applying the linear regression model as well as the multiple linear regression model. The overall project is based on analyzing the dataset and applying the transformation as needed. In this project, we first visualized the data to get some brief insight into it, and then we did a deep analysis of the data distribution, where I checked if the data is normally distributed or not. If not, then I apply the data transformation technique and check the performance with the help of a linear or multiple linear regression model and cross validate it, and I also visualize the data before and after transformation to get a better idea of how data transformation works inside the data.

## About Dataset
Embark on a journey through the air quality landscape of Hyderabad City with our meticulously curated dataset. This invaluable resource, derived from trusted government sources, presents a comprehensive view of the air quality index (AQI) alongside various pollutant parameters. With 72 rows and 11 columns of data at your disposal, including PM10, SO2, NOx, PM2.5, Ammonia, O3, CO, Benzene, and the AQI, you'll have the tools to explore and analyze the city's air quality patterns and trends.

Our dataset, inspired by the need for environmental awareness and analysis, offers an unrivaled opportunity for researchers, data scientists, and environmental enthusiasts. By examining the various pollutant concentrations, we aim to shed light on the factors contributing to air pollution and encourage sustainable initiatives to mitigate its impact. The inclusion of historical data spanning different months empowers you to observe seasonal variations and potential correlations between pollutant levels, enabling a deeper understanding of the city's air quality dynamics.

With a focus on transparency and reliability, the data has been sourced directly from reputable government sources. This ensures the accuracy and credibility of the information, providing a solid foundation for impactful research and data-driven decision-making. By leveraging this dataset, you can identify critical areas for intervention, devise targeted pollution reduction strategies, and contribute to the collective effort in creating a cleaner and healthier environment.

In short, the data is taken through kaggle dataset collection and the data is related to hyderabad city air quality where it have 72 rows and 11 columns.

# Table of Content
1. Pre-Processing
2. Visualizatioin
3. Statistical Analysis
4. After data Visualization

## Pre-Processing

Data pre-processing is an essential and foundational step in the journey from raw data to meaningful insights. It serves as a crucial bridge that ensures the quality, accuracy, and reliability of the subsequent analyses or machine learning models. This preliminary phase involves a series of techniques and transformations that clean, structure, and enhance the raw data, making it more amenable for downstream processing.

Data pre-processing is both an art and a science, demanding domain knowledge and analytical acumen. Choices made during this phase can profoundly impact the final outcomes

Basically in our project, after the extraction of data from excel to csv, I have try to remove the duplicate data, clean the null values and also replace with their mean, median or mode as per needed. This is one of the basic process step where all the project of data science or data analyst have gone while once through it. After re-checking the null and duplicates values I have tried to analyse the date-time of dataset where I have revaluate in correct order or sequence. Now the data is ready to go on further steps.

## Visualizatioin


Visualization is more than just aesthetics; it's a medium through which complex ideas are distilled into intuitive images. Effective visualization transcends language barriers, enabling data-driven storytelling that resonates across diverse audiences. Ultimately, this process bridges the gap between data and decision-making, enabling analysts to distill patterns, outliers, and relationships that might otherwise remain obscured, facilitating more informed choices and insights.

Visualization is the artistic and informative facet of data analysis, transforming raw numbers into visual narratives that facilitate understanding, reveal patterns, and unveil insights. This process involves selecting appropriate visualization techniques, crafting meaningful representations, and conveying complex information in a digestible manner.

In this project I have done the two vizualization one in before the statistical analysis and second one is after the analysis. The first Visualization which is done before analysis is used to understand the data into deep. It elaborate the whole dataset in wide manner or give the better understanding of data inside the dataset. This Visualization is generally used to find the pattern or anomoly which help to analyst check the data nature. After the statistical analysis visualization is used to find the difference in between before and after analysis graphs. In after visualization.

Before and after the application of statistical analysis visualization, data remains a sea of potential insights, awaiting translation into actionable knowledge. The "before" phase encompasses raw data, a labyrinth of numbers and attributes that lack coherent structure or meaning. At this stage, patterns and trends are hidden beneath layers of complexity, making it difficult for even seasoned analysts to discern meaningful information.

Enter statistical analysis visualization, the transformative "after" phase. This is where data gains a visual voice, speaking in the language of graphs, charts, and interactive plots. The abstract becomes tangible, as relationships and trends emerge from the visual representations. Complex statistics find resonance in these visual cues, enabling immediate comprehension and deep insights.

The "before" is a realm of potential, and the "after" is where potential is realized. Visualizations distill intricate statistical results into a form that is accessible to a wider audience, transcending the barriers of technical jargon. Decision-makers, stakeholders, and experts from various domains can all grasp the story told by the data.

I use multiple Visualization libraries for this such as
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
Plotly is a dynamic and interactive data visualization library that empowers users to create compelling visualizations with ease. Offering both open-source and commercial versions, Plotly supports a range of programming languages, including Python, R, and JavaScript. One of its standout features is its ability to generate interactive plots and dashboards, where users can explore data, zoom in on specific sections, and toggle between different views.

Plotly's versatility shines through its diverse chart types, which encompass everything from basic scatter plots to intricate 3D surface plots and geographical maps. Its integration with Jupyter notebooks and web applications allows for seamless data exploration and presentation. Additionally, Plotly Express, a high-level interface built on top of Plotly, simplifies the creation of complex visualizations with concise syntax.

One of Plotly's hallmarks is its emphasis on aesthetics and interactivity, fostering a user-friendly experience for both creators and consumers of visualizations. With its ability to produce visually appealing and responsive graphs, Plotly has become a valuable tool for data scientists, analysts, and researchers seeking to communicate insights effectively. Whether used for exploratory data analysis or for crafting interactive dashboards, Plotly's impact on the data visualization landscape is significant and continues to evolve.

### Scipy
The probability plot functionality within the `scipy.stats` module offers a powerful tool for assessing the distributional characteristics of data and comparing them against theoretical probability distributions. This feature allows users to visualize how closely a dataset aligns with a chosen distribution, aiding in the selection of an appropriate model for statistical analysis. By plotting the quantiles of the observed data against the quantiles of the theoretical distribution, deviations from linearity can indicate departures from the chosen distribution. This method is particularly useful in identifying outliers, skewness, and overall goodness-of-fit. The probability plot functionality in `scipy.stats` serves as a valuable diagnostic tool for statisticians and data analysts, enabling them to make informed decisions about the suitability of specific distributions for their datasets and refine their statistical modeling approaches accordingly.

Basically this project is totally based on the statistical analysis so the visualization is also is based on the statistical. In the starting of visualization section I visualize the box whisker chart where we try to understand that what column of data is scaled on what range?.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/f2484017-9928-4c52-9d6e-968639024f27)

Now we get the rough statistical mesurement or assumption that the PM10 data is in between the 80-127 or SO2 have many outliers as well as the range of SO2 is in between the 10- 18. I am again repeating it is just assumption not accurate value. So with the help of this we just got the idea of how much we have to pre-process the data or refine the data.

Then after we have perform the histogram chart which give the basic idea of skewness or data skewness.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/86c86549-8469-445b-ad17-300e91afa223)

The very basic we have not proper skewness idea but after viewing this we have rough estimation that the NH13 data is equaly distribute, CO have right skewed data as well as messing also. So this graph is generally used for this.

Our next graph is scatter plot where at once i have done and visualize the data where each data is just like matix multiplication or in easy language when each row are multipied with each column and generate the scatter plot.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/23ec92c7-8c94-4eb0-80d5-e0b7e06d0adb)

In this image the scatter plot is formed with the help of matics concept where while once the X-axis change with column and along the Y-axis randomly change as per the matrics or columns number.

Just after this graph, the next graph or visualization is also same but there have little change inside it the scatter of the plot is generated as according to the year. This graph show you that how much increment or decrement is done inside the AIQ as per the year.
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/17ddb23d-f418-4eb1-9f35-b0ef2fb0d6c8)


Then I visualize the Vilon plot, Line plot and seperate scatter plot for better understanding.

## Statistical Analysis

Statistical analysis is the systematic process of extracting insights and making sense of data through mathematical and computational techniques. It encompasses a wide range of methods, from summarizing and describing data to inferring relationships and patterns. By applying statistical techniques, data analysts and researchers can uncover hidden trends, validate hypotheses, and make informed decisions. This involves measures such as mean, median, and standard deviation, as well as more advanced techniques like regression analysis, hypothesis testing, and ANOVA. Statistical analysis enables the quantification of uncertainty, helping to assess the reliability of conclusions drawn from data. It plays a pivotal role across various fields, from scientific research and economics to healthcare and social sciences. The goal is to transform raw data into meaningful information, providing valuable insights that guide understanding, decision-making, and policy formulation.

Statistical analysis with regression is a cornerstone of data science that delves into the relationships between variables, aiming to understand how one or more predictors influence a target outcome. Regression models provide a structured framework for quantifying these relationships, enabling us to make predictions, infer causal links, and uncover underlying patterns. Whether it's linear regression for simple relationships or more complex variants like multiple regression, polynomial regression, or logistic regression for classification tasks, these models allow us to quantify the impact of independent variables on the dependent variable. Through techniques like parameter estimation and hypothesis testing, statistical analysis with regression provides insights into the strength, direction, and significance of associations, allowing data scientists and analysts to draw meaningful conclusions from their data. This approach has applications across various fields, from economics and social sciences to healthcare and engineering, guiding decision-making and fostering a deeper understanding of the intricate connections that drive real-world phenomena.

After the statistical analysis portion is done I have start visualizing the transformation and without transformation data with the help of Scipy library where it give result like :- 
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/ce50db0e-b11d-4796-bb2f-00d3bfb40f32)

I also visualize the 3rd dimension graph to understand more clearly the nature of data and the output is like:-
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/d9f2325e-1e71-43df-b88b-584222ff9809)
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/f0c3180c-b835-4cde-8199-ec380deb3659)
![image](https://github.com/DrNginX/Air-Quality-Analysis/assets/86653787/ea8ffe9a-a660-4d81-be96-866a311b3202)

Then after we have done more comparison with before and after transformation of data and find which transformation is best for data skewness. 

## Final Conclusion of this analysis is :-
There are several reasons for negative values arrived when we perform the cross validation score those are :-

Scoring Function
Data Preprocessing
Model Implementation
Model Hyperparameters
Data Leakage
Feature Selection and Engineering
Model Complexity
Insufficient Data
Model Validation
and I personally believe and think that the negative values of cross validation score occured due to the insufficient data during the model turing and I think it is an important factor to considerd that sometimes or in some cases, negative scores can occur when there is data is not sufficient to train the model effectively. and for that we will try to consider obtaining more data or using data augmentation techniques if possible.
