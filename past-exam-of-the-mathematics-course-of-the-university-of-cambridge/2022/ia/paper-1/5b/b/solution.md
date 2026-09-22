<h1 id="5b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because the sphere passes through the origin and has centre $P$, its radius is $|P|$. A point $X$ lies on it exactly when

$$
|X-P|^2=|P|^2,
$$

or equivalently

$$
2P\cdot X=|X|^2.
$$

With $P=\alpha A+\beta B+\gamma C$, the three required equations are the [Gram matrix](../../../../../../gram-matrix.md) system

$$
\begin{pmatrix}
A\cdot A&A\cdot B&A\cdot C\\
B\cdot A&B\cdot B&B\cdot C\\
C\cdot A&C\cdot B&C\cdot C
\end{pmatrix}
\begin{pmatrix}\alpha\\\beta\\\gamma\end{pmatrix}
=\frac12
\begin{pmatrix}|A|^2\\|B|^2\\|C|^2\end{pmatrix}.
$$

For the specified vectors this becomes

$$
\alpha+\beta=\frac12,\qquad
\alpha+2\beta+\gamma=1,\qquad
\beta+5\gamma=\frac52.
$$

Thus

$$
\alpha=\frac12,\qquad\beta=0,\qquad\gamma=\frac12,
$$

and the centre is

$$
\boxed{P=\frac12A+\frac12C
=\left(\frac12,\frac12,1\right)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5B](../../5b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
