<h1 id="8g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The dual space is

$$
V^*=\operatorname{Hom}_F(V,F),
$$

the [vector space](../../../../../../vector-space-split.md) of linear functionals on $V$. If $e_1,\ldots,e_n$ is a [basis](../../../../../../basis.md) of a finite-dimensional $V$, define $e_i^*(e_j)=\delta_{ij}$. Every $f\in V^*$ has the unique expansion

$$
f=\sum_{i=1}^nf(e_i)e_i^*,
$$

so the [dual basis](../../../../../../dual-basis.md) $e_1^*,\ldots,e_n^*$ proves

$$
\boxed{\dim V^*=\dim V=n}.
$$

For $U\leq V$, its [annihilator of a vector subspace](../../../../../../annihilator-of-a-vector-subspace.md) is

$$
U^\circ=\{f\in V^*:f(u)=0\text{ for every }u\in U\}.
$$

If $u_1,\ldots,u_k$ is a [basis](../../../../../../basis.md) of $U$ and is extended to a [basis](../../../../../../basis.md) $u_1,\ldots,u_n$ of $V$, then

$$
U^\circ=\operatorname{span}\{u_{k+1}^*,\ldots,u_n^*\}.
$$

Consequently

$$
\boxed{\dim U^\circ=\dim V-\dim U}.
$$

If $U\ne V$, this dimension is positive, giving a nonzero functional that vanishes on $U$.

For a [linear map](../../../../../../linear-map.md) $\alpha:V\to W$, the [dual map](../../../../../../transpose-of-a-linear-map.md) is

$$
\alpha^*:W^*\to V^*,
\qquad
\alpha^*(g)=g\circ\alpha.
$$

Now

$$
g\in\ker\alpha^*
\Longleftrightarrow g(\alpha v)=0\text{ for every }v
\Longleftrightarrow g\in(\operatorname{im}\alpha)^\circ,
$$

so

$$
\boxed{\ker\alpha^*=(\operatorname{im}\alpha)^\circ}.
$$

Every $g\circ\alpha$ vanishes on $\ker\alpha$, hence

$$
\operatorname{im}\alpha^*\subseteq(\ker\alpha)^\circ.
$$

The two spaces have the same dimension, since

$$
\begin{aligned}
\dim\operatorname{im}\alpha^*
&=\dim W-\dim(\operatorname{im}\alpha)^\circ
=\dim\operatorname{im}\alpha,\\
\dim(\ker\alpha)^\circ
&=\dim V-\dim\ker\alpha
=\dim\operatorname{im}\alpha.
\end{aligned}
$$

Thus

$$
\boxed{\operatorname{im}\alpha^*=(\ker\alpha)^\circ}.
$$

Let $Q:V\to V/U$ be the quotient map. Since $Q$ is onto, $Q^*$ is injective, and the preceding identity gives

$$
\operatorname{im}Q^*=(\ker Q)^\circ=U^\circ.
$$

Therefore

$$
\boxed{(V/U)^*\cong U^\circ}.
$$

For the inclusion $J:U\hookrightarrow V$, the map $J^*:V^*\to U^*$ is restriction to $U$. It is onto and has kernel

$$
\ker J^*=(\operatorname{im}J)^\circ=U^\circ.
$$

The first isomorphism theorem now gives the other [duals of a subspace and its quotient](../../../../../../duals-of-a-subspace-and-its-quotient.md):

$$
\boxed{U^*\cong V^*/U^\circ}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8G](../../8g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
