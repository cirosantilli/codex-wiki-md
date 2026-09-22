<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T_i>0$ be record time and let $x_i=(1,c_i,d_i)^T$ contain standardized climb and distance. Model 1 is the [normal linear model](../../../../../../normal-linear-model.md)

$$
T_i=x_i^T\beta+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Model 2 applies the same model after a [logarithmic transformation](../../../../../../logarithmic-transformation.md):

$$
\log T_i=x_i^T\alpha+e_i,
\qquad e_i\overset{\mathrm{iid}}\sim N(0,\tau^2),
$$

so $T_i$ is conditionally log-normal. Model 3 is a [Gamma regression with logarithmic link](../../../../../../gamma-regression-with-logarithmic-link.md):

$$
\boxed{\mathbb E(T_i\mid x_i)=\mu_i,
\qquad
\operatorname{Var}(T_i\mid x_i)=\phi\mu_i^2,
\qquad
\log\mu_i=x_i^T\gamma.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
