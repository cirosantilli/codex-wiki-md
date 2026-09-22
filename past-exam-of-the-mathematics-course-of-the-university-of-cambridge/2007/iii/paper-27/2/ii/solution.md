<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) asserts that $E(K)/mE(K)$ is finite for an [elliptic curve](../../../../../../elliptic-curve.md) over a [number field](../../../../../../number-field.md) $K$ and an [integer](../../../../../../integer.md) $m\ge2$. The role of (i) is to make division by $m$ possible in the local [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) whenever the [residue characteristic](../../../../../../residue-characteristic.md) does not divide $m$.

Let $v$ be a finite place with [good reduction of an elliptic curve](../../../../../../good-reduction-of-an-elliptic-curve.md) and $v\nmid m$. The [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md) is parametrized by $t=-x/y$ in the [maximal ideal](../../../../../../maximal-ideal.md) of the local [valuation ring](../../../../../../valuation-ring.md). Multiplication by $m$ is represented by an integral [formal power series](../../../../../../formal-power-series.md)

$$
[m](T)=mT+\text{terms of degree at least }2.
$$

Its linear coefficient is a local [unit](../../../../../../unit-in-a-ring.md). Part (i) supplies an integral compositional inverse. Both series converge on the [maximal ideal](../../../../../../maximal-ideal.md), so multiplication by $m$ is a [bijection](../../../../../../bijection.md) on the reduction kernel, over the [local field](../../../../../../local-field.md) and over every finite [unramified extension](../../../../../../unramified-extension.md).

This implies [unramified division torsors at good primes](../../../../../../unramified-division-torsors-at-good-primes.md). For $P\in E(K)$, first divide its reduction by $m$ over the algebraic closure of the [residue field](../../../../../../residue-field.md). Multiplication by $m$ on the reduced curve is [surjective](../../../../../../surjective-function.md) and separable, so the chosen division point is defined over some finite residue extension. Smooth lifting gives a point $Q_0$ over the corresponding unramified local extension with the required reduction. The difference $P-mQ_0$ lies in the reduction kernel; the inverse series supplies $Q_1$ with $mQ_1=P-mQ_0$. Thus $Q=Q_0+Q_1$ divides $P$ over an [unramified extension](../../../../../../unramified-extension.md). Applying the same reasoning to all reduced $m$-torsion points lifts all of $E[m]$, so every point of $[m]^{-1}P$ lies in the maximal [unramified extension](../../../../../../unramified-extension.md). This excludes ramification outside a fixed [finite set](../../../../../../finite-set.md) $S$ consisting of [primes](../../../../../../prime-number.md) of bad reduction and [primes](../../../../../../prime-number.md) over $m$.

For completeness, the remaining global finiteness step in the [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../../../../kummer-theoretic-proof-of-the-weak-mordell-weil-theorem.md) is as follows. Choose $Q\in E(\overline K)$ with $mQ=P$. The [cocycle](../../../../../../cocycle.md) $\sigma\mapsto\sigma Q-Q$ defines the [Kummer map of an elliptic curve](../../../../../../kummer-map-of-an-elliptic-curve.md)

$$
E(K)/mE(K)\hookrightarrow H^1(K,E[m]).
$$

Changing $Q$ by an $m$-torsion point changes the [cocycle](../../../../../../cocycle.md) by a [coboundary](../../../../../../coboundary.md). A zero class makes $Q$ rational after that change, so the map is injective.

Let $L=K(E[m])$, fixed independently of $P$. Since the torsion is rational over $L$, the [cocycle](../../../../../../cocycle.md) restricted to its [Galois group](../../../../../../galois-group.md) is a homomorphism into $E[m]$. Consequently $L(Q)/L$ is Galois of degree at most $m^2$, contains the entire division fibre, and is unramified outside $S$. Hence $[L(Q):K]\le m^2[L:K]$. There are only finitely many extensions of bounded degree unramified outside a fixed [finite set](../../../../../../finite-set.md): local extensions of bounded degree have bounded [field discriminant](../../../../../../field-discriminant.md) exponents, and the [Hermite–Minkowski theorem](../../../../../../hermite-minkowski-theorem.md) then applies to the bounded global [field discriminants](../../../../../../field-discriminant.md). Their finite Galois compositum $M$ contains every such division fibre; each $L(Q)$ is stable over $K$ because it contains $E[m]$ and the whole fibre above the rational point $P$. All the Kummer classes consequently factor through the fixed [finite group](../../../../../../finite-group.md) $\operatorname{Gal}(M/K)$ with values in the fixed [finite group](../../../../../../finite-group.md) $E[m]$. There are only finitely many such [cocycles](../../../../../../cocycle.md), proving

$$
\boxed{E(K)/mE(K)\text{ is finite}.}
$$

Thus (i) provides the local division step that bounds ramification; the global arithmetic finiteness completes the argument.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
