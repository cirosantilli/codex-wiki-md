<h1 id="13k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Dividing row $i$ of both $Y$ and $X$ by $\sqrt{v(X_i)}$ transforms the model to one with covariance $\sigma^2I$. Ordinary least squares without an intercept on these transformed data is exactly the estimator in part (a). In R, the unweighted estimator is returned by

```
R
fit2 <- lm(Y ~ X - 1)
fit2$coefficients
```

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13K](../../13k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
