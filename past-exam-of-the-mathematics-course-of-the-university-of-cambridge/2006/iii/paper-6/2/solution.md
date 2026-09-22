<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A point $x$ of a [convex set](../../../../../convex-set.md) $K$ is an [extreme point](../../../../../extreme-point.md) if $x=(1-t)a+tb$ with $a,b\in K$ and $0<t<1$ forces $a=b=x$. It is enough to test midpoints: a nontrivial interior point of a segment is the midpoint of a smaller nontrivial segment.

Here is a proof of the [Krein-Milman theorem](../../../../../krein-milman-theorem.md). The empty-set case is immediate, so take $K\ne\varnothing$. A [face of a convex set](../../../../../face-of-a-convex-set.md) is a convex subset $F\subseteq K$ such that an interior convex combination lying in $F$ has both endpoints in $F$. Consider nonempty compact faces. They include $K$. Every inclusion chain has nonempty intersection, because its closed subsets of the compact set $K$ have the [finite intersection property](../../../../../finite-intersection-property.md). The intersection remains a compact face. The [Zorn lemma](../../../../../zorn-s-lemma.md), ordered by reverse inclusion, therefore supplies a minimal nonempty compact face $F$.

If $F$ contains two distinct points, the Hausdorff locally convex hypotheses and the allowed separation theorem supply a continuous real [linear functional](../../../../../linear-functional.md) $\ell$ taking different values there. Its maximizer set in $F$ is nonempty and compact. It is convex, and if a convex combination attains the maximum, both endpoint values attain it too; hence it is a face of $F$. A face of a face is a face of $K$, by applying the defining endpoint property twice. This maximizer face is proper because $\ell$ is nonconstant, contradicting minimality. Thus $F$ is a singleton, whose point is extreme in $K$. The same [minimal compact face argument](../../../../../minimal-compact-face-argument.md) inside any nonempty compact face shows that each such face contains an [extreme point](../../../../../extreme-point.md) of $K$.

Let $H=\overline{\operatorname{conv}}(\operatorname{ext}K)$. Since $K$ is compact, hence closed in the [Hausdorff space](../../../../../hausdorff-space.md), and convex, $H\subseteq K$. It is nonempty, closed and convex. If $p\in K\setminus H$, the allowed strict separation theorem supplies a continuous [linear functional](../../../../../linear-functional.md) with

$$
\ell(p)>\sup_{h\in H}\ell(h).
$$

The maximizer face of $\ell$ on $K$ contains an [extreme point](../../../../../extreme-point.md) $e$ by the preceding argument. Then $e\in H$ but $\ell(e)=\max_K\ell\ge\ell(p)>\sup_H\ell$, a contradiction. Therefore

$$
\boxed{K=\overline{\operatorname{conv}}(\operatorname{ext}K).}
$$

All closures refer to the given locally convex topology, and [compactness](../../../../../compact-space.md) is what justified both maxima and chain intersections.

For the real [l-infinity sequence space](../../../../../l-infinity-sequence-space.md), if $|x_j|<1$ for any coordinate, choose $0<\epsilon\le1-|x_j|$. The two distinct sequences $x\pm\epsilon e_j$ belong to the closed unit ball and have midpoint $x$, so $x$ is not extreme. Conversely, if every $x_j$ is one or minus one, writing $x=(1-t)a+tb$ for unit-ball sequences forces $a_j=b_j=x_j$ at every coordinate, because an endpoint of $[-1,1]$ cannot be a nontrivial convex average of its points. Thus

$$
\boxed{\operatorname{ext}B_{\ell^\infty}=\{-1,1\}^{\mathbb N}.}
$$

For the [space of sequences converging to zero](../../../../../space-of-sequences-converging-to-zero.md), every unit-ball sequence has some coordinate with $|x_j|<1$, since its coordinates tend to zero. The same opposite single-coordinate perturbations still belong to $c_0$, giving

$$
\boxed{\operatorname{ext}B_{c_0}=\varnothing.}
$$

These are [extreme points of real sequence-space unit balls](../../../../../extreme-points-of-real-sequence-space-unit-balls.md). There is no conflict with Krein-Milman: the norm-closed unit ball of $c_0$ is not [compact](../../../../../compact-space.md) in the [norm topology](../../../../../norm-topology.md), as the coordinate vectors have mutual distance one.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
