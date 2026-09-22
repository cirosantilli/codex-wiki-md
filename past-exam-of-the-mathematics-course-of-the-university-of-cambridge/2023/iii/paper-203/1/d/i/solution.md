<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $A_r=[-r,r]\times(0,1]$ and take $r\geq1$. By the [Brownian representation of half-plane capacity](../../../../../../../brownian-representation-of-half-plane-capacity.md),

$$
\operatorname{hcap}(A_r)
=\lim_{y\to\infty}y\,
\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

On hitting $A_r$, the exit height is at most one. Moreover, $A_r$ lies in the half-disc of radius $\sqrt{r^2+1}\leq2r$. The [harmonic measure](../../../../../../../harmonic-measure.md) of that semicircle as viewed from $iy$ is $O(r/y)$: mapping its exterior to $\mathbb H$ by $z\mapsto z+(2r)^2/z$ reduces the estimate to the [Poisson kernel for the upper half-plane](../../../../../../../poisson-kernel-for-the-upper-half-plane.md) on an interval of length $O(r)$. Consequently

$$
\mathbb E_{iy}[\operatorname{Im}B_\tau]\leq\frac{Cr}{y}
$$

for large $y$, and $\operatorname{hcap}(A_r)\leq Cr$. This is the [half-plane capacity of a low rectangle](../../../../../../../half-plane-capacity-of-a-low-rectangle.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
