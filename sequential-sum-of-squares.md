# Sequential sum of squares

↑ **Parent:** [Analysis of variance](analysis-of-variance.md)

For an ordered sequence of nested [linear regression](linear-regression-split.md) models $M_0\subset M_1\subset\cdots$, the sequential sum of squares for the $j$th added term is $\operatorname{RSS}(M_{j-1})-\operatorname{RSS}(M_j)$. These are also called type-I sums of squares. They depend on term order when the design is not orthogonal. Dividing by the number of newly added coefficients and the full model's residual mean square gives the sequential [F-test](f-test.md). A covariate added first is tested before adjustment for later terms, whereas a treatment added after the covariate is tested with that covariate already included.

## ↑ Ancestors (9)

1. [Analysis of variance](analysis-of-variance.md)
2. [Linear regression](linear-regression-split.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
