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
| Community building | @GuzalBulatova | 
| Outreach & marketing |@GuzalBulatova|
| Documentation | @RNKuhns (@mloning advisory)  | 
| Software engineering & dev ops | @mloning |
| sktime-dl | @TonyBagnall (@mloning advisory) 
| Classification | @TonyBagnall | 
| Regression | @MatthewMiddlehurst
| Clustering | @chrisholder |
| Transformations | @fkiraly (@aiwalter advisory) 
| Forecasting: univariate | @aiwalter
| Forecasting: multivariate | @aiwalter
| Benchmarking, performance metrics and statistical tests | @RNKuhns
| Annotation: outlier detection | @fkiraly
| Forecasting: hierarchical & global | (@fkiraly advisory)

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
    * add time series regression dataset so we can update quickstart
    * add docs on scitype/mtypes
    * add plot to clustering quickstart
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
* Refactor unit tests
    * make estimator-related unit tests follow unified design
    * make estimator-related unit tests portable
    * Improve consistency of pytest fixture usage
* publish deprecation policy
* publish release cycle
* replace Appveyor CI service, use GitHub Actions or Azure DevOps pipelines instead
* transfer existing accounts to sktime community accounts (e.g. CI/CD, PyPI)

#### Medium Term
* improve coverage to at least 90%
* reduce warnings raised by sktime (e.g. FutureWarnings from not updating use of dependencies)
* add gradual static type checking to precommit and CI (e.g. using mypy)
* speed up unit tests
* simplify dependency management
* move fbprophet to companion package 
* remove Cython code, replace where possible with numba 
* make module structure in transformations module consistent 

#### Long Term
* make sktime more extendible
    * make all API related functionality portable (unit testing, registry functionality, etc.)
    * make estimator unit tests callable from interactive Python interpreter
    * add template repository for easy creation of companion packages
* make sktime more robust
    * complete static type annotations and type checking 
    * manage all accounts through sktime community accounts
    * improve coverage to at least 95%
* make sktime more usable
    * make module and submodule structure consistent:`sktime.<module>.<submodule>` where `<module>` refers to a main scitype (e.g. classification or forecasting) and `<submodule>` refers to a family of algorithms
    * have an easy installation process for all platforms, for just core package or all extra packages
    * reduce warnings
* make sktime more deployable
    * support for logging
    * persistence of fitted models
    * caching in pipelines, grid-search, etc
* make sktime more maintainable
    * keep dependencies in core package to a minimum
    * have a docs generation process without warnings (fail on warnings)
    * convert most tutorial notebooks into Python files, except basic intro notebooks run during docs generation


### Project management and operations
> Descriptions of work items for core areas

Project management structure - tech, agile
Operational structure - sktime as entity

#### Short Term
> * This is a tactical set of tasks we can implement to help us move toward our medium- and long- term goals. 
> * Focus is on next 6 months (3 releases)

* set up agile project boards for all work streams
    * weekly stand-ups (in-person or written)
    * agile board manager
    * work stream architect
    * team members
    * kanban: todo; todo priority; doing; review; done
    * developer board: active/inactive (notes with GitHub IDs)
* simple agile process running
    * agile board manager ensuring reviews take place
    * regular triage
    * defined work streams
* bugfixing board
    * weekly stand-ups
    * agile board manager
    * to start, integrate with topical boards
    * kanban: reported; verified; investigating; fixing; review; done
* integration of paid maintainers
    * charter for volunteer contributors vs paid maintainers
    * updated governance document
    * maintenance projects set up - bugs, docs, focus areas

#### Medium Term
> * This is akin to an organization’s annual operating plan
> * What are our priorities for new modules, functionality within modules, etc)? 
> * Do we intend to have completed a first draft of user guide content in a year?
> * Focus is on next year

* sktime becomes a legal entity
    * contributor model
    * legal set-up specified and implemented
    * trademarks
    * operational policies
    * documented on governance page
* discussions with open source umbrellas concluded
    * Linux Foundation
    * numfocus
    * other options arising
* finance operations established
    * regular revenue streams - industry engagement
    * accounting/bursar/treasurer role
    * monthly budget reports
    * documented on governance page 
    * dedicated roles
* strategic operations established
    * regular (e.g., yearly) strategy sessions
    * regular strategy reports/updates
    * established key performance indicators (KPIs) & success control
    * dedicated roles
* internship pipeline all year round
    * get process back up running
    * interview and applicant pipeline
    * dedicated roles
* bugfixing team, dedicated process
    * paid maintainer focus
    * separate workstream & process
    * keep integration with topical streams

#### Long Term

> Focus is on next 5-10 years

* sustainable revenue streams, targeting $100k-1M/year long-term
* entity, e.g., charity, independent research organisation status, possibly as part of consortium (OS or academia), or stand-alone
* integrated operations with academic partners
* integrated operations with industry partners
* replicating operations and governance model to other projects


