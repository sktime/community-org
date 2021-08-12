# Sprint planning 

**Session:** [name/topic]

**Reporter:** [name of reporter]


### :wave: Roll call
- [name=Markus (he/him)] / PhD student at UCL / t: [@mloning_](https://twitter.com/mloning_) / gh: [@mloning](https://github.com/mloning) :turtle: 
- ...

### :bulb: Define the workstream *scope* (10min)

What is the area to work on during the dev days, as a group?
Be as specific as you can, without going to go into details.

:::info

**Example:** (sklearn pipeline) extending the capability of `scikit-learn` pipelines to allow transformers to operate on sub-sets of features

(if this exercise would be done before `FeatureUnion` and `ColumnTransformer` exists)

Note: "pipelines" is not specific enough; talking about `FeatureUnion` etc is too specific at this stage.
:::

### :construction: Collect related issues (15min)

Only issues that *already exist*.

Make notes for issues you think you might need (don´t create them yet on GitHub, just make notes).


### :mag: High-level work plan (20min)

Identify the most important work items, in bullet points.
Identify which are crucial dependencies, which are optional.
Estimate how much time the work will roughly take.
Tentatively put names against the work items.

Think carefully about:
* what is realistic to achieve during the dev sprint (3 days)
* what should go on longer roadmap
* which items are "good first issues", which ones are expert issues

Create a work plan for the week. Prioritize so crucial items are covered. 
Ensure there are a number of "good first issues" for new community members

:::info

**Example:** (sklearn pipeline)

* re-factor design for pipeline - components needed? construction syntax? user journey? (may highlight need for `FeatureUnion` and `ColumnTransformer` or others) - don't forget to save some time for planning and design before starting to hack along!
* improving docstrings for existing pipeline (not too great, so newcomers can't contribute) - good first issue
* `ColumnTransformer` needed (may be easier to spot than need for `FeatureUnion`) - good first issue
* user testing existing pipeline features, may highlight syntax and user journey design directions - good first issue
* looking for existing workarounds on the internet - good first issue
* refactoring of pipeline interface to make it more modular - expert issue(s)
* ambitious roadmap item: network pipeline; support for pandas data frames
:::


### :pencil: Prepare the report-out (10min)

The reporter should prepare a quick summary of the above.

Markdown is perfectly fine here, but can also be PowerPoint or Paint.


### :wrench: Create issues (15min, can also be done later & iteratively)

Turn the high-level work plan into issues!

Write descriptive issue descriptions, with a clear definition of "done".

Consider using "checkbox items" to create sub-tasks - i.e., use `-[]` in the issue description.

Consider using a project board (but don't overcomplicate it) or linking the issue to an existing board. 

Add issue tags. 

:::info

**Example:** (sklearn pipeline)
Create issues on GitHub about:
* Implementing `ColumnTransformer`
* Implementing `FeatureUnion`
* Updating existing pipeline class
* Update docs
:::


