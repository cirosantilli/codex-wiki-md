<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\kappa=\omega_1$ and choose a [club sequence](../../../../../../club-sequence.md) on $\omega_2$, each $C_\delta$ of [order type](../../../../../../order-type.md) at most $\omega_1$. For a successor $\delta$ use its predecessor as a singleton; at a limit use a cofinal sequence of minimal length. Form the [minimal-walk tree](../../../../../../minimal-walk-tree.md)

$$
T_\alpha=\{\rho_\beta\upharpoonright\alpha:\alpha\leq\beta<\omega_2\},
\qquad T=\bigcup_{\alpha<\omega_2}T_\alpha,
$$

ordered by proper extension. Its height is $\omega_2$.

For $\xi<\delta$, the initial segment $C_\delta\cap\xi$ has [order type](../../../../../../order-type.md) strictly below $\omega_1$, and is countable. The strict inequality follows because a point of $C_\delta$ at or above $\xi$ occurs later in its enumeration. Hence every entry of every trace is countable. Under the [Continuum hypothesis](../../../../../../continuum-hypothesis.md), for $|\alpha|\leq\aleph_1$,

$$
|[\alpha]^{\leq\omega}|\leq\aleph_1^{\aleph_0}
=(2^{\aleph_0})^{\aleph_0}=\aleph_1.
$$

There are at most $\aleph_1$ finite sequences of such sets. The [trace coherence lemma for minimal walks](../../../../../../trace-coherence-lemma-for-minimal-walks.md) says that, for $\beta>\alpha$, the value $\rho_\beta(\alpha)$ determines $\rho_\beta\upharpoonright\alpha$. The case $\beta=\alpha$ adds at most one node. Thus $|T_\alpha|\leq\aleph_1$ for every level.

Suppose that $T$ had a [cofinal branch](../../../../../../cofinal-branch.md), and take the union of its functions, $f$, with domain $\omega_2$. Every $\rho_\beta$ is injective by the proper-initial-segment argument, so $f$ is injective too. On the [stationary set](../../../../../../stationary-set.md)

$$
S=\{\alpha<\omega_2:\operatorname{cf}(\alpha)=\omega_1\},
$$

this set is stationary because the supremum of a strictly increasing $\omega_1$-sequence from any [club set](../../../../../../club-set.md) has cofinality $\omega_1$ and lies in that club. The union of the finitely many countable entries of $f(\alpha)$ is bounded below $\alpha$. Assign a strict upper bound below $\alpha$ to obtain a [regressive function](../../../../../../regressive-function.md). By [Fodor lemma](../../../../../../fodor-lemma.md), there is a stationary $S'\subseteq S$ and a single $\eta<\omega_2$ such that every entry of $f(\alpha)$ lies inside $\eta$ for $\alpha\in S'$. There are at most $\aleph_1$ such finite sequences by the same [cardinal arithmetic](../../../../../../cardinal-arithmetic.md), but $|S'|=\aleph_2$, contradicting injectivity.

Therefore **$T$ is an [aleph-two Aronszajn tree](../../../../../../aleph-two-aronszajn-tree.md)**:

$$
\boxed{\operatorname{ht}(T)=\omega_2,\quad |T_\alpha|<\aleph_2,
\quad T\text{ has no cofinal branch}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
