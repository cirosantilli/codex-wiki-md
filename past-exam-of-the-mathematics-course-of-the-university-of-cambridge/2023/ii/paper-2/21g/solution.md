<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

Choose a path $\gamma$ in $X$ from $x_0$ to $x_1$. For every $\widehat x\in p^{-1}(x_0)$, the [path lifting theorem](../../../../../path-lifting-theorem.md) gives a unique lift of $\gamma$ starting at $\widehat x$. Send $\widehat x$ to the endpoint of this lift. Lifting the reversed path gives the inverse map, so this is the [fibre bijection by path lifting](../../../../../fibre-bijection-by-path-lifting.md)

$$
p^{-1}(x_0)\cong p^{-1}(x_1).
$$

In particular, all fibres have the same cardinality.

A connected covering is a [normal covering map](../../../../../normal-covering-map.md) when its deck transformations act transitively on a fibre. Equivalently, for a choice of $\widehat x_0$ above $x_0$,

$$
p_*\pi_1(\widehat X,\widehat x_0)
\triangleleft
\pi_1(X,x_0).
$$

The relevant [lifting criterion for a covering space](../../../../../lifting-criterion-for-a-covering-space.md) says that a based map $f:(Y,y_0)\to(X,x_0)$ lifts through $p$ exactly when

$$
f_*\pi_1(Y,y_0)
\subseteq
p_*\pi_1(\widehat X,\widehat x_0).
$$

For a universal covering, $\widehat X$ is simply connected, so the displayed covering subgroup is trivial and hence normal. Thus a [universal covering map is normal](../../../../../universal-covering-map-is-normal.md).

Now consider connected finite covers of the closed orientable surface $\Sigma_g$. By the [classification of connected covering spaces](../../../../../classification-of-connected-covering-spaces.md), degree-$n$ connected covers correspond to index-$n$ subgroups of the [fundamental group of a closed orientable surface](../../../../../fundamental-group-of-a-closed-orientable-surface.md), and normal covers correspond to normal subgroups.

The cases in which normality is forced are:

- $n=1$, because the subgroup is the whole fundamental group.
- $n=2$, because every [index-two subgroup is normal](../../../../../index-two-subgroup-is-normal.md).
- $g=1$, because $\pi_1(\Sigma_1)\cong\mathbb Z^2$ is abelian, so all its subgroups are normal.
- For $g=0$, the sphere is simply connected, so a connected cover necessarily has $n=1$.

It remains to show that these are the only forced cases. Let $g\geq2$ and $n\geq3$. Write

$$
\pi_1(\Sigma_g)=
\left\langle a_1,b_1,\ldots,a_g,b_g
\mathrel{\Big|}
\prod_{i=1}^g[a_i,b_i]=1
\right\rangle.
$$

In the [symmetric group](../../../../../symmetric-group.md) $S_n$, put

$$
\sigma=(1\,2\,\cdots\,n),
\qquad
\tau=(1\,2).
$$

Define a homomorphism by

$$
a_1\mapsto\sigma,\quad b_1\mapsto\tau,\quad
a_2\mapsto\tau,\quad b_2\mapsto\sigma,
$$

and send all remaining generators to the identity. The relation is respected because

$$
[\sigma,\tau][\tau,\sigma]=1.
$$

The cycle $\sigma$ and transposition $\tau$ generate $S_n$, so the homomorphism is surjective.

Let

$$
H=\phi^{-1}\bigl(\operatorname{Stab}_{S_n}(1)\bigr).
$$

The natural action of $S_n$ is transitive, so $H$ has index $n$. Its image is the point stabilizer $S_{n-1}$, which is not normal in $S_n$ for $n\geq3$; hence $H$ is not normal. The connected covering corresponding to $H$ is therefore an explicit degree-$n$ nonnormal cover. This is the [nonnormal finite cover of a higher-genus orientable surface](../../../../../nonnormal-finite-cover-of-a-higher-genus-orientable-surface.md).

Consequently, among connected covers that exist, normality is forced exactly when

$$
\boxed{n\leq2\quad\text{or}\quad g\leq1,}
$$

with the qualification that $g=0$ permits only $n=1$, as summarized by the [forced normality of finite connected covers of orientable surfaces](../../../../../forced-normality-of-finite-connected-covers-of-orientable-surfaces.md).

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
