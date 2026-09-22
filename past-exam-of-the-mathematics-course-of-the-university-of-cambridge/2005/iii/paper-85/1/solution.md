<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take rings and modules to be unital. Let $J_\ell$ denote the intersection of the [maximal left ideals](../../../../../maximal-left-ideal.md). For each nonzero vector $v$ of a [simple module](../../../../../irreducible-module.md) $M$ on the left, the map $R\to M$, $r\mapsto rv$, is onto and its kernel is a [maximal left ideal](../../../../../maximal-left-ideal.md). Consequently $J_\ell$ annihilates every [simple module](../../../../../irreducible-module.md) on the left. Conversely, annihilating $R/L$ forces an element to belong to the [maximal left ideal](../../../../../maximal-left-ideal.md) $L$. Thus

$$
J_\ell=\bigcap_{M\text{ simple left}}\operatorname{Ann}_R(M),
$$

which shows that $J_\ell$ is a two-sided [ideal](../../../../../ideal.md).

For $j\in J_\ell$ and $r\in R$, the [left ideal](../../../../../left-ideal.md) $R(1-rj)$ cannot be proper: a containing [maximal left ideal](../../../../../maximal-left-ideal.md) would also contain $rj$ and hence $1$. Therefore $u(1-rj)=1$ for some $u\in R$. Here $u=1+urj$ also differs from $1$ by an element of $J_\ell$, so it too has a left inverse $v$. Multiplying the first equality by $v$ gives $1-rj=v$; hence $(1-rj)u=1$. We have proved that $1-rj$ is a [unit](../../../../../unit-in-a-ring.md), not just left invertible.

The identity

$$
(1-ba)^{-1}=1+b(1-ab)^{-1}a
$$

is verified by multiplying on either side, using $(1-ab)^{-1}(1-ab)=(1-ab)(1-ab)^{-1}=1$. It implies that $1-jr$ is a [unit](../../../../../unit-in-a-ring.md) as well. If $j$ were outside a [maximal right ideal](../../../../../maximal-right-ideal.md) $I$, then $I+jR=R$, so $1-jr\in I$ for some $r$. A proper [right ideal](../../../../../right-ideal.md) cannot contain a [unit](../../../../../unit-in-a-ring.md), giving a contradiction. Thus $J_\ell$ belongs to every [maximal right ideal](../../../../../maximal-right-ideal.md). Applying the same argument to the [opposite ring](../../../../../opposite-ring.md) proves the reverse inclusion. This proves the [Jacobson radical is independent of handedness](../../../../../jacobson-radical-is-independent-of-handedness.md):

$$
\boxed{J(R)=\bigcap_{L\text{ maximal left}}L=\bigcap_{I\text{ maximal right}}I.}
$$

For the zero ring the intersections are interpreted as the whole ring, so the equality remains valid.

If a two-sided [ideal](../../../../../ideal.md) $N$ satisfies $N^m=0$, then for $x\in N$ and $r\in R$, $(rx)^m=0$. The finite [geometric series](../../../../../geometric-series.md) $\sum_{i=0}^{m-1}(rx)^i$ inverts $1-rx$. The [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md), also proved above by the maximal-ideal argument, gives **$N\subseteq J(R)$**. This assertion concerns a [nilpotent ideal](../../../../../nilpotent-ideal.md); arbitrary [nilpotent elements](../../../../../nilpotent.md) of a noncommutative ring need not lie in its [Jacobson radical](../../../../../jacobson-radical.md).

For the [formal power series ring](../../../../../formal-power-series.md) over the [p-adic integers](../../../../../p-adic-integer.md), a series $f=\sum_{i\ge0}a_it^i$ is a [unit](../../../../../unit-in-a-ring.md) exactly when $a_0$ is a [unit](../../../../../unit-in-a-ring.md) of $\mathbb Z_p$. Necessity follows by comparing constant coefficients. If $a_0$ is invertible, construct the inverse recursively by $b_0=a_0^{-1}$ and $b_m=-a_0^{-1}\sum_{i=1}^m a_ib_{m-i}$. Therefore the nonunits are exactly the series whose constant coefficient lies in $p\mathbb Z_p$. They form the unique maximal [ideal](../../../../../ideal.md) $(p,t)$, and the quotient is $\mathbb F_p$. Hence

$$
\boxed{J(\mathbb Z_p[[t]])=(p,t).}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 85](../../paper-85-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
