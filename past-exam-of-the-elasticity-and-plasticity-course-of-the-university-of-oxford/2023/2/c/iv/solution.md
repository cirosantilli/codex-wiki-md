<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The net upward [force](../../../../../force-split.md) is the sum of the contact [point forces](../../../../../point-force.md), since the distributed [normal contact force](../../../../../normal-contact-force.md) vanishes in every regime here. Before contact it is zero. During isolated contact it is $R_0=12B(\alpha L-2H)/L^3$. For an interval of contact it is $R_{-s}+R_s=12BH/d^3$, with $d=3H/\alpha$. Therefore

$$
\boxed{F_{\mathrm{up}}(\alpha)=
\begin{cases}
0,&0\leq\alpha\leq2H/L,\\
\dfrac{12B}{L^2}\left(\alpha-\dfrac{2H}{L}\right),
&2H/L\leq\alpha\leq3H/L,\\
\dfrac{4B\alpha^3}{9H^2},&\alpha\geq3H/L.
\end{cases}}
$$

The formulae agree at both transitions. At $\alpha=3H/L$ they give $12BH/L^3$, and their first [derivatives](../../../../../derivative.md) also agree there. As a check on the sign and normalization, integrating the [Euler-Bernoulli beam equation](../../../../../euler-bernoulli-beam-equation.md) over the whole [elastic beam](../../../../../elastic-beam.md) gives $F_{\mathrm{up}}=B(w'''(L^-)-w'''(-L^+))$, which yields the same values.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../../split.md)
6. [Elasticity and plasticity course of the University of Oxford](../../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
