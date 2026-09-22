<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $S$ lies in the closed ball of radius $R$ centred at $c$. By [compactness](../../../../../../compact-space.md), the continuous function $q\mapsto|q-c|$ attains its maximum $r\leq R$ at some $p\in S$. The sphere of radius $r$ about $c$ is a [supporting sphere](../../../../../../supporting-sphere.md) tangent to $S$ at $p$.

Put $N=(p-c)/r$. For any unit vector $v\in T_pS$, choose a surface curve $\alpha$ with $\alpha(0)=p$ and $\alpha'(0)=v$. Since $|\alpha(t)-c|^2$ has a local maximum at zero,

$$
0\geq
\left.\frac{d^2}{dt^2}|\alpha(t)-c|^2\right|_{t=0}
=2+2r\langle\alpha''(0),N\rangle.
$$

The scalar $\langle\alpha''(0),N\rangle$ is the [normal curvature](../../../../../../normal-curvature.md) in direction $v$, so every normal curvature is at most $-1/r$ with this choice of [unit normal](../../../../../../unit-normal.md). Applying this to [principal directions](../../../../../../principal-direction.md) shows that both [principal curvatures](../../../../../../principal-curvature.md) satisfy $k_i\leq-1/r$. Therefore

$$
K(p)=k_1k_2\geq\frac1{r^2}\geq\frac1{R^2}>0.
$$

This proves both assertions, including the existence of an [elliptic point](../../../../../../elliptic-point.md) on every compact regular surface.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
