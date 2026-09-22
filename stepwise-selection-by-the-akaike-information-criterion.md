# Stepwise selection by the Akaike information criterion

↑ **Parent:** [Akaike information criterion](akaike-information-criterion.md)

Starting from a fitted model, compare admissible single-term additions and deletions within specified lower and upper scopes, retaining hierarchical lower-order terms when an interaction requires them. Select a change reducing the [Akaike information criterion](akaike-information-criterion.md) and repeat until no admissible change improves it. For a Gaussian [normal linear model](normal-linear-model.md) with $N$ observations and $k$ fitted mean coefficients, the criterion used by R's linear-model stepwise search is $N\log(\operatorname{RSS}/N)+2k$, up to constants common to the models. The search is greedy and need not find the best model in the whole scope. Ordinary coefficient tests in the selected model do not account for this [model selection](model-selection.md). The software arguments are documented in [the MASS documentation](https://stat.ethz.ch/R-manual/R-devel/library/MASS/html/stepAIC.html).

**Table of contents**

- [AIC deletion threshold in a normal linear model](aic-deletion-threshold-in-a-normal-linear-model.md)

## ↑ Ancestors (8)

1. [Akaike information criterion](akaike-information-criterion.md)
2. [Model selection](model-selection.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38/1/solution.md)
