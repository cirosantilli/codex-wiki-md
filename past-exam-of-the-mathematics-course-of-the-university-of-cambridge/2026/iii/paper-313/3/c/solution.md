<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Represent the [real affine group](../../../../../../orientation-preserving-affine-group-of-the-real-line.md) by

$$
g(a,b)=
\begin{pmatrix}
e^a&b\\0&1
\end{pmatrix}.
$$

Matrix multiplication reproduces

$$
(a,b)(a',b')=(a+a',b+e^ab').
$$

The [Maurer-Cartan form](../../../../../../maurer-cartan-form.md) is

$$
g^{-1}dg=
\begin{pmatrix}
da&e^{-a}db\\0&0
\end{pmatrix},
$$

so a basis of left-invariant one-forms is

$$
\boxed{\sigma^1=da,
\qquad \sigma^2=e^{-a}db}.
$$

The dual left-invariant vector fields are

$$
\boxed{E_1=\partial_a,
\qquad E_2=e^a\partial_b}.
$$

Indeed $\sigma^i(E_j)=\delta^i_j$, and left translation preserves the one-forms and vector fields.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 313](../../../paper-313-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
