<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [separation of variables](../../../../../separation-of-variables.md), write $B=F(r)\Theta(\theta)$. The exterior [Laplace equation](../../../../../laplace-equation.md) separates into

$$
\frac{(r^2F')'}F=-\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}=\lambda.
$$

With $\mu=\cos\theta$, angular regularity at the poles selects $\lambda=\ell(\ell+1)$ and the [Legendre polynomial](../../../../../legendre-polynomial.md) $P_\ell(\mu)$. The radial equation is $(r^2F')'-\ell(\ell+1)F=0$, an [Euler-Cauchy equation](../../../../../euler-cauchy-equation.md) with solutions $r^\ell,r^{-\ell-1}$. Decay at infinity excludes the first branch for every $\ell$, including its constant $\ell=0$ case. Therefore

$$
\boxed{B_{\rm out}(r,\theta)=\sum_{\ell=0}^\infty A_\ell r^{-\ell-1}P_\ell(\cos\theta),\qquad r>R.}
$$

The expansion uses axisymmetric [spherical harmonics](../../../../../spherical-harmonic.md). The written scalar boundary-value problem permits the $\ell=0$ term; any additional physical exclusion of that sector must be stated separately.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
