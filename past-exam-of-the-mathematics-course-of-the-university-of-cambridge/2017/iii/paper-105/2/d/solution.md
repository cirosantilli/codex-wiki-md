<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A fixed smooth choice $g\equiv0$ already gives a counterexample. Select nonzero smooth functions $\phi(x_1,x_2)$ and $\chi(x_3)$ with product support compactly contained in a small box inside the shell. Let

$$
u_k(x)=\phi(x_1,x_2)\chi(x_3)\sin(kx_3),\qquad
f_k=(\partial_1^2+\partial_2^2)\phi\,\chi\sin(kx_3).
$$

Then $u_k$ has zero boundary trace and is a classical, hence weak, solution. The $L^2$ [norms](../../../../../../norm.md) of $f_k$ are bounded independently of $k$. On the other hand,

$$
\partial_3u_k=\phi\bigl[\chi'\sin(kx_3)+k\chi\cos(kx_3)\bigr].
$$

The squared [norm](../../../../../../norm.md) of $\chi\cos(kx_3)$ tends to $\frac12\|\chi\|_2^2$, by the oscillatory integral identity for $\cos^2$. The other term has bounded [norm](../../../../../../norm.md), so $\|u_k\|_{H^1}$ grows at least proportionally to $k$. Therefore

$$
\boxed{\text{no uniform }C\text{ can satisfy the claimed estimate for this fixed }g=0.}
$$

This [failure of a coercive Dirichlet estimate under degeneracy](../../../../../../failure-of-a-coercive-dirichlet-estimate-under-degeneracy.md) loses control in the third direction; it does not rely on varying $g$ with the sequence.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
