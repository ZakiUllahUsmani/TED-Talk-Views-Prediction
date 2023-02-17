# Project Name - TED Talks Views Prediction

Project Type - Regression

Contribution - Individual

Name - Md Zaki Ullah Usmani
# Project Summary -
TED stands for Technology, Entertainment, and Design. It is an American-Canadian non-profit media organization that posts international talks online for free distribution under the slogan "ideas worth spreading". TED was founded by Richard Saul Wurman and Harry Marks in February 1984 as a tech conference, in which Mickey Schulhof gave a demo of the compact disc that was invented in October 1982. It has been held annually since 1990. TED covers almost all topics – from science to business to global issues – in more than 100 languages. To date, more than 13,000 TEDx events have been held in at least 150 countries.

This TED data collected from 2006 to 2020, has 4005 observations with 19 features. Our main objective is to build a predictive model to predict the number of views for the respective videos from the TEDx website. As we have a continuous variable to predict, we use regression models to predict the views of the TED talks. But before that, I'll check whether the assumption of linear regression is satisfying or not and fix it.

In this project first, I'll do some exploratory data analysis to get some valuable insights. Then I'll do features engineering to manipulate the data a bit if needed. To do this sort of work I'm going to use some amazing python libraries. like pandas and numpy for data manipulation, matplotlib, seaborn, and plotly for visualization, maths for calculations, and scikit learn to build a better machine learning model.

In order to get the best-fit line (best predictions) I'll remove the outliers after exploratory data analysis. At the end of the project, I'll conclude the best model by comparing each machine learning model with or without cross-validation and hyperparameter tuning.

For model evaluation, we have multiple evaluation metrics. Like mean squared error (MSE), root mean squared error (RMSE), mean absolute error (MAE), mean absolute percentage error (MAPE) r2 score, and adjusted r2.

# Used Libraries:-
Numpy :- NumPy is a Python library used for working with arrays. It also has functions for working in the domain of linear algebra, Fourier transform, and matrices.

Pandas :- Pandas is an open-source Python package that is most widely used for data science/data analysis and machine learning tasks. It is built on top of Numpy, which provides support for multi-dimensional arrays.

Matplotlib :- Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. Matplotlib makes easy things easy and hard things possible.

Seaborn :- Seaborn is a library that uses Matplotlib underneath to plot graphs. It will be used to visualize random distributions.

Plotly :- The plotly Python library is an interactive, open-source plotting library that supports over 40 unique chart types covering a wide range of statistical, financial, geographic, scientific, and 3-dimensional use cases.

Math :- Math is a built-in module in the Python standard library that provides standard mathematical constants and functions. We can use the math module to perform various mathematical calculations, such as numeric, trigonometric, logarithmic, and exponential calculations.

DateTime :- datetime in Python is the combination between dates and times. The attributes of this class are similar to both date and separate classes. These attributes include day, month, year, minute, second, microsecond, hour, and time zone information.

Scikit-Learn :- Scikit-learn is an open-source data analysis library and the gold standard for Machine Learning (ML) in the Python ecosystem. Key concepts and features include Algorithmic decision-making methods, including Classification: identifying and categorizing data based on patterns.

I will consider mean squared error, r2 and adjusted r2 as my evaluation metrics, beacause sum of squared errors gives the distence from the actual data point to the predicted data point. If we can get the mean of that sum of squared error we'll get the best fit line or better predictions. Sometimes R squared doesn't give a satisfactory score that is why i also considerd adjust R squared as my evaluation metrics.

If i talk about the model which i'll choose, is the randomforest regressor model from the above created model. Beacause in linear regression and xgb model i got the highest mean squared error as compared to randomforest model. If i talk about the r2 and adjusted r2 score then again randomforest model performed well as compared to other two models.


# Conclusion
I did a lot of hard work, from loading a dataset to making the best model. Which includes Exploratory data analysis, data cleaning, feature engineering, and ml model building.

## I've modeled on:-

* Simple linear regression

* Lasso Regressor

* Random forest Regressor

* XGB Regressor

My model is able to predict views correctly 90% of the time. Given that model has 10% errors, my models have performed very well on unseen data due to various factors like feature selection, correct model selection, etc.
Out of all these models, RandomForestRegressor is the best performer in terms of MSE, R2, and Adjusted R2.
Of all the features speaker_wise_avg_views is the most important this implies that speakers are directly impacting the views.
