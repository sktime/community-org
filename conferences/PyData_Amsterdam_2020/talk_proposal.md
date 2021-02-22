# PyData2020 talk: "sktime - A Unified Toolbox for Machine Learning with Time Series"


## Short description
We present sktime, a new scikit-learn compatible Python toolbox for machine learning with time series. We focus on aspects of practical machine learning and software architecture, highlighting different learning tasks that arise in temporal data settings, machine learning strategies to solve them, and sktime's key design ideas that extend available tools like scikit-learn to time series data. 


## Long description
Time series are ubiquitous in real-world applications, and often add considerable complications to data science workflows. What's more, popular toolboxes like scikit-learn are limited to the tabular setting and hence not easily applicable to time series data.

We present sktime, a new scikit-learn compatible Python toolbox for machine learning with time series (https://github.com/alan-turing-institute/sktime). sktime is an open-source project, currently developed in collaboration by researchers at The Alan Turing Institute, UCL and the University of East Anglia and industry practitioners, and we're looking for new contributors. 

In this talk, we'll focus on aspects of practical machine learning and software architecture. In particular, you'll learn about:

1. What machine learning with time series is, i.e. the different learning tasks that arise in a temporal data settings, such as forecasting and time series classification/regression, and common machine learning approaches to solve them,
2. Why we develop another toolbox and the main advantage of sktime over other task-specific toolboxes like statsmodels, tsfresh or prophet, 
3. How sktime extends scikit-learn to time series data, including reduction (e.g. solving a more complex task by decomposing it into simpler tasks) and other composition strategies,
4. Key software design lessons for machine learning toolboxes. 

