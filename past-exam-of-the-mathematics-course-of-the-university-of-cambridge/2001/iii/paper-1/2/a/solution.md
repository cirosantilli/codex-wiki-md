<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Lie algebra](../../../../../../lie-algebra-split.md) of [SL2R](../../../../../../real-special-linear-group-of-degree-two.md) is the space of traceless real two-by-two [matrices](../../../../../../matrix.md). For $A$ in this space, the [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) gives $A^2=cI$, where $c=-\det A$. Expanding the [matrix exponential](../../../../../../matrix-exponential.md), if $c=s^2>0$ then

$$
\exp A=(\cosh s)I+\frac{\sinh s}{s}A,
\qquad \operatorname{tr}(\exp A)=2\cosh s\geq2.
$$

If $c=0$, then $\exp A=I+A$ and its [trace](../../../../../../matrix-trace.md) is $2$. If $c=-s^2<0$, then

$$
\exp A=(\cos s)I+\frac{\sin s}{s}A,
\qquad \operatorname{tr}(\exp A)=2\cos s\in[-2,2].
$$

In every case $\operatorname{tr}(\exp A)\geq-2$. But

$$
g=\begin{pmatrix}-2&0\\0&-1/2\end{pmatrix}
$$

has determinant one and [trace](../../../../../../matrix-trace.md) $-5/2$. Thus $g\in SL_2(\mathbb R)$ is not an exponential, and **the exponential map is not surjective**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
