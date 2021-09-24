# Roadmap

###### tags: `sktime`

Current roadmap: https://www.sktime.org/en/latest/roadmap.html

Contributors: @RNKuhns, @mloning, @fkiraly, @TonyBagnall, @GuzalBulatova, @SveaMeyer13, @Lovkush-A

> Key questions to keep in mind:
> * Who is the target audience for the roadmap? Funders, developers, maintainers of other packages, end users 
> * What are the overarching goals?
> How can we measure the project's goals and roadmap completion?

## Mission Statement
> Review mission statement below
> Integrate points from "Project vision" section on README
> What are the project's overarching goal(s)?
> How do we judge if we're successful in achieving our mission?
 
sktime is an easy-to-use, flexible and modular framework for a wide range of time series machine learning tasks. It provides scikit-learn compatible algorithms and model composition tools, with the goal to make the ecosystem more interoperable as a whole. sktime is developed by a diverse community, welcoming new contributors from academia and industry through instructive documentation, mentoring and workshops.

### Notes
- "Understandable" might be misleading toward explainable ML academic field
    - "intuitive"
    - Expressive syntax a better descriptor?
    - "transparent"
    - "easy-to-use"
- In last sentence about community, we need to think about phrasing related to governance and we vs. sktime. 

What does "community-led" mean:
* community governed
* workshops
* mentoring
* community of practice, expertise ...
* docs!
* academia + industry 
* open source
* welcoming, motivated to upskill new contributors
* replace "developed" by "driven"
* want to emphasise 'we are' not 'sktime is'
* want to emphasise governance, somehow.

#### key themes
* software framework
* community practice
* ecosystem interoperability

#### measuring how we achieve our mission
- Is there a good way to collect feedback from end-users?
    - User testing?
    - Surveying?
    - number of stars/contributors/dependent projects/downloads/user issues

### Action Items
- Think about and come back with ways to measure how we achieve our mission for the next meeting

## Motivation: why do we develop sktime?
* fair evaluation and comparison of algorithms
* quicker application development
* have transparent, readable specification of ML applications
* make ecosystem more interoperable and usable as a whole
* create unified software and theory framework for multiple learning tasks in time series analysis
  * time series tasks split up all over the place. no consistent terminology or conventions.
* connect communities of algorithm developers, domain experts and practitioners
* quality/reproducibility crisis in science/research/ML/data science/AI and available off-shelf methodology (algorithms)
* new, community-driven model for full data science innovation cycle: software products, statistical methodology, software development process, deployment in industry
    * in the past, some academic writes a paper. some industry person randomly finds it. does not properly understand it. implements it in mixed up way. becomes part of commerical product.
    * speeding up the innovation cycle
* alternative options for junior academics / junior data scientists
  * more opportunities for more people.
* make it easier to study time series analysis

## Scope of sktime
> Review scope below

features:
* API for machine learning with time series, for the purpose of specifying, fitting, applying and validating machine learning models
* key use cases: notebook style analytics; use as a library component

specs:
* in-memory computation of a single machine, no distributed computing 
* medium-sized data in pandas and NumPy
* modular, principled object-oriented API
* a Python library
* making use of Python interpreter, no command-line interface or graphical user interface


## Points of Emphasis
> Set 3 - 5 overall goals + measurables
> 
> for example:
> * documentation: 
>    *  number of classes with missing docstrings
> * software engineering: code coverage
> * classification module: implemented algorithms, add specific cutting-edge algorithms 
> * interoperability with other libraries in the ecosystem: number of interfaced libraries

| Goal | Description |Measurable |
|---|---|---|
| :books: **Documentation** | (1) Clear technical docs; (2) Explain data scientific tasks | (1) Incomplete docstring; (2) User Guide for each major learning has description of learning task.| 
| :hammer_and_wrench: **Software engineering & dev ops** | (1) Unit testing; (2) Efficiency; (3) Module structure; (4) Managing releases | (1) Code coverage; (2) Run time (functionality + unit tests) |
| **Ecosystem interoperability** | | | 


## Core Areas
> Identify core areas
> Identify coordinators
> Describe detailed roadmap split by core areas and for short/mid/long term 
>
> Add link to STEPs
>
> Timelines:
> * short term: next 6 month, next 3 releases
> * medium term: next 1 year
> * long term: next 5 years

| Core Area | Coordinator |
|---|---|
| Documentation | | 
| Software engineering & dev ops | |
| Annotation
| Classification | |
| Regression 
| Forecasting
| Clustering
| Data container
| Performance metrics, benchmarking and statistical tests


### Documentation
> Descriptions of work items for core areas

#### Short Term
> * This is a tactical set of tasks we can implement to help us move toward our medium- and long- term goals. 
> * Focus is on next 6 months (3 releases)

#### Medium Term
> * This is akin to an organization’s annual operating plan
> * What are our priorities for new modules, functionality within modules, etc)? 
> * Do we intend to have completed a first draft of user guide content in a year?

#### Long Term
> * What are our concrete goals in terms of the functionality we want to have for each learning task eventually? 
> * What type of documentation do we want to have as part of the project eventually?
> * Do we have long-run expectations for unit testing, the project’s module layout or other important technical areas (that are not learning tasks but are nonetheless important)?


## Progress Report
> Synopsis overall (1-2 sentences)

### Documentation
> Bullet-point summary of progress, updated throughout development
> 
> For example:
> - Created new website
> - Cleaned 20 of 80 class docstrings


## Milestones & Issues
> milestones for releases 
> link to milestones for next releases


## References
* "The State of our Roadmaps" by Ralf Gommers, https://www.slideshare.net/RalfGommers/numfocussummit2018roadmapssession
