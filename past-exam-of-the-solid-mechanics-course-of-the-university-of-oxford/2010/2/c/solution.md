<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [determinant](../../../../determinant.md) condition is $r'(r/R)^2=1$, or $r^2r'=R^2$. Integration gives $r^3=R^3+C$ and the outer boundary value fixes $C=t^3-1$. Thus

$$
\boxed{r(R)=(R^3+t^3-1)^{1/3}.}
$$

For $t>1$, $r(R)$ tends to the positive cavity radius $(t^3-1)^{1/3}$ as $R\downarrow0$. Its tangential stretches grow like that radius divided by $R$, so $|F|\to\infty$. The [deformation](../../../../deformation-mechanics.md) is singular at the origin and is interpreted as a finite-energy Sobolev [deformation](../../../../deformation-mechanics.md), with a point value irrelevant to its energy.

Since $r'=R^2/r^2$ and the [determinant](../../../../determinant.md) penalty is zero almost everywhere,

$$
\boxed{E_{\mathrm{cav}}(t)=4\pi\int_0^1\left(\frac{R^6}{r(R)^4}+2r(R)^2\right)dR.}
$$

For fixed $t>1$, the first integrand is $O(R^6)$ near zero and the second is bounded. Thus the energy is finite despite the unbounded [gradient](../../../../gradient.md). In particular the [gradient](../../../../gradient.md) is square integrable, as required for this competitor.

For large $t$, $r(R)/t\to1$ uniformly on $[0,1]$. The first [integral](../../../../integral-split.md) is $O(t^{-4})$, while $\int_0^1r(R)^2dR\sim t^2$. Consequently

$$
\boxed{E_{\mathrm{cav}}(t)\sim8\pi t^2.}
$$

The spherical [volume](../../../../volume.md) factor $R^2dR$ is what makes the $R^{-1}$ tangential-[gradient](../../../../gradient.md) singularity integrable in three dimensions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
