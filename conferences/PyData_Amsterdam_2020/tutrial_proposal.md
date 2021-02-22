# PyData2020 tutorial: "Introduction to Machine Learning with Time Series"


## Short description
Time series are ubiquitous in real-world applications, but often add considerable complications to data science workflows. In this tutorial, you’ll learn about how to apply and extend machine learning techniques to time series. You’ll learn about state-of-the-art algorithms, time series specific composition approaches like ensembling, detrending and reduction. 

## Long description
Time series are ubiquitous in real-world applications, but often add considerable complications to data science workflows. What's more, most available machine learning toolboxes (e.g. scikit-learn) are limited to the tabular setting, and cannot easily be applied to time series data. 

In this tutorial, you'll learn how to apply common machine learning techniques to time series and how to extend available toolkits. 

This is a beginner-friendly tutorial: we assume familiarity with scikit-learn, but no prior experience with time series. 

To start, you'll learn how to distinguish between different kinds of temporal data and associated learning tasks, such as forecasting and time series classification. 

You'll then learn how to solve these tasks with machine learning techniques specific to time series data, including:

* State-of-the-art algorithms for time series classification and regression,
* Reduction strategies, i.e. solving a complex learning tasks by decomposing it into simpler tasks, e.g. solving forecasting via regression,
* Composite strategies like ensembling and pipelining, as well as data transformations like detrending and feature extraction. 

We'll work through all of them step by step and make use of interactive Jupyter notebooks and sktime, a new scikit-learn compatible toolbox for machine learning with time series (https://github.com/alan-turing-institute/sktime).
