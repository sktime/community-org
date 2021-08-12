# HCrystalball meets sktime

Date: 21/09/2020
Participants: @MichalChromcak, @pavelkrizek, @fkiraly, @mloning

## Technicalities

### Data container
* pd.Series (univariate) and pd.DataFrame (multivariate/exogeneous) seems to be consensus for time-homogeneous setting
* more complications for time-heterogeneous setting (see https://github.com/sktime/enhancement-proposals/blob/master/steps/02_data_container/step.md)
* extra maintenance burden when adding support for time-heterogeneous data and/or multiple accept data input formats
* discussed future development of vector forecasting framework 

Aligned:
* y series should be numpy or series (no multivariate currently)
* exogeneous vars (optional) should be pandas data frame
* defer multivariate and unequally spaced discussion
* deferred - input/output type of y (converted to pandas.series in hc)

### Specification of the forecasting horizon

#### Specification of the forecasting horizon
* support for relative/absolute and loc/iloc specification
* relative (integer steps ahead relative to end of training series)
* absolute (precise timestamps)
* no consensus in time series analysis ecosystem (e.g. statsmodels, pmdarima, sktime, HCrystalball

#### How to pass forecasting horizon
* in HC, as index of X to `predict()`
* in sktime, as separate obj to `predict()`

#### Whether to pass it to fit or to predict 
For models that require fh during fitting:
* HC moves fitting into predicting
* sktime allows to pass fh to `fit`


Consensus:
* HC positive about sktime, will review sktime PR on new horizon then comment

### Composition and pipelining interface
* reduction
```
pipe = Pipeline([
    StandardScaler(), 
    Imputer(),
    SVR()]
)
                
tuned_pipe = GridSearchCV(pipe, sthsth)

forecaster = FancyTabulator(tuned_pipe, lags=3)
```

## Governance/admin
* short-term goal: make HCrystalball compatible with sktime, so that users can go to sktime and easily use HCrystalball or vice versa

next steps:
1. invite to slack server
2. contribute wrapper for HCrystalball to sktime
3. review PR for adding date/time support https://github.com/alan-turing-institute/sktime/pull/392
4. work towards aligning APIs, specifying a common API 
