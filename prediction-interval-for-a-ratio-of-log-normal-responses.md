# Prediction interval for a ratio of log-normal responses

↑ **Parent:** [Prediction interval](prediction-interval.md)

Suppose independent future log responses satisfy $Z_j=x_j^T\beta+\varepsilon_j$, where the errors have variance $\sigma^2$. Conditional on a fitted [normal linear model](normal-linear-model.md), the predicted log ratio $Z_1-Z_2$ has estimated mean $(x_1-x_2)^T\widehat\beta$ and estimated variance

$$
(x_1-x_2)^T\widehat{\operatorname{Var}}(\widehat\beta)(x_1-x_2)+2\widehat\sigma^2.
$$

A [Student t interval](student-t-confidence-interval.md) on this logarithmic scale can be exponentiated to obtain a prediction interval for the positive ratio.

## ↑ Ancestors (6)

1. [Prediction interval](prediction-interval.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/13j/iii/solution.md)
