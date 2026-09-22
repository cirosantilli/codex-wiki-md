<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

The value $f(\mathbf a,\mathbf b,\mathbf c)$ is twice the [signed area](../../../../../../signed-area.md) of the [triangle](../../../../../../triangle.md) traversed in that order; it is positive for counterclockwise [orientation](../../../../../../orientation-of-a-simplex.md). Choose [points](../../../../../../point-geometry.md) on the [parabola](../../../../../../parabola.md)

$$
\boxed{\mathbf p_i=(i,i^2),\qquad 1\le i\le n.}
$$

For $i<j<k$, subtracting the first row in the [determinant](../../../../../../determinant.md) and factoring gives

$$
\begin{aligned}
f(\mathbf p_i,\mathbf p_j,\mathbf p_k)
&=(j-i)(k^2-i^2)-(k-i)(j^2-i^2)\\
&=(j-i)(k-i)(k-j)>0.
\end{aligned}
$$

Each of the three factors is positive, proving the required property for every [integer](../../../../../../integer-split.md) $n\ge3$.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [1](../../1.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
