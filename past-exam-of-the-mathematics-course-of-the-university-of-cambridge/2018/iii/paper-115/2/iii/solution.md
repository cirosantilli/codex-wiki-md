<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The printed hint is impossible: if $\int_0^1f=0$, then

$$
\int_0^1f(s)\left(\int_0^sf(t)\,dt\right)ds
=\frac12\left(\int_0^1f\right)^2=0.
$$

Changing the order of integration gives the same zero, so the additional condition involving $\int tf$ cannot repair it. Using the same function in both proposed controls cannot generate an arbitrary third coordinate.

Instead, put $\Delta=P_z-P_xP_y/2$, $a=2(\Delta+P_x)$, and choose two different oscillatory controls:

$$
\boxed{\alpha(t)=P_x+a\cos(2\pi t),\qquad
\beta(t)=P_y+2\pi\sin(2\pi t).}
$$

Their integrals give $x(t)=P_xt+a\sin(2\pi t)/(2\pi)$ and $y(t)=P_yt+1-\cos(2\pi t)$, hence $x(1)=P_x$ and $y(1)=P_y$. The third endpoint is

$$
z(1)=\int_0^1x(t)\beta(t)\,dt
=\frac{P_xP_y}{2}-P_x+\frac a2=P_z.
$$

The resulting curve is smooth and horizontal at every time, proving [smooth horizontal reachability in the real Heisenberg group](../../../../../../smooth-horizontal-reachability-in-the-real-heisenberg-group.md).

If the [Heisenberg horizontal distribution](../../../../../../heisenberg-horizontal-distribution.md) were an [integrable distribution](../../../../../../integrable-distribution.md), every horizontal curve from the identity would remain in its maximal connected integral leaf. Reachability would force that two-dimensional leaf to be the whole three-dimensional group, contradicting the local leaf coordinates of the [Frobenius theorem](../../../../../../frobenius-theorem.md). The bracket computation in part (i) gives the same obstruction directly.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
