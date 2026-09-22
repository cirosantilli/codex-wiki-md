<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\vartheta=(q,t)$ use the [estimating equation](../../../../../../estimating-equation.md)

$$
\psi(Y,Z;\vartheta)=
\binom{Z-q}{ZY/q-(1-Z)Y/(1-q)-t}.
$$

Its empirical mean vanishes exactly at $(\widehat p,\widehat\tau)$. The population equation has the unique root $(p,\tau^*)$, so the [Z-estimator](../../../../../../z-estimator.md) is consistent. Linearizing the equation, or simplifying the corresponding sandwich covariance, gives the influence function

$$
\phi(Y,Z)
=\frac Zp(Y-\mu_1)-\frac{1-Z}{1-p}(Y-\mu_0).
$$

Hence

$$
\boxed{\sqrt n(\widehat\tau-\tau^*)
\xrightarrow{d}N(0,V_{\mathrm{estimated}}),
\qquad
V_{\mathrm{estimated}}
=\frac{\operatorname{Var}(Y\mid Z=1)}p
+\frac{\operatorname{Var}(Y\mid Z=0)}{1-p}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
