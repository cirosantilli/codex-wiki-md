# Leave-one-out residual identity for a linear smoother

↑ **Parent:** [Leave-one-out cross-validation](leave-one-out-cross-validation.md)

If a linear smoother has fitted vector $\widehat Y=HY$, its residual after fitting without observation $i$ is

$$
Y_i-\widehat Y_{-i,i}=\frac{Y_i-\widehat Y_i}{1-H_{ii}}.
$$

The identity follows from a [block matrix inverse](block-matrix-inverse.md) or a rank-one inverse update.

## ↑ Ancestors (9)

1. [Leave-one-out cross-validation](leave-one-out-cross-validation.md)
2. [Cross-validation](cross-validation.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/5/b/solution.md)
