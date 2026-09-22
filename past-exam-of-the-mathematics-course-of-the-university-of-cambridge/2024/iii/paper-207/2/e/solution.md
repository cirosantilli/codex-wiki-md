<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Under $H_0$, $(Z_1,Z_2)$ is a [bivariate standard normal distribution](../../../../../../bivariate-standard-normal-distribution.md) with correlation $\rho=\sqrt{m_1/m_2}$. Rejection occurs either at stage 1 through $Z_1\geq u_1$, or at stage 2 through $Z_2\geq u_2$ after continuation $l_1<Z_1<u_1$. Hence the [Type I error](../../../../../../type-i-and-type-ii-errors.md) is

$$
\alpha_{\mathrm{actual}}
=\mathbb P_0(Z_1\geq u_1)
+\mathbb P_0(l_1<Z_1<u_1,,Z_2\geq u_2)
$$



$$
=1-\Phi(u_1)+
\int_{l_1}^{u_1}\phi(z)
\left[1-\Phi\!\left(\frac{u_2-\rho z}{\sqrt{1-\rho^2}}\right)\right]dz.
$$

The final lack-of-benefit boundary $l_2$ affects acceptance, but not the probability of crossing an efficacy boundary.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