### Community building, outreach and marketing
> sktime is a community of practice that brings value to both its members and users. Provide regular collaborative/upskilling sessions; create informative content and share it on social media.

#### Short term
- make 2 posts on hashnode and corresponding threads to Twitter + LinkedIn posts (according to format)
- create a todo board on github projects 
- inventory of existing material, posts etc
- reuse existing code snippets, break down tutorials

#### Middle term
- collect good first issues 
- present sktime on a conference similar to pyData (tutorials)
- create a FAQ on the website (especially Windows OS installation, fbprophet issues)
- go through the instructions for windows os, and fix them/update
- record onboarding day one
- record a video on developer setup
- create a collaborative material with other communities/bloggers
- find people who are interested in forecasting but currently don't look at it from data science perspective 
- interactive tutorials (sth like dev days)

#### Long term goals

- created extensive library of learning materials (articles, videos on how to use sktime, on core concepts and best practices of working with time series data)
- robust documentation website (inspiration - sklearn)
- content creation (biweekly articles/posts/videos on social media)
- annual sktime conference with workshops, tutorials (extended sktime dev-days)

### Benchmarking, metrics and statistical tests

#### Short-term

- Separate (and then complete) PR on forecasting loss functions sample-by-sample into:
    - minor refactor of classes (try to use tags to reduce base classes and mixins)
    - Add ability to calculate sample based losses
- Add forecasting performance metric user guide
- Add forecasting performance metrics for measuring "sucess" (e.g. R-Squared, Covariance/Correlation between prediction and actual)
- Add directional accuracy metric
    - Need to re-evaluate interface we proposed way back when
- Complete initial BaseStatisticalTest and unit tests
- Add several concrete implementations of diagnostic and post-hoc statistical tests
    - Diagnostic
        - Seasonality
        - Stationarity
        - Ljung-Box
    - Post-hoc
        - Diebold-Mariano
        - Efficiency
        - Encompassing
        - Directional
            - Runs test
            - Pesaran-Timmerman
        

#### Medium-term

- Add sktime implementations for metrics for learning tasks beyond forecasting:
    - clustering
    - classification
- Add forecasting metrics for evaluating probabilistic/interval/quantile forecasts
- Identify and add datasets that can be used to benchmark different learning tasks and highlight differences between algorithms

#### Long-term

- Finalize framework for benchmarking algorithms (running experiments and then analyzing results) for:
    - annotation (anomaly detection)
    - forecasting
    - classification
    - clustering
    - regression
- Create user-facing benchmark reporting
    - Add new section to documentation

- sktime should include "common" metrics (from literature/books) for:

    - clustering
    - classification
    - regression and forecasting
    - annotation
        - really just an application of other metrics in a certain way

- sktime should include diagnostic tests to aid manual model selection and inspection, as well as post-hoc tests to evaluate properties of model predictions (and compare model predictions against one another).

### Forecasting: general

#### Short term
- pipelining (consolidation, see [STEP](https://github.com/sktime/enhancement-proposals/blob/main/steps/01_forecasting_api/forecasting_pipeline.md) Pipelining)
- more multivariate forecasters (e.g. VECM)
- multivariate make_reduction
- compositions based on decompositions (e.g. STL)
- stabilization based on feedback/bugs from industry applications
- More ensemble algorithms implemented in AutoEnsembleForecaster
- efficient ensembling of fitted models

#### Middle term
- integration of forecasting API into mlflow (not only forecasting related?)
- panel forecasting
- HTS
- Forecasting algorithm overview 
    - describing the properties of them and showing on what kind of data they are performing well
    - comparison of algorithms and user guidance

#### Long term goals
- Explainable AI (XAI) sub-module as part of forecasting module. (XAI for forecasting is a research gap currently.)
- More forecasting algorithms implementations directly in sktime instead wrapping from other packages.
- Forecasting interface established as interface standard, so that other FOSS packages have adopted it.
- Complete coverage of traditional forecasting algorithms
- Probabilistic forecasting (confidence intervals)
- Good date/time related functionality (estimators, transformations, plotting, etc) 

## Progress Report
> Synopsis overall (1-2 sentences)

### Documentation
> Bullet-point summary of progress, updated throughout development
> 
> For example:
> - Created new website
> - Cleaned 20 of 80 class docstrings


## Transformations, pipelines

### Short-term

* finish transformer refactor, proper tests
* 

### Mid-term
* Add transformer caching to pipelines

### Long-term

## Milestones & Issues
> milestones for releases 
> link to milestones for next releases


## References
* "The State of our Roadmaps" by Ralf Gommers, https://www.slideshare.net/RalfGommers/numfocussummit2018roadmapssession
