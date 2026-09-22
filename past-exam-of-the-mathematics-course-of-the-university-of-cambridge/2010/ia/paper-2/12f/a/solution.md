<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The nonsingular [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) has $\sigma_1,\sigma_2>0$ and $|\rho|<1$. Put $a=(x_1-\mu_1)/\sigma_1$ and $b=(x_2-\mu_2)/\sigma_2$. Completing the square gives

$$
a^2-2\rho ab+b^2=(b-\rho a)^2+(1-\rho^2)a^2.
$$

Consequently the joint [probability density function](../../../../../../probability-density-function.md) factors as

$$
f_{X_1,X_2}(x_1,x_2)=
\frac{e^{-a^2/2}}{\sqrt{2\pi}\sigma_1}\,
\frac{\exp[-(b-\rho a)^2/(2(1-\rho^2))]}
{\sqrt{2\pi}\sigma_2\sqrt{1-\rho^2}}.
$$

For fixed $x_1$, the second factor is a normalized [normal distribution](../../../../../../normal-distribution.md) density in $x_2$, with mean $\mu_2+\rho\sigma_2a$ and standard deviation $\sigma_2\sqrt{1-\rho^2}$. Its integral is one; explicitly substitute $w=(b-\rho a)/\sqrt{1-\rho^2}$ in the [Gaussian integral](../../../../../../gaussian-integral.md). Thus **the marginal density is**

$$
\boxed{f_{X_1}(x_1)=\frac1{\sqrt{2\pi}\sigma_1}
\exp\left[-\frac{(x_1-\mu_1)^2}{2\sigma_1^2}\right].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
