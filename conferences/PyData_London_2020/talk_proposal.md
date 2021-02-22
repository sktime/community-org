contributor: @mloning

# Title
sktime - a new scikit-learn compatible toolbox for machine learning with time series

## Audience level
novice

## Brief summary 
400 chars

We present sktime, a new scikit-learn compatible Python toolbox for machine learning with time series. We focus on aspects of practical machine learning and software architecture, highlighting different learning tasks that arise in temporal data settings, machine learning strategies to solve them, and sktime's key design ideas that extend available tools like scikit-learn to time series data. 


## Description
200 words

We present sktime -- a new Python library for machine learning with time series. 

Time series data are ubiquitous in many applications. Examples include sensor readings from industrial processes, spectroscopy wave length data from chemical samples, or bed-side monitor medical data from patients. There is a broad variety of distinct but closely related learning tasks that arise in such contexts, including time series classification, forecasting and annotation among others. 

Why sktime? Because there is no unified toolbox for time series. Of course, there are many toolboxes for time series, but none of them offers an interface for multiple learning tasks and advanced modular functionality as in scikit-learn. Our ambition is to extend scikit-learn beyond the standard tabular setting to time series data. But why does a unified interface for time series make sense? 

A unified API has two key advantages: first, many time series tasks can be solved by decomposing the task into simpler tasks first – an idea called reduction. For example, forecasting is often solved via regression by using rolling window cross-validation. Having a unified interface allows to build modular workflows, using different algorithms to solve different tasks and to tune hyper-parameters of composite and reduction workflows. Second, a unified interface reduces confusion by clearly distinguishing the different learning tasks, estimators and how they can be used interchangeably. 
