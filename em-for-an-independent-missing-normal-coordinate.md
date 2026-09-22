# EM for an independent missing normal coordinate

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

For independent normal coordinates, an unobserved first coordinate has conditional law equal to its current marginal [normal distribution](normal-distribution.md), even when the second coordinate of that observation is known. Thus its E-step first moment is $\mu_1^{(t)}$ and second moment is $(\mu_1^{(t)})^2+v_1^{(t)}$. With three observed first coordinates and one missing value, the mean update is $(\sum_{i=1}^3x_{i1}+\mu_1^{(t)})/4$ and the [variance](variance-split.md) update is $[\sum_{i=1}^3(x_{i1}-\mu_1^{(t+1)})^2+v_1^{(t)}+(\mu_1^{(t)}-\mu_1^{(t+1)})^2]/4$. The [conditional variance](conditional-variance.md) term is essential: filling in only the conditional mean is not the [expectation-maximization algorithm](expectation-maximization-algorithm.md).

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/6/solution.md)
