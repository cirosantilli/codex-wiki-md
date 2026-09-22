<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [bounded linear operator](../../../../../../continuous-linear-operator.md) $K:U\to V$ between [Hilbert spaces](../../../../../../hilbert-space-split.md), the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) assigns to each admissible datum its unique [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md). Its domain is

$$
\boxed{\mathcal D(K^\dagger)=\operatorname{ran}K\oplus(\operatorname{ran}K)^\perp.}
$$

Write $f=Ku+h$, where $u\in(\ker K)^\perp$ and $h\in(\operatorname{ran}K)^\perp=\ker K^*$. Then $K^\dagger f=u$. Restricting to $(\ker K)^\perp$ removes the ambiguity among solutions differing by an element of the [kernel](../../../../../../kernel-of-a-linear-map.md). The [orthogonal decomposition](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) also shows that $KK^\dagger f$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) of $f$ onto $\overline{\operatorname{ran}K}$, and $K^\dagger Ku$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) of $u$ onto $(\ker K)^\perp$. The inverse is defined on a dense domain and need not be a [bounded linear operator](../../../../../../continuous-linear-operator.md) when the range is not closed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
