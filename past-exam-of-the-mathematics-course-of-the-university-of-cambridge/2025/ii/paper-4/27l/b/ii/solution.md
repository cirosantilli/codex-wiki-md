<h1 id="27l/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $T_k=R_k^3$. Part (i) identifies $T_k$ as the $k$th arrival time of a rate

$$
\rho=\frac{4\pi\lambda}{3}
$$

Poisson process. Hence $T_k$ has the gamma density

$$
f_{T_k}(t)=\frac{\rho^k}{(k-1)!}t^{k-1}e^{-\rho t},
\qquad t>0.
$$

The change of variables $t=r^3$, with $dt=3r^2\,dr$, gives the [kth-nearest-neighbour distance in a homogeneous Poisson point process](../../../../../../../kth-nearest-neighbour-distance-in-a-homogeneous-poisson-point-process.md):

$$
\boxed{
f_{R_k}(r)
=\frac{3\rho^k}{(k-1)!}\,
r^{3k-1}e^{-\rho r^3},
\qquad r>0,
\quad
\rho=\frac{4\pi\lambda}{3}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [27L](../../../27l.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
