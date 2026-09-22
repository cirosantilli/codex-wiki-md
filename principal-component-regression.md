# Principal component regression

↑ **Parent:** [Principal component analysis](principal-component-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_component_regression)

Regress a response on selected [principal component scores](principal-component-score.md) of centered predictors. If $X=UDV^T$ is a [singular value decomposition](singular-value-decomposition.md) and the first $q$ positive-singular-value components are retained, the retained score matrix is $U_qD_q$ and the fitted coefficient in predictor coordinates is $V_qD_q^{-1}U_q^Ty$. The fitted centered response is $U_qU_q^Ty$: this follows by applying the [least-squares normal equations](normal-equations-for-linear-least-squares.md) to the orthogonal score columns. Truncating small singular directions limits variance amplification, but directions of large predictor variance need not be those best predicting the response; select $q$ using prediction assessment rather than explained predictor variance alone.

## ↑ Ancestors (8)

1. [Principal component analysis](principal-component-analysis.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/3/ii/solution.md)
