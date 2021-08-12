# Roadmap planning meeting

## Contributors
Contributors: @mloning, @fkiraly, @sveameyer13, @lovkush-a, @bilal-196, @GuzalBulatova, @chrisholder, @satya-pattnaik, @aiwalter

Current roadmap: https://github.com/alan-turing-institute/sktime/blob/main/docs/source/roadmap.rst

Time watcher: @lovkush-a

## Agenda: 
Brainstorming: 45 mins
Discussion: 30 mins

---
## Brainstorming
Chris Holder:
* **Clustering**, support sklearn clustering algorithms for time series data
* interface between **distances** (time series) and skleran style clustering
* re-work of metrics - optimized, tested, Numba
* "cool new" time series **algorithms** like k-shapes
* FK: maybe interface to shapes, e.g., Nina's geomstats package
* reducing **test duration**, optimize testing workflow

Guzal Bulatova:
* **multiariate forecasting** module
* keep api consistent/uniform 
* **documentation** before features
* `plot_series` only accepts pd.Series. Refactor it to accept np arrays and dataframes?
* ML: perhaps getting more **end user feedback** & engagement
* user tutorials (different use cases, possibly with videos)

Ahmed Bilal:
* work on classifiers (there area of interst)
* improve functionality, e.g. **multivariate time series classification** and other attributes
* **documentation** should be worked on as a priority, not strong

Satya Pattnaik
* add support for exogenous variables to reduction (forecasting)
* improve **forecasting interface for exogenous data**
* **prediction intervals** in forecasting
* **variants of forecasting** task: panel, multivariate/vector, hierarchical

Lovkush Agarwal:
* frustration: obscure code structure *in parts*, zero documentation in parts
* improve **documentation**
* how to improve quality of research grade code contributions
* pair programming of "researchers" with "software engineers"?

Svea Meyer:
* **unequal length time series** (panel or multivariate)
* **annotation**, especially for EEG/neuro data
* "random" whether transformers support multivariate, extend this! Should be out-of-the-box (e.g., not composition/reduction)
* not always clear whether pandas or numpy is the way to go - inspection should be easy, support should be easy for either
* **documentation**, findability of methods is poor
* documentation, format of data to load is unclear - tagging with univariate, multivariate, exogeneous for available data sets
* maybe transformers should have additional methods? update should be implemented in more transformers
* **transformers design** incoherent/inconsistent, maybe interface refactor or at least interface consolidation
* very long term vision: real time processing, e.g., for BCI. FK: maybe requires refactoring update and making update more consistent across sktime.
* **real time** annotation, e.g., segmentation then classification; ML: related to early TSC?

Taiwo Owoseni:
* frustrations: fit method (forecasting) does not accept numpy, is a frustration. Accepting numpy is user expectation
* documnetation needs to be improved - especially forecasters are not precisely documented
* need for individual documentation format for forecasters?
* frustration: tests take very long

Martin Walter:
* Many topics already covered by current developments
* Dependency to other packages: there is blocker if you want to introduce more dependencies. problem is figuring out the co-dependencies.
* cleaner dependency management, numpy fixed to a range (upper bound) is sub-optimal; perhaps problematic dependencies to move out of core package, available on-demand as different extension package
* unit tests too focused on univariate topic (not exogeneous, not multivariate endogeneous), needs extension
* community growth is important; perhaps more industial contributions

Franz Kiraly:
* multivariate forecasting
* advanced pipelining (e.g. networks, see mlr3pipelines or ADTK) & pipelines across tasks
* new modules: annotation, clustering, sequence-similarity-type tasks
* get documentation straight!
* long term: if critical mass or resource: probabilistic forecasting models, event models (e.g, survival, time-to-event, multi-event or multi-state) - see mlr3proba
    * this is big project. many interacting pieces
* 2nd degree transformers
* proper benchmarking, replicate & publish 
* lower priority tasks: supervised forecasting, functional prediction

