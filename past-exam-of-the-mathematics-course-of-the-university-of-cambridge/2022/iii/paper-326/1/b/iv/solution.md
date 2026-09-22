<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [Reverse-order law for the Moore--Penrose inverse](../../../../../../../reverse-order-law-for-the-moore-penrose-inverse.md) is false in general. Take

$$
A=\begin{pmatrix}1&0\\0&2\\0&0\end{pmatrix},
\qquad
B=\begin{pmatrix}1\\1\end{pmatrix}.
$$

Then

$$
(AB)^\dagger=\begin{pmatrix}1/5&2/5&0\end{pmatrix},
\qquad
B^\dagger A^\dagger=\begin{pmatrix}1/2&1/4&0\end{pmatrix}.
$$

A sufficient condition is

$$
\operatorname{rank}(A)=n,
\qquad
\operatorname{rank}(B)=n,
$$

so that $A$ has [full column rank](../../../../../../../full-column-rank.md) and $B$ has [full row rank](../../../../../../../full-row-rank.md). Indeed $A^\dagger A=I_n$ and $BB^\dagger=I_n$; these identities make $B^\dagger A^\dagger$ satisfy all four [Penrose equations](../../../../../../../penrose-equations.md) for $AB$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
