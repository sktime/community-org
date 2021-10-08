# Roadmap

###### tags: `sktime`

Current roadmap: https://www.sktime.org/en/latest/roadmap.html

Contributors: @RNKuhns, @mloning, @fkiraly, @TonyBagnall, @GuzalBulatova, @SveaMeyer13, @Lovkush-A

> Key questions to keep in mind:
> * Who is the target audience for the roadmap? Funders, developers, maintainers of other packages, end users 
> * What are the overarching goals?
> How can we measure the project's goals and roadmap completion?

---
## Mission Statement
> Review mission statement below
> Move to About section, print on roadmap page
 
sktime provides an easy-to-use, flexible and modular open-source framework for a wide range of time series machine learning tasks. It offers scikit-learn compatible interfaces and model composition tools, with the goal to make the ecosystem more usable and interoperable as a whole. We build and sustain an open, diverse and self-governing community, welcoming new contributors from academia and industry through instructive documentation, mentoring and workshops.


### Themes
- framework
- ecosystem
- community


### Measuring how we achieve our mission
> How do we judge if we're successful in achieving our mission?

- Quantity of usage: Can't achieve mission if we don't have people using sktime and participating in the community
    - Number of contributors, number of downloads, dependent projects, number of stars, how many people participate in developer meetings, etc
    - how much of the key time series analysis ecosystem is usable within a consistent interface
        - Would need to define "key" parts of ecosystem amongst our list of related software
- Quality of experience: Is there a good way to collect feedback from end-users?
    - user testing: surveys/questionaires
    - "expert" feedback: survey/questionaires/interview
        - Does sktime do what it should in terms of scientific methodology and software engineering?
    - number of bug reports (at least for consolidated module)
    - response time to bug reports
    - response time to feature requests


#### Notes
- FK thoughts:
    * number of algorithms native in sktime?
    * change in issues, PR over time? should be on average zero or negative (!)
    * time to first proper PR review! Very important!
        * for new contributors?
        * and developers
    * time to categorize new issues
    * user testing results - need to do this regularly!
        * perhaps also scale this up by online user testing, self-administered
    * Percentage of Issues/PRs with useful response (PR review; issue: categorization and pulling in relevent devs)

### Action Items

- Think about your favorite metrics in each category (and why)
    - Goal is to discuss specific metrics next time


---
## Motivation: Why do we develop sktime?
> review Markus' summary
> move to the bottom of the roadmap or into About section on website

* Easier application development
    * have transparent, readable specification of ML applications
    * make ecosystem more interoperable and usable as a whole
* Easier algorithm development
    * research, implementation, testing
* Better algorithm research
    * fair evaluation and comparison of algorithms
    * quality/reproducibility crisis in science/research/ML/data science/AI and available off-shelf methodology (algorithms)
* Easier teaching and learning
    * make it easier to study time series analysis
* Clearer time series methodology
    * clearer terminology, notation, conventions across learning tasks
* More collaboration and innovation
    * connect communities of algorithm developers, domain experts and practitioners
    * alternative career progression options for junior academics / junior data scientists
    * new, community-driven model for full data science innovation cycle: software products, statistical methodology, software development process, deployment in industry

### Action Item

- Wordsmith motivation and distill topics for eventual posting to "About" section of website [Franz]
    - Goal to have ready for PR review

---
## Scope of sktime
> Review scope below
> Move to docs landing page

Features:
* API for machine learning with time series, for the purpose of specifying, fitting, applying and validating machine learning models
* key use cases: notebook style analytics; use as a library component

Technical specification:
* in-memory computation of a single machine, no distributed computing 
* medium-sized data in pandas and NumPy
* modular, principled object-oriented API
* a Python library
* making use of interactive Python interpreter, no command-line interface or graphical user interface

### Action Items
- Wordsmith and get ready for PR review

## Points of Emphasis
> Set 3 - 5 overall goals + measurables
> 
> for example:
> * documentation: 
>    *  number of classes with missing docstrings
> * software engineering: code coverage
> * classification module: implemented algorithms, add specific cutting-edge algorithms 
> * interoperability with other libraries in the ecosystem: number of interfaced libraries

| Point of Emphasis | Theme | Description | Measurable |
|---|---|---|---|
| **Documentation** | Community | (1) Clear technical docs; (2) Explain data scientific tasks | (1) Incomplete docstring; (2) User Guide for each major learning has description of learning task.| 
| **Software engineering & dev ops** | Framework, ecosystem | (1) Unit testing; (2) Efficiency (algorithm training and inference, unit tests); (3) Module structure; (4) Managing releases; (5) API design quality | (1) Code coverage; (2) Run time (functionality + unit tests) |
| **Ecosystem interoperability** | Ecosystem | (1) Portable unit tests for API compliance, (2) Defining common APIs; (3) Interfacing other packages; (4) Defining key parts of ecosystem; | 
| **Community building** | Community | (1) Community of practice (developers + users); (2) mentoring | (1) Number of mentees
| **Functionality** | Framework | see core areas below

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
| Project management and operations |
| Community building |
| Comms and social media |
| Documentation | | 
| Software engineering & dev ops | |
| Annotation: Segmentation
| Annotation: Change point and outlier detection
| Annotation: Advance event modelling 
| Classification, Regression, Clustering (series-samples)
| Forecasting: univariate & multivariate
| Forecasting: hierarchical, panel & supervised
| Sequence/series alignment (aka sequence registration)
| Deep learning
| Transformers
| Data container
| Performance metrics, benchmarking and statistical tests

### Action Items
* Markus: post question about which 7-10 core areas to focus on 

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
