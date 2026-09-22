<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since $X_j\sim\operatorname{Poisson}(n_j\lambda_j)$, the rate MLE has asymptotic variance $\lambda_j/n_j$. The [delta method](../../../../../../delta-method.md) for the logarithm gives

$$
\operatorname{Var}(\log\widehat\lambda_j)\simeq\frac1{n_j\lambda_j}.
$$

Independence of the arms therefore yields

$$
Z=\frac{\log\widehat\lambda_T-\log\widehat\lambda_C}
{\sqrt{1/(n_T\widehat\lambda_T)+1/(n_C\widehat\lambda_C)}}.
$$

Under $H_0:\lambda_T=\lambda_C=\lambda$, the asymptotic variance of the log rate ratio is

$$
\boxed{\frac1{n_T\lambda}+\frac1{n_C\lambda}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