Markus Loning:
* biggest blocker for wider adoption (for users and dev) is lack of really good documentation
* agree with most points already said: multivariate forecasting, probabilitic forecasts, annotation (at least simple ones like outlier detection)
* time series regression
* once we have multiple tasks - solid reduction interface to go from one task to another. current reduction interface(s) not general and not clear
* code structure. agree with martin that need to improve dependency management. maybe have structured way of having companion packages
    * FK: we could copy mlr3 model? or MLJ model?
* improve unit testing, and have template package to allow other ppl to create sister packages easily
* community: have other types of meetings/groups. more regular meetings. the community group is good starting point
* deep learning. it is popular, so should have sktime-dl up to speed. common feedback from people markus talks to
* unequal length. might need to deprecate nested pandas dataframe. probably better to make use of awkward array (this would be long-term)
    * FK. agree with awkward array, but think we should support multiple data types (incl np.array and pd.stuff)

Svea asked whether forecasting is main focus of sktime?
* Current meeting is biased towards who is in the call
* Tony and their team are similar size to team on forecasting. also, classification is probably more well developed than forecasters
* Nice thing about sktime is that by design/philosophy, it does not prioritise one task over another


---

Stars indicate priorties, only voted on technical topics, excluding the "community building" topic. 

## Topics (collected)

### Documentation :star::star::star::star::star::star::star::star:
* Core documentation needs to be created "properly"
* Tutorials, examples
* Extension guidelines
* For research algorithms, possibly pairing up researchers with 'engineer' to improve readability/documentation

### Refactoring/extending capabilities of existing modules :star::star::star::star::star::star:
* Forecasting: multivariate, exogeneity
* Unequal length time series
* Input type support or conversion (awkward array etc)
* Real-time interface, stream/update capability
* Forecasting: prediction intervals
* Refactoring: TSC, transformers
* Distance metrics
* Reduction interface
* Advanced pipelines
* Clustering evaluation

### New modules & algorithms :star::star::star::star::star::star:
* Annotation
* Clustering
    - Get clustering into next version of sktime
    - Implement wrapper around all the sklearn clusterers
    - Implement time series specific clustering algorithms (i.e. k-shapes)
* Probabilistic interface, event modelling 
* Panel & supervised forecasting
* Time series regression
* sequence-similarity tasks

### Software engineering & dev ops :star::star::star::star::star::star:
* Dependency management
* Template for companion packages
* Continuous integration & unit testing
    - Test refactor
    - Extending unit tests
    - Improving code quality/documentation for "research" grade contribs
    - Reducing total test time

### Community building 
- Integrating "off-line" contributors
- For research algorithms, possibly pairing up researchers with 'engineer' to improve readability/documentation
- Regular meetings



Below is the roadmap to be published on the sktime repo/online docs.

---
# Roadmap draft

Contributors: @mloning, @fkiraly, @sveameyer13, @lovkush-a, @bilal-196, @GuzalBulatova, @chrisholder, @satya-pattnaik, @aiwalter

Created during the 2021 sktime dev days, 25/06/2021.

## Overview


## Documentation
* Core documentation needs to be created "properly"
* Tutorials, examples
* Extension guidelines
* For research algorithms, possibly pairing up researchers with 'engineer' to improve readability/documentation

## Refactoring/extending capabilities of existing modules
* Forecasting: multivariate, exogeneity
* Unequal length time series
* Input type support or conversion (awkward array etc)
* Real-time interface, stream/update capability
* Forecasting: prediction intervals
* Refactoring: TSC, transformers
* Distance metrics
* Reduction interface
* Advanced pipelines
* Clustering evaluation

### New modules & algorithms
* Annotation
* Clustering
    - Get clustering into next version of sktime
    - Implement wrapper around all the sklearn clusterers
    - Implement time series specific clustering algorithms (i.e. k-shapes)
* Probabilistic interface, event modelling 
* Panel & supervised forecasting
* Time series regression
* sequence-similarity tasks

### Software engineering & dev ops
* Dependency management
* Template for companion packages
* Continuous integration & unit testing
    - Test refactor
    - Extending unit tests
    - Improving code quality/documentation for "research" grade contribs
    - Reducing total test time

### Community building 
- Integrating "off-line" contributors
- For research algorithms, possibly pairing up researchers with 'engineer' to improve readability/documentation
- Regular meetings


