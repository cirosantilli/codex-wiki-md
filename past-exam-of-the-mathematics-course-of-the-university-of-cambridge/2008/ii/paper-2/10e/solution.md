<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

For a regular spherical star, [mass conservation](../../../../../mass-conservation.md) gives $m'=4\pi r^2\rho$. Multiplying the [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) equation by $r^2/\rho$ and differentiating therefore yields

$$
\boxed{\frac{d}{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G r^2\rho.}
$$

At the center, finite density implies $m(r)=O(r^3)$, so a regular pressure satisfies $P(0)=P_c<\infty$ and $P'(0)=0$. At a free outer boundary in vacuum, $P(R)=0$; a surrounding medium would instead prescribe its external pressure.

Differentiate the auxiliary function, using both equations:

$$
F'=-\frac{Gm\rho}{r^2}+\frac{Gmm'}{4\pi r^4}-\frac{Gm^2}{2\pi r^5}=-\frac{Gm^2}{2\pi r^5}<0
$$

where enclosed mass is nonzero. Since $m^2/r^4\to0$ at the regular center, $F(0)=P_c$, whereas $F(R)=GM^2/(8\pi R^4)$. Integrating the strictly negative derivative gives

$$
\boxed{P_c>\frac{GM^2}{8\pi R^4}.}
$$

With nonzero external pressure, the corresponding bound is $P_c>P(R)+GM^2/(8\pi R^4)$.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
