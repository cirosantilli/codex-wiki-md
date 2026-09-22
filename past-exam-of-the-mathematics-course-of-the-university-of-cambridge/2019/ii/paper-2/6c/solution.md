<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

At a positive [spatially homogeneous equilibrium](../../../../../spatially-homogeneous-equilibrium.md),

$$
uv^2=a,
\qquad
v-uv^2=0,
$$

so

$$
(u_*,v_*)=\left(\frac1a,a\right).
$$

The [Jacobian matrix](../../../../../jacobian-matrix.md) of the reaction terms there is

$$
J=\begin{pmatrix}a^2&2\\-a^2&-1\end{pmatrix},
\qquad
\operatorname{tr}J=a^2-1,
\qquad
\det J=a^2.
$$

The [linear stability analysis](../../../../../linear-stability.md) of a two-dimensional system requires negative trace and positive determinant. Since $a>0$, the homogeneous equilibrium is stable exactly when

$$
\boxed{0<a<1}.
$$

For a spatial [Fourier mode](../../../../../fourier-mode.md) proportional to $\cos(kx)$, put $q=k^2$. The linearized matrix is

$$
J_q=J-q\begin{pmatrix}D&0\\0&1\end{pmatrix}.
$$

Its trace is still negative when $0<a<1$, while

$$
\det J_q=Dq^2+(D-a^2)q+a^2.
$$

A [Turing instability](../../../../../turing-instability.md) occurs for some $q>0$ exactly when this quadratic has a negative minimum. This requires

$$
D<a^2,
\qquad
(a^2-D)^2>4Da^2.
$$

Writing $d=\sqrt D$, the second inequality reduces to $d<a(\sqrt2-1)$. Hence, for continuously available wave numbers, the condition is

$$
\boxed{D<a^2(\sqrt2-1)^2=a^2(3-2\sqrt2).}
$$

On a bounded spatial domain, one additionally requires an allowed wave number $k$ for which $\det J_{k^2}<0$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
