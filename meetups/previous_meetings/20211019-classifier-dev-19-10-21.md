# sktime classifier dev meetings 19/10/21
###### tags: `sktime`


Here: Tony, Matt, Chris and Jay

There are currently 32 open issues and 6 prs. Next meeting we will review all classification open issues and PRs. We will then move to project management on github. First there are some known required improvements: Priorities

1. Revise base class: move tags up, tidy up. (Tony/Matt)
https://github.com/alan-turing-institute/sktime/pull/1517

https://github.com/alan-turing-institute/sktime/issues/981

Add type hints

2. Refactor coerce_X_to_numpy tags (Tony, maybe delay this)
3. Review classification template (Tony)
4. Update all docstrings
https://github.com/alan-turing-institute/sktime/issues/1521
5. Refactor for fit/_fit (Tony/Matthew)
https://github.com/alan-turing-institute/sktime/issues/1146

6. purge cython (Chris/Jay/?)
    6.1 distances and NN classifier
https://github.com/alan-turing-institute/sktime/issues/1039
    6.2 MrSEQL
    
7. Contractable interface
https://github.com/alan-turing-institute/sktime/issues/159

not sure if we just use tags or a mixin. Tony to talk to Franz/Markus

Mixin for TrainEstimate more logical as there are abstract methods

8. Update notebooks and examples
https://github.com/alan-turing-institute/sktime/issues/878

9. Split checking and data conversion (Tony): include ability to accept 2D input:   check_input(X,y), check_capabilities(X,y), refactor_input(X)
https://github.com/alan-turing-institute/sktime/issues/1537
10. Refactor/merge distances dists_and_metrs
11. Refactor series_as_features
https://github.com/alan-turing-institute/sktime/issues/212
Options:
    1. Common base class (current model)
    2. Classifier inherits from Regressor
    3. static methods in either Classifier or Regressor

Solution: have it as a transformer: look in detail. Consider with transformer work. 

12. new cor dev from cs?
13. Sort out benchmarking and results evaluator https://github.com/alan-turing-institute/sktime/issues/141  
14. speed up unit tests
Many still test on gunpoint and italy. Move to only unit tests. Original shapelet transform
15. Other stuff
https://github.com/alan-turing-institute/sktime/issues/906
16. Tidy up rocket?
https://github.com/alan-turing-institute/sktime/issues/1095
17. check compliance with all scikit-learn functionality, e.g. parameter tuning

18. Distances: the big refactor maybe raise an issue at the next big meeting




