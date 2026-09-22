<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because $\partial_u=\sqrt g\,\partial_s$ and $\mathbf r_t=U\mathbf n+W\mathbf t$, commuting $\partial_t$ and $\partial_u$ gives

$$
\partial_t\mathbf t=(\partial_sU+kW)\mathbf n.
$$

Preservation of orthonormality then gives

$$
\boxed{
\partial_t
\begin{pmatrix}\mathbf t\\\mathbf n\end{pmatrix}
=
\begin{pmatrix}
0&\partial_sU+kW\\
-\partial_sU-kW&0
\end{pmatrix}
\begin{pmatrix}\mathbf t\\\mathbf n\end{pmatrix}
}.
$$

The tangential derivative of the velocity is

$$
\partial_s\mathbf r_t
=(\partial_sW-kU)\mathbf t
+(\partial_sU+kW)\mathbf n,
$$

so

$$
\boxed{\partial_tg=2g(\partial_sW-kU)}.
$$

Finally commute the $s$ and $t$ derivatives in $\partial_s\mathbf t=k\mathbf n$, accounting for the evolving metric through

$$
[\partial_t,\partial_s]
=-(\partial_sW-kU)\partial_s.
$$

The normal component gives

$$
\boxed{
\partial_tk=(\partial_s^2+k^2)U+W\partial_sk
}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 344](../../../../paper-344-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
