<h1 id="3i/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With rows indexed by outputs $A,B,\star$ and columns by inputs $A,B$, the channel matrix is

$$
\boxed{
\begin{pmatrix}
1/2&0\\
0&1/2\\
1/2&1/2
\end{pmatrix}}.
$$

This is a [binary erasure channel](../../../../../../../binary-erasure-channel.md) with erasure probability $1/2$. Conditional on no erasure, the input is recovered exactly, whereas an erasure supplies no information. Thus

$$
I(X;Y)=\frac12H(X),
$$

which is maximized by the uniform input distribution. Therefore

$$
\boxed{C=\frac12\text{ bit}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3I](../../../3i.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
