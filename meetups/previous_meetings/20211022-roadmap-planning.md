# Roadmap

###### tags: `sktime`

Current roadmap: https://www.sktime.org/en/latest/roadmap.html

Contributors: @RNKuhns, @mloning, @fkiraly, @TonyBagnall, @GuzalBulatova, @SveaMeyer13, @Lovkush-A, @aiwalter, @MatthewMiddlehurst

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
https://sktime-group.slack.com/archives/G01MYS9EFUL/p1634315490343000
- move to report writing section

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
- Wordsmith and get ready for PR review [Markus] (done), see https://github.com/alan-turing-institute/sktime/pull/1527

---
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
| **Documentation** | Community | (1) Clear technical docs; (2) Explain data scientific tasks | (1) Incomplete docstrings; (2) User Guide for each major learning has description of learning task.| 
| **Software engineering & dev ops** | Framework, ecosystem | (1) Unit testing; (2) Efficiency (algorithm training and inference, unit tests); (3) Module structure; (4) Managing releases; (5) API design quality | (1) Code coverage; (2) Run time (functionality + unit tests) |
| **Ecosystem interoperability** | Ecosystem | (1) Portable unit tests for API compliance, (2) Defining common APIs; (3) Interfacing other packages; (4) Defining key parts of ecosystem; | 
| **Community building** | Community | (1) Community of practice (developers + users); (2) mentoring | (1) Number of mentees
| **Functionality** | Framework | see core areas below

---
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

### Action Items
* Markus: post question about which 7-10 core areas to focus on (done) https://sktime-group.slack.com/archives/G01MYS9EFUL/p1633879921311300

### Overview

| Core Area | Coordinator | 
|---|---|
| Project management and operations (e.g. reporting, fundraising) | @fkiraly |
| Community building | | 
| Outreach & marketing | |
| Documentation | @RNKuhns, @mloning can help  | 
| Software engineering & dev ops | @mloning |
| sktime-dl | @TonyBagnall, @mloning can help 
| Classification | @TonyBagnall | 
| Regression | @MatthewMiddlehurst
| Clustering | ask @chrisholder |
| Transformations | @fkiraly, @aiwalter can help
| Forecasting: univariate | @aiwalter
| Forecasting: multivariate | @aiwalter
| Benchmarking, performance metrics and statistical tests | @RNKuhns
| Annotation: outlier detection | @fkiraly
| Forecasting: hierarchical & global | ask @DanielBartling, @fkiraly advisory

### Aspirational core areas
| Core Area | Coordinator | 
|---|---|
| Forecasting: panel & supervised
| Annotation: Segmentation
| Annotation: Change point
| Annotation: Advance event modelling (predicting annotation of time point in the future) 
| Sequence/series alignment (aka sequence registration)


> Plan for today:
> 1. Review last meeting
> 1. Rank core areas and agree on 7-10 learning task specific areas to focus on
> 1. Assign coordinators
> 1. Focus on 2-3 overarching core areas today (docs, software engineering & dev ops, community building)
>
> Action: Coordinators collect and prepare roadmap items for learning task related core areas until next meeting
> Next, final meeting: review learning task specific core areas

Link from previous roadmap planning session during dev sprint: https://hackmd.io/UPzaTv_ER2GiTXUyfy-XFQ

### Documentation
> Descriptions of work items for core areas

User-facing or developer-facing information designed to make it easy to use sktime, for example docstrings, user guide, online book. 

#### Short Term
> * This is a tactical set of tasks we can implement to help us move toward our medium- and long- term goals. 
> * Focus is on next 6 months (3 releases)

* have a minimal but complete set of docs (user guide + examples) for:
    * classifcation
    * forecasting
    * clustering
    * transformations
* revise univariate and multivariate classification examples 
* revise classification docstrings and docstring examples 
* revise forecasting docstrings and docstring examples
* arrange meetings with UCL ARC to discuss taught graduate course 
* improve getting started guide 
    * add time series regression quickstart
    * add docs on scitype/mtypes
    * add plot to custering quickstart
    * add plot to forecasting quickstart
    * add plot to annotation quickstart
* revise developer getting started guide (CONTRIBUTING.md)

#### Medium Term
> * This is akin to an organization’s annual operating plan
> * What are our priorities for new modules, functionality within modules, etc)? 
> * Do we intend to have completed a first draft of user guide content in a year?
> * Focus is on next year

1. have a minimal but complete set of docs for all supported learning tasks (user guide + examples)
1. have a minimal but complete set of docs for transformations (user guide + examples)
3. have a comprehensive set of docs for classification (user guide + examples)
4. have a comprehensive set of docs for univariate & multivariate forecasting (user guide + examples)
5. improve getting started guide 
6. improve developer guide, especially the getting started section on using git, precommit, etc
7. identify interested stakeholders in developing joint graduate course (UCL, UEA, Berlin, Dublin, Monash)

#### Long Term
> * What are our concrete goals in terms of the functionality we want to have for each learning task eventually? 
> * What type of documentation do we want to have as part of the project eventually?
> * Do we have long-run expectations for unit testing, the project’s module layout or other important technical areas (that are not learning tasks but are nonetheless important)?
> Focus is on next 5-10 years

* write online book, something like "Introduction to Statistical Learning" for time series 
* create massive open online course (MOOC)
* create taught graduate course, adoptable by different universities 
* have a great website
    * "an idiot's guide to developing sktime", minimal-effort developer documentation (for different platforms and IDEs)
    * have a complete and user-friendly changelog
    * all docstrings are complete and compliant with sktime convention
    * user guide for every learning task


### Software engineering & dev ops

Infrastructure designed to make it easy to develop sktime and optimize user experience, for example unit tests, CI/CD, portability & package ecosystem, time & memory efficiency, module structure and API design quality.

#### Short Term


#### Medium Term


#### Long Term

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
