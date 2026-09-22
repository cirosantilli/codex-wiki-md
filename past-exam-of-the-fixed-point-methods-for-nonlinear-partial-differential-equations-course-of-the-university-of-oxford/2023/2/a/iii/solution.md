<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We first prove the compact-domain [Schauder fixed-point theorem](../../../../../schauder-fixed-point-theorem.md). Let $K$ be a nonempty compact [convex set](../../../../../convex-set-split.md) in a [Banach space](../../../../../banach-space-split.md) $X$, and let $T:K\to K$ be a [continuous map](../../../../../continuous-map.md). The [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) states that every [continuous map](../../../../../continuous-map.md) of a finite-dimensional [closed unit ball](../../../../../closed-unit-ball.md) into itself has a [fixed point](../../../../../fixed-point.md). By the [homeomorphism](../../../../../homeomorphism.md) proved in part (a)(ii), it applies equally to any nonempty finite-dimensional compact [convex set](../../../../../convex-set-split.md), including a singleton.

For $\varepsilon>0$, use the supplied [Schauder approximation lemma](../../../../../schauder-approximation-lemma.md) to obtain a finite-dimensional [linear subspace](../../../../../vector-subspace.md) $L_\varepsilon$ and a [continuous map](../../../../../continuous-map.md) $T_\varepsilon:K\to K\cap L_\varepsilon$ with $\|Tx-T_\varepsilon x\|\leq\varepsilon$. The set $K_\varepsilon=K\cap L_\varepsilon$ is nonempty because it contains $T_\varepsilon(K)$. It is a compact [convex set](../../../../../convex-set-split.md), since a finite-dimensional [linear subspace](../../../../../vector-subspace.md) is closed. Restricting $T_\varepsilon$ to $K_\varepsilon$ and applying the [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) gives $x_\varepsilon=T_\varepsilon x_\varepsilon$, and thus

$$
\|Tx_\varepsilon-x_\varepsilon\|\leq\varepsilon.
$$

Take $\varepsilon_j=1/j$. The [compactness](../../../../../compact-space.md) of $K$ yields a [convergent subsequence](../../../../../convergent-subsequence.md) $x_{\varepsilon_{j_m}}\to x_*\in K$. The [continuity](../../../../../continuous-function.md) of $T$ and the preceding estimate give

$$
\boxed{Tx_*=x_*.}
$$

For completeness, this also proves the version on a nonempty closed bounded [convex set](../../../../../convex-set-split.md) $C$ when $T(C)$ is [relatively compact](../../../../../relatively-compact-subset.md). Let $K=\overline{\operatorname{conv}}T(C)\subset C$. The [closed convex hull of a compact set](../../../../../closed-convex-hull-of-a-compact-set.md) in a [Banach space](../../../../../banach-space-split.md) is compact. To verify the fact needed here, cover $T(C)$ by finitely many [balls](../../../../../ball-mathematics.md) of radius $\delta$. Replacing every term of a [convex combination](../../../../../convex-combination.md) by a centre changes it by at most $\delta$ in [norm](../../../../../norm.md). The [convex hull](../../../../../convex-hull.md) of those finitely many centres is compact in a finite-dimensional [linear subspace](../../../../../vector-subspace.md), so it has a [finite net](../../../../../finite-net.md) of radius $\delta$. Thus $\operatorname{conv}T(C)$ is [totally bounded](../../../../../totally-bounded-space.md). Its closure is [complete](../../../../../completeness.md) and [totally bounded](../../../../../totally-bounded-space.md), hence compact. Now $T(K)\subset T(C)\subset K$, so the compact-domain result supplies a [fixed point](../../../../../fixed-point.md) in $C$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
