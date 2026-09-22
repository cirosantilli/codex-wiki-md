<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A smooth [vector field](../../../../../../vector-field.md) on a [smooth manifold](../../../../../../smooth-manifold.md) $M$ is a smooth section of its [tangent bundle](../../../../../../tangent-bundle.md): it assigns $v(p)\in T_pM$ smoothly to each point. On a [Lie group](../../../../../../lie-group.md), it is a [left-invariant vector field](../../../../../../left-invariant-vector-field.md) when

$$
v(gp)=(dL_g)_p v(p),\qquad L_g(p)=gp.
$$

For $X\in T_eG$, define $v_X(g)=(dL_g)_eX$. Smoothness of multiplication makes this a smooth [vector field](../../../../../../vector-field.md), and $L_gL_p=L_{gp}$ plus the chain rule proves left invariance. Every [left-invariant vector field](../../../../../../left-invariant-vector-field.md) arises this way from its value at the identity.

For a matrix [Lie group](../../../../../../lie-group.md), $v_X(g)=gX$, because the derivative at zero of $g\gamma(t)$ is $gX$. The printed group name in this subpart must be read as $\mathrm{SL}_2$, rather than the additive vector space $\mathfrak{sl}_2$: it is the matrix-group calculation consistent with the preceding subparts. At the specified matrix,

$$
\boxed{v_X\!\left(\begin{pmatrix}0&1\\-1&0\end{pmatrix}\right)
=\begin{pmatrix}0&1\\-1&0\end{pmatrix}\begin{pmatrix}0&1\\0&0\end{pmatrix}
=\begin{pmatrix}0&0\\0&-1\end{pmatrix}.}
$$

A tangent vector at a nonidentity group element need not itself be trace-free; here $g^{-1}v_X(g)=X$ is trace-free, as required. If one instead interpreted the printed $\mathfrak{sl}_2$ as its additive [Lie group](../../../../../../lie-group.md), the field would be the constant field $X$, a different problem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
