<h1 id="19d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a nonzero real vector $v$, its [Householder reflection](../../../../../../householder-transformation.md) is

$$
\boxed{H=I-2\frac{vv^T}{v^Tv}.}
$$

Let $P=vv^T/(v^Tv)$. Then $P^T=P$ and $P^2=P$, so

$$
H^TH=(I-2P)^2=I-4P+4P^2=I.
$$

Thus **$H$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md)**, and it is also symmetric with $H^{-1}=H$. It sends $v$ to $-v$ and fixes every vector perpendicular to $v$, explaining the reflection in the hyperplane $v^\perp$. For a target reduction of a vector $a$ to $\|a\|e_1$, choose $v=a-\|a\|e_1$ when this vector is nonzero; an alternative sign avoids cancellation in numerical implementations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19D](../../19d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
