<h1 id="18d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P=uu^T/(u^Tu)$, well defined because $u\ne0$. It is symmetric and satisfies $P^2=P$, so for the [Householder reflection](../../../../../../householder-transformation.md) $H=I-2P$,

$$
H^TH=(I-2P)^2=I-4P+4P^2=\boxed{I}.
$$

Thus $H$ is orthogonal; it reverses the component parallel to $u$ and fixes the perpendicular hyperplane.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18D](../../18d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
