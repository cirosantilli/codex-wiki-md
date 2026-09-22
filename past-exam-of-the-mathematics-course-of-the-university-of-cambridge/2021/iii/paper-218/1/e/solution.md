<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For prediction at covariate value $u$, the intercept contributes variance $\sigma^2/n$ in every case because $x$ is centered. The one-copy ridge shrinkage is $a_1=s/(s+\lambda)$, while the duplicated-design total has $a_2=2s/(2s+\lambda)$. Thus

$$
\operatorname{Bias}\widehat m_j(u)=u(a_j-1)\beta_0,
$$

and

$$
\operatorname{Var}\widehat m_1(u)=\frac{\sigma^2}{n}
+\frac{u^2\sigma^2s}{(s+\lambda)^2},
\qquad
\operatorname{Var}\widehat m_2(u)=\frac{\sigma^2}{n}
+\frac{4u^2\sigma^2s}{(2s+\lambda)^2}.
$$

Since $a_2>a_1$, duplication reduces ridge bias and increases variance.

For constrained Lasso, let $Z=z/s\sim N(\beta_0,\sigma^2/s)$ and $C_t(Z)=\max(-t,\min(Z,t))$. Both designs have the identical fitted total $C_t(Z)$, so both have

$$
\operatorname{Bias}\widehat m(u)=u\{\mathbb EC_t(Z)-\beta_0\},
\qquad
\operatorname{Var}\widehat m(u)=\frac{\sigma^2}{n}+u^2\operatorname{Var}\{C_t(Z)\}.
$$

Duplicating the predictor has no effect on Lasso predictions, despite making the coefficient vector nonunique.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
