<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the invariant set $C$ is nonempty, as required for any fixed-point assertion. For $x\in C$, put $r(x)=\sup_{c\in C}\|x-c\|$ and $r_*=\inf_{x\in C}r(x)$. Boundedness makes these finite. The parallelogram identity gives, for $x,y\in C$,

$$
r\left(\frac{x+y}{2}\right)^2
\leq\frac{r(x)^2+r(y)^2}{2}-\frac{\|x-y\|^2}{4}.
$$

The midpoint lies in $C$, so a minimizing sequence $x_n$ satisfies

$$
\|x_n-x_m\|^2\leq2r(x_n)^2+2r(x_m)^2-4r_*^2\longrightarrow0.
$$

Since $C$ is closed in a [Hilbert space](../../../../../../hilbert-space-split.md), the sequence converges to $x_*\in C$. The function $r$ is 1-Lipschitz, hence $r(x_*)=r_*$. The same midpoint inequality proves uniqueness of this minimizing center.

An affine isometry from the [group](../../../../../../group-split.md) maps $C$ onto itself, since its inverse also preserves $C$. Therefore it preserves $r$ and sends its unique minimizer to another minimizer. Uniqueness gives

$$
\boxed{gx_*=x_*\quad\text{for every group element }g.}
$$

This proof applies to a closed bounded convex subset, the substantive meaning of the printed “convex subspace”; if it is literally a bounded [vector](../../../../../../vector.md) subspace, it is just the zero subspace.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
