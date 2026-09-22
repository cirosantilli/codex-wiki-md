<h1 id="4/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Conditional on $\mu,\psi>0$, let $\lambda\sim\chi^2_4$ and independently $Z\sim N(0,1)$. The [normal distribution](../../../../../../normal-distribution.md) with the stated [precision parameter](../../../../../../precision-parameter.md) can be generated as

$$
\beta_j=\mu+\frac{2\psi Z}{\sqrt\lambda}.
$$

Therefore

$$
\boxed{\frac{\beta_j-\mu}{\psi}=\frac Z{\sqrt{\lambda/4}}\sim t_4,}
$$

by the defining [normal distribution](../../../../../../normal-distribution.md) and [chi-squared distribution](../../../../../../chi-squared-distribution.md) representation of [Student's t-distribution](../../../../../../student-s-t-distribution.md). Its density is

$$
f(\beta_j\mid\mu,\psi)=\frac3{8\psi}\left(1+\frac{(\beta_j-\mu)^2}{4\psi^2}\right)^{-5/2}.
$$

Thus **$\mu$ is the location and $\psi$ is the scale**, not the [standard deviation](../../../../../../standard-deviation.md): $\operatorname{Var}(\beta_j\mid\mu,\psi)=2\psi^2$. Each study gets its own independent chi-squared draw in this [Student t random-effect model](../../../../../../student-t-random-effect-model.md).

## ↑ Ancestors (11)

1. [H](../h.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
