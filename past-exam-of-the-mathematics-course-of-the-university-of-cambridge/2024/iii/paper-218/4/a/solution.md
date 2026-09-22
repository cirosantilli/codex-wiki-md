<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $X_i^*=(1,X_i^T)^T$ and $\gamma=(\gamma_0,\beta^T)^T$, a linear [support vector machine](../../../../../../support-vector-machine.md) predicts

$$
\widehat C_\gamma(x)=\operatorname{sign}(\gamma_0+x^T\beta).
$$

One penalized formulation minimizes empirical [hinge loss](../../../../../../hinge-loss.md) plus a squared [Euclidean norm](../../../../../../euclidean-norm.md) penalty:

$$
\widehat\gamma\in\underset{\gamma\in\mathbb R^{p+1}}{\operatorname{argmin}}
\left\{
\sum_{i=1}^n\max(0,1-Y_iX_i^{*T}\gamma)
+\lambda\|\gamma\|_2^2
\right\},
\qquad \lambda>0.
$$

Conventions often leave the intercept unpenalized, replacing $\|\gamma\|_2^2$ by $\|\beta\|_2^2$; this does not change the role of the two terms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
