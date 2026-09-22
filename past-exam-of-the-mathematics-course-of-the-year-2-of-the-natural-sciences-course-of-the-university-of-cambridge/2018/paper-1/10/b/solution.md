<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiply the separated [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) by real $R$ and apply [integration by parts](../../../../../integration-by-parts.md):

$$
\nu\int_0^1rR^2\,dr
=-\int_0^1R(r\kappa R')'\,dr
=-[r\kappa RR']_0^1+\int_0^1r\kappa R'^2\,dr.
$$

The outer endpoint term vanishes because $R(1)=0$. At zero, regularity gives vanishing radial flux. This can be obtained from the equation without assuming a bounded [derivative](../../../../../derivative.md): let $F=r\kappa R'$. Since $F'=-\nu rR$ and $R$ is bounded, $F$ has a finite limit at zero. If that limit were nonzero, positive bounded [thermal diffusivity](../../../../../thermal-diffusivity.md) would make $R'$ have fixed sign and magnitude at least a constant times $1/r$ sufficiently near zero, contradicting bounded $R$. Hence $F(0)=0$, and in fact $F(r)=-\nu\int_0^r sR(s)\,ds=O(r^2)$. This also forces $RF\to0$ for bounded $R$.

The boundary terms therefore vanish, proving

$$
\boxed{\nu\int_0^1rR^2\,dr=\int_0^1r\kappa(r)R'(r)^2\,dr}.
$$

As usual for diffusion, $\kappa$ is nonnegative and positive for $0<r\leq1$; the later power-law case may vanish at the centre. The argument applies in that case as well.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
