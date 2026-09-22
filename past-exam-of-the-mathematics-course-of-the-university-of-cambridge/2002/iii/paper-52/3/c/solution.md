<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Constant density in each layer and negligible ambient acceleration far from the front give

$$
\boxed{u_t+uu_x+g'h_x=0.}
$$

This primitive [momentum conservation](../../../../../../momentum-conservation.md) equation remains valid with slowly varying $B$. In conservative form it is

$$
\partial_t(Au)+\partial_x\left(Au^2+\frac{g'Bh^3}{6}\right)=\frac{g'h^3}{6}B',
$$

where the right side is the longitudinal component of the [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) force on the sloping sidewalls. Omitting that term while retaining variable $B$ would give the wrong acceleration.

Together with [volume conservation](../../../../../../volume-conservation.md), the principal coefficient matrix in $(h,u)$ is

$$
\begin{pmatrix}u&h/2\\g'&u\end{pmatrix}.
$$

Its real [eigenvalues](../../../../../../eigenvalue.md) and [characteristic curves](../../../../../../characteristic-curve.md) are

$$
\boxed{\frac{dx}{dt}=u\pm c,\qquad c=\sqrt{\frac{g'h}{2}}.}
$$

These are downstream and upstream [gravity waves](../../../../../../gravity-wave-split.md) relative to the moving fluid. The factor $1/2$ is geometric: the hydraulic depth is $A/b(h)=h/2$. Both waves move downstream in a sufficiently fast current, whereas one can carry information upstream in a slower current.

For $B=1$, differentiate $c^2=g'h/2$ and combine the two equations. The [Riemann invariants](../../../../../../riemann-invariant.md) are

$$
\boxed{\left[\partial_t+(u\pm c)\partial_x\right](u\pm4c)=0.}
$$

For variable $B$ they instead obey

$$
\left[\partial_t+(u\pm c)\partial_x\right](u\pm4c)=\mp cu\frac{B'}B,
$$

which also checks that the invariant claim depends on a prismatic channel.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Section B](../../section-b.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
