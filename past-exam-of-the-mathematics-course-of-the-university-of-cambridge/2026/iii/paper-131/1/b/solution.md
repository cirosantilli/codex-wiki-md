<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose

$$
0<\delta<\min\{d_g(p,q),r_p\},
$$

where $r_p$ is a normal radius at $p$. Take piecewise smooth curves $c_j$ from $p$ to $q$ such that $L_g(c_j)\to d_g(p,q)$. Each $c_j$ first leaves the normal ball $B_g(p,\delta)$ at a point $p_j$. The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) gives $d_g(p,p_j)=\delta$. The geodesic sphere

$$
S_g(p,\delta)=\exp_p\{v\in T_pM:|v|_g=\delta\}
$$

is [compact](../../../../../../compact-space.md), because the tangent-space sphere is compact and $\exp_p$ is defined on it. After taking a [convergent subsequence](../../../../../../convergent-subsequence.md), let $p_j\to p_0$.

The part of $c_j$ after $p_j$ has length at least $d_g(p_j,q)$, so continuity of the [Riemannian distance](../../../../../../riemannian-distance.md) gives

$$
\delta+d_g(p_0,q)
\leq\lim_{j\to\infty}L_g(c_j)
=d_g(p,q).
$$

The [triangle inequality](../../../../../../triangle-inequality.md) gives the reverse inequality. Therefore

$$
\boxed{d_g(p,p_0)=\delta,
\qquad
d_g(p,p_0)+d_g(p_0,q)=d_g(p,q).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
