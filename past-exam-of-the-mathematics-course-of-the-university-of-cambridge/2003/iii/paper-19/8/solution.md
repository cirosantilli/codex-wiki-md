<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For [Fodor's theorem](../../../../../fodor-lemma.md), let $\kappa$ be regular uncountable, $S\subseteq\kappa$ stationary, and $f:S\to\kappa$ regressive: $f(\alpha)<\alpha$ for every nonzero $\alpha\in S$. A [club set](../../../../../club-set.md) is unbounded in $\kappa$ and closed under limits below $\kappa$; a [stationary set](../../../../../stationary-set.md) meets every club. Removing $0$ preserves stationarity. We prove that some fibre of $f$ is stationary, not merely that one fibre is large.

We first check the club facts used in the argument. An [intersection](../../../../../set-intersection.md) of fewer than $\kappa$ club [subsets](../../../../../subset.md) of $\kappa$ is club. Closure is immediate. For unboundedness, given $\gamma$ and clubs $(C_i)_{i<\mu}$ with $\mu<\kappa$, choose an increasing [sequence](../../../../../sequence.md) $\gamma_n$ starting above $\gamma$, such that $\gamma_{n+1}$ is above a point of every $C_i$ beyond $\gamma_n$. Regularity bounds the [supremum](../../../../../supremum.md) of the fewer-than-$\kappa$ points at each step. Then $\delta=\sup_{n<\omega}\gamma_n<\kappa$, and the chosen points in each $C_i$ are cofinal in $\delta$; closure puts $\delta$ in their [intersection](../../../../../set-intersection.md).

For a [sequence](../../../../../sequence.md) $(C_\xi)_{\xi<\kappa}$ of clubs its [diagonal intersection](../../../../../diagonal-intersection.md)

$$
\Delta_{\xi<\kappa}C_\xi
=\{\delta<\kappa:\forall\xi<\delta\ (\delta\in C_\xi)\}
$$

is also club. To obtain a point above $\gamma$, recursively choose $\gamma_{n+1}>\gamma_n$ in $\bigcap_{\xi\le\gamma_n}C_\xi$, possible by the preceding result, and take the [supremum](../../../../../supremum.md) $\delta$ of the [sequence](../../../../../sequence.md). For each $\xi<\delta$, every sufficiently late $\gamma_n$ belongs to $C_\xi$, so $\delta\in C_\xi$. For closure, if diagonal-intersection points are cofinal in $\delta<\kappa$, then for each $\xi<\delta$ their sufficiently late points lie in $C_\xi$, and closure again puts $\delta$ there.

Suppose every fibre $S_\xi=\{\alpha\in S:f(\alpha)=\xi\}$ were nonstationary. Choose a club $C_\xi$ disjoint from each fibre. Stationarity supplies $\alpha\in S\cap\Delta_{\xi<\kappa}C_\xi$, with $\alpha>0$. Put $\xi=f(\alpha)<\alpha$. By diagonal membership $\alpha\in C_\xi$, but by its definition $\alpha\in S_\xi$, a contradiction. Thus

$$
\boxed{\exists\xi<\kappa\quad \{\alpha\in S:f(\alpha)=\xi\}\text{ is stationary}.}
$$

This is precisely the pressing-down assertion. Regularity and uncountability were used to keep the club-building suprema below $\kappa$.

For the [Cantor normal form](../../../../../cantor-normal-form.md) theorem, every nonzero [ordinal](../../../../../ordinal.md) has a unique expression

$$
\boxed{\alpha=\omega^{\beta_0}n_0+\cdots+\omega^{\beta_{m-1}}n_{m-1},
\qquad \beta_0>\cdots>\beta_{m-1},\quad 0<n_i<\omega.}
$$

All operations are [ordinal](../../../../../ordinal.md) operations, so the order of the terms matters. The [ordinal](../../../../../ordinal.md) zero has the empty expression. We give the greedy existence proof and then prove uniqueness.

The powers $\omega^\beta$ are strictly increasing and continuous at limit exponents, and satisfy $\omega^\beta\ge\beta$. Hence the [set](../../../../../set-split.md) of exponents with $\omega^\beta\le\alpha$ is nonempty and bounded, and its [supremum](../../../../../supremum.md) $\beta_0$ belongs to it by continuity (or is already its last successor member). Thus there is a largest such exponent and

$$
\omega^{\beta_0}\le\alpha<\omega^{\beta_0+1}
=\omega^{\beta_0}\cdot\omega.
$$

Since the last product is the [supremum](../../../../../supremum.md) of the finite multiples, there is a unique positive finite $n_0$ satisfying

$$
\omega^{\beta_0}n_0\le\alpha<\omega^{\beta_0}(n_0+1).
$$

The initial segment of $\alpha$ of length $\omega^{\beta_0}n_0$ leaves a tail of unique order type $\rho$, so

$$
\alpha=\omega^{\beta_0}n_0+\rho,\qquad \rho<\omega^{\beta_0}.
$$

The bound follows from strict increase of [ordinal addition](../../../../../ordinal-addition.md) in its right argument: a tail at least $\omega^{\beta_0}$ would contradict the preceding interval. This is the relevant instance of the [ordinal division algorithm](../../../../../ordinal-division-algorithm.md).

If $\rho>0$, apply the same construction to it. Its leading exponent must be below $\beta_0$. Continue with the remainder. An infinite continuation would produce an infinite strictly descending [sequence](../../../../../sequence.md) of [ordinals](../../../../../ordinal.md), impossible by [well-foundedness](../../../../../well-founded-relation.md). Thus the process terminates after finitely many steps and gives the required form.

To prove uniqueness, first observe that a finite decreasing-exponent suffix with leading exponent $\gamma$ is smaller than $\omega^{\gamma+1}$. This follows by induction on its number of terms: the later tail is below $\omega^\gamma$, so adding it to a finite multiple of $\omega^\gamma$ stays below the next finite multiple and hence below $\omega^\gamma\cdot\omega$. Consequently the tail after a term with exponent $\beta$ is below $\omega^\beta$.

Any proposed normal form therefore places $\alpha$ in exactly the interval

$$
\omega^{\beta_0}n_0\le\alpha<\omega^{\beta_0}(n_0+1)
<\omega^{\beta_0+1}.
$$

Its first exponent is recoverable as the largest exponent whose power does not exceed $\alpha$, and its first coefficient is recoverable as the largest finite multiple not exceeding $\alpha$. The right remainder is unique because [ordinal addition](../../../../../ordinal-addition.md) is strictly increasing in its right argument. Apply the same reasoning to the remainder, successively fixing every exponent and coefficient. This proves uniqueness without treating [ordinal addition](../../../../../ordinal-addition.md) as commutative or cancelling arbitrary left summands.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
