<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [extreme point](../../../../../extreme-point.md) $x$ of a [convex set](../../../../../convex-set.md) $K$ is one for which $x=(1-t)y+tz$, $y,z\in K$ and $0<t<1$ imply $y=z=x$. It is enough to test midpoint decompositions: a nontrivial interior point of a segment is itself the midpoint of a shorter nontrivial segment contained in that segment.

We prove the [Krein-Milman theorem](../../../../../krein-milman-theorem.md). Assume first that $K$ is nonempty. A [face of a convex set](../../../../../face-of-a-convex-set.md) $K$ means a convex subset $F$ with the property that whenever an interior point of a segment in $K$ belongs to $F$, both endpoints belong to $F$. The family of nonempty compact faces of $K$, including $K$ itself, has a minimal member by the [Zorn lemma](../../../../../zorn-s-lemma.md): every inclusion-decreasing chain has a nonempty intersection by [compactness](../../../../../compact-space.md) and the [finite intersection property](../../../../../finite-intersection-property.md), and that intersection is again a compact face.

Let $M$ be such a minimal face. If it contains two distinct points, the continuous dual of a Hausdorff [locally convex space](../../../../../locally-convex-space.md) separates them, by the permitted [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). Choose a continuous real [linear functional](../../../../../linear-functional.md) $\ell$ that is not constant on $M$. It attains a maximum on the compact set $M$, and

$$
M_1=\{z\in M:\ell(z)=\max_M\ell\}
$$

is a nonempty proper compact face of $M$, and hence a face of $K$. Indeed, equality at the maximum in a convex combination forces both endpoint values to be maximal. This contradicts minimality. Thus $M$ is a singleton, and its point is extreme in $K$. The same argument applied within any nonempty compact face proves that every such face contains an [extreme point](../../../../../extreme-point.md) of $K$.

Let $C=\overline{\operatorname{conv}}(\operatorname{ext}K)$. It is contained in $K$, since the latter is closed and convex, and [extreme points](../../../../../extreme-point.md) exist when $K$ is nonempty. If $x_0\in K\setminus C$, the permitted separation theorem provides a continuous real [linear functional](../../../../../linear-functional.md) $\ell$ with $\ell(x_0)>\sup_C\ell$. Let $F$ be its maximizer face on $K$. This nonempty compact face contains an [extreme point](../../../../../extreme-point.md) $v$ of $K$, but

$$
\ell(v)=\max_K\ell\geq\ell(x_0)>\sup_C\ell,
$$

contradicting $v\in\operatorname{ext}K\subseteq C$. Therefore

$$
\boxed{K=\overline{\operatorname{conv}}(\operatorname{ext}K)}.
$$

For empty $K$, the equality holds with the usual empty convex-hull convention. This proves both the extreme-point existence step and the closed-convex-hull step; no [compactness](../../../../../compact-space.md) of the set of [extreme points](../../../../../extreme-point.md) itself is assumed.

The real [absolutely summable sequence space](../../../../../absolutely-summable-sequence-space.md) is $\ell^1=\{x=(x_j):\sum_j|x_j|<\infty\}$ with [norm](../../../../../norm.md) $\|x\|_1=\sum_j|x_j|$. The real [l-infinity sequence space](../../../../../l-infinity-sequence-space.md) is $\ell^\infty=\{x=(x_j):\sup_j|x_j|<\infty\}$ with [norm](../../../../../norm.md) $\|x\|_\infty=\sup_j|x_j|$. Their [completeness](../../../../../completeness.md) is allowed as given; their [extreme points](../../../../../extreme-point.md) still require proof.

For $\ell^1$, an interior point of the [unit ball](../../../../../unit-ball.md) is not extreme because small opposite perturbations in one coordinate stay in the ball. At a boundary point with two nonzero coordinates $i,j$, choose $0<\varepsilon<\min(|x_i|,|x_j|)$ and put

$$
z=\varepsilon\operatorname{sgn}(x_i)e_i-\varepsilon\operatorname{sgn}(x_j)e_j.
$$

The two distinct vectors $x+z,x-z$ both have [norm](../../../../../norm.md) one and average to $x$, so $x$ is not extreme. A remaining boundary point must be $\pm e_j$. If $e_j=(y+z)/2$ with $\|y\|_1,\|z\|_1\leq1$, the $j$th coordinate forces $y_j=z_j=1$, exhausting both [norm](../../../../../norm.md) budgets and forcing all other coordinates to zero. The negative case is identical. Thus

$$
\boxed{\operatorname{ext}B_{\ell^1}=\{e_j,-e_j:j\geq1\}}.
$$

For $\ell^\infty$, if $|x_j|<1$ in even one coordinate, small opposite changes to that coordinate give a nontrivial midpoint decomposition within the ball. If every $x_j=\pm1$, a midpoint decomposition forces both summands to have that same value in every coordinate, so they equal $x$. Hence

$$
\boxed{\operatorname{ext}B_{\ell^\infty}=\{-1,1\}^{\mathbb N}}.
$$

These are precisely the [extreme points of real sequence-space unit balls](../../../../../extreme-points-of-real-sequence-space-unit-balls.md) for the two spaces under consideration.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
