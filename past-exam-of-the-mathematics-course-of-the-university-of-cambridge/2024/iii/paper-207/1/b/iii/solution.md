<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If [incidence](../../../../../../../incidence-epidemiology.md) grows exponentially, $\Delta_t=C e^{\rho t}$, substitution in the [infectious disease renewal equation](../../../../../../../infectious-disease-renewal-equation.md) gives the discrete [Euler-Lotka equation](../../../../../../../euler-lotka-equation.md)

$$
1=R_t\sum_{i=1}^{t}g_i e^{-\rho i},
\qquad
R_t=\left(\sum_{i=1}^{t}g_i e^{-\rho i}\right)^{-1}.
$$

For $X\sim\operatorname{Geometric}(p)$ on $\{0,1,\ldots\}$, $g_i=\mathbb P(X=i-1)=p(1-p)^{i-1}$. The [finite geometric series](../../../../../../../finite-geometric-series.md) therefore yields

$$
\sum_{i=1}^{t}g_i e^{-\rho i}
=pe^{-\rho}\frac{1-(1-p)^t e^{-\rho t}}{1-(1-p)e^{-\rho}},
$$

and consequently

$$
\boxed{R_t=
\frac{1-(1-p)e^{-\rho}}
{pe^{-\rho}\bigl(1-(1-p)^t e^{-\rho t}\bigr)}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
