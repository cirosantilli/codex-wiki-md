<h1 id="26j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $W=\sqrt{1+h_x^2+h_y^2}$. An upward-pointing Gauss map is

$$
N=\frac{(-h_x,-h_y,1)}{W}.
$$

For [tangent vectors](../../../../../../tangent-vector.md) $v,w$, [differentiation](../../../../../../differentiation.md) of

$$
d\phi_t=d\phi+t\,dN
$$

gives

$$
\left.\frac d{dt}\right|_{t=0}I^{S_t}(v,w)
=\langle dN(v),d\phi(w)\rangle
 +\langle d\phi(v),dN(w)\rangle.
$$

The Weingarten map is self-adjoint and $S=-dN$, so the right side is $-2II^S(v,w)$. Hence

$$
II^S=-\frac12\left.\frac d{dt}\right|_{t=0}I^{S_t}.
$$

Alternatively differentiating $\langle N,\phi_i\rangle=0$ gives

$$
II_{ij}=-\langle N_i,\phi_j\rangle
       =\langle N,\phi_{ij}\rangle.
$$

Therefore

$$
\boxed{
II^S=\frac1W
\begin{pmatrix}
h_{xx}&h_{xy}\\
h_{xy}&h_{yy}
\end{pmatrix}.}
$$

This is the [fundamental forms of a graph surface](../../../../../../fundamental-forms-of-a-graph-surface.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26J](../../26j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
