<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [straight line](../../../../../../straight-line.md) $2x=y=z$ has [direction vector](../../../../../../direction-vector.md) $(1,2,2)$, so take the [unit vector](../../../../../../unit-vector.md) $\mathbf n=(1,2,2)^T/3$. A [half-turn](../../../../../../half-turn.md) has $\cos\pi=-1$ and $\sin\pi=0$. The preceding [rotation](../../../../../../rotation-mathematics.md) formula becomes

$$
R(\mathbf v)=2(\mathbf v\cdot\mathbf n)\mathbf n-\mathbf v.
$$

Thus the [rotation matrix](../../../../../../rotation-matrix.md) in the [standard basis](../../../../../../standard-basis.md) is

$$
\boxed{2\mathbf n\mathbf n^T-I=\frac19\begin{pmatrix}-7&4&4\\4&-1&8\\4&8&-1\end{pmatrix}.}
$$

It fixes $(1,2,2)^T$ and negates every [vector](../../../../../../vector.md) in its [orthogonal complement](../../../../../../orthogonal-complement.md), which also checks the [half-turn](../../../../../../half-turn.md) geometrically.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
