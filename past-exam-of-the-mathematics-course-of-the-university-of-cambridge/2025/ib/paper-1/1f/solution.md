<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

The Leibniz definition is

$$
\det A=\sum_{\pi\in S_n}\operatorname{sgn}(\pi)\prod_{i=1}^nA_{i,\pi(i)}.
$$

The adjugate is the transpose of the cofactor [matrix](../../../../../matrix.md). Cofactor expansion gives

$$
A\operatorname{adj}(A)=\operatorname{adj}(A)A=(\det A)I.
$$

For the displayed tridiagonal [matrix](../../../../../matrix.md), expansion along the last row gives $D_n=2D_{n-1}-D_{n-2}$, with $D_1=2,D_2=3$. Induction yields

$$
\boxed{\det A_n=D_n=n+1.}
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
