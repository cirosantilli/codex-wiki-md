<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
\mathbf r_0=\frac{\mathbf a\wedge\mathbf b}{|\mathbf a|^2},\qquad
\mathbf N=\mathbf b+\mathbf a\wedge\mathbf y.
$$

The [vector triple product](../../../../../../vector-triple-product.md) identity $(\mathbf a\wedge\mathbf b)\wedge\mathbf a=|\mathbf a|^2\mathbf b-(\mathbf a\cdot\mathbf b)\mathbf a$ shows that $\mathbf r_0\wedge\mathbf a=\mathbf b$. Moreover, $(\mathbf r-\mathbf r_0)\wedge\mathbf a=\mathbf0$ exactly when $\mathbf r-\mathbf r_0$ is a [scalar multiple](../../../../../../scalar-multiple.md) of $\mathbf a$. Thus the given [line](../../../../../../straight-line.md) is

$$
L=\{\mathbf r_0+t\mathbf a:t\in\mathbb R\}.
$$

Also $\mathbf a\wedge\mathbf r_0=-\mathbf b$, so $\mathbf N=\mathbf a\wedge(\mathbf y-\mathbf r_0)$. The assumption $\mathbf N\ne\mathbf0$ says precisely that $\mathbf y$ is outside $L$. Consequently $L$ and $\mathbf y$ determine a unique [plane](../../../../../../plane.md), with [normal vector](../../../../../../normal-vector.md) $\mathbf N$.

To identify its equation, use cyclic invariance of the [scalar triple product](../../../../../../scalar-triple-product.md):

$$
\mathbf r\cdot(\mathbf a\wedge\mathbf y)
=\mathbf y\cdot(\mathbf r\wedge\mathbf a).
$$

For $\mathbf r\in L$, this equals $\mathbf y\cdot\mathbf b$, while $\mathbf r\cdot\mathbf b=\mathbf r\cdot(\mathbf r\wedge\mathbf a)=0$. Hence $\mathbf r\cdot\mathbf N=\mathbf y\cdot\mathbf b$ throughout $L$. The [point](../../../../../../point-geometry.md) $\mathbf y$ also satisfies that equation because $\mathbf y\cdot(\mathbf a\wedge\mathbf y)=0$. Since $\mathbf N\ne\mathbf0$, the required [plane](../../../../../../plane.md) is therefore exactly

$$
\boxed{\mathbf r\cdot(\mathbf b+\mathbf a\wedge\mathbf y)=\mathbf y\cdot\mathbf b.}
$$

This also proves the reusable [plane through a point and a line given by a cross product](../../../../../../plane-through-a-point-and-a-line-given-by-a-cross-product.md) construction.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
