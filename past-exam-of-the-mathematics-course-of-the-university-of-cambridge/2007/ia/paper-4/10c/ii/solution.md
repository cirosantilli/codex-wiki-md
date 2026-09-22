<h1 id="10c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\boldsymbol v=\dot{\boldsymbol r}$. The original PDF contains the cross product $\dot{\boldsymbol r}\times\boldsymbol r$; the TeX aid drops its [velocity](../../../../../../velocity.md) dot. Since $\boldsymbol v\times\boldsymbol v=0$, differentiation and the equation of motion give

$$
\frac d{dt}\left[m(\boldsymbol v\times\boldsymbol r)\cdot\boldsymbol B\right]
=m(\ddot{\boldsymbol r}\times\boldsymbol r)\cdot\boldsymbol B
=-e[(\boldsymbol v\times\boldsymbol B)\times\boldsymbol r]\cdot\boldsymbol B.
$$

The radial restoring [force](../../../../../../force.md) contributes no [torque](../../../../../../torque.md). The vector triple-product identity yields

$$
[(\boldsymbol v\times\boldsymbol B)\times\boldsymbol r]\cdot\boldsymbol B
=B^2\boldsymbol v\cdot\boldsymbol r
-(\boldsymbol v\cdot\boldsymbol B)(\boldsymbol r\cdot\boldsymbol B).
$$

Meanwhile

$$
\frac d{dt}\left[\frac e2|\boldsymbol r\times\boldsymbol B|^2\right]
=e(\boldsymbol r\times\boldsymbol B)\cdot(\boldsymbol v\times\boldsymbol B)
=e\left[B^2\boldsymbol r\cdot\boldsymbol v
-(\boldsymbol r\cdot\boldsymbol B)(\boldsymbol v\cdot\boldsymbol B)\right].
$$

The [derivatives](../../../../../../derivative.md) cancel, proving

$$
\boxed{m(\dot{\boldsymbol r}\times\boldsymbol r)\cdot\boldsymbol B
+\frac e2|\boldsymbol r\times\boldsymbol B|^2=\mathrm{constant}.}
$$

This is the [magnetic axial angular-momentum invariant](../../../../../../magnetic-axial-angular-momentum-invariant.md). Its first term is the negative of the ordinary [angular momentum](../../../../../../angular-momentum.md) projected on $\boldsymbol B$; retaining that sign is essential.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10C](../../10c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
