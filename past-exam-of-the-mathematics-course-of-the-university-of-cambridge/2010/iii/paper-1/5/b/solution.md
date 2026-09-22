<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define

$$
\mathfrak h=\{X\in\mathfrak g:\exp(tX)\in H\text{ for every }t\in\mathbb R\}.
$$

It contains zero, and $X\in\mathfrak h$ implies $aX\in\mathfrak h$ for every real scalar $a$, by replacing $t$ with $at$.

For $X,Y\in\mathfrak h$, we prove closure under addition using the [Lie product formula in a Lie group](../../../../../../lie-product-formula-in-a-lie-group.md). In the [local exponential chart](../../../../../../local-exponential-chart.md), let $Z(s)=\log(\exp(sX)\exp(sY))$. Smooth multiplication has differential $(U,V)\mapsto U+V$ at the identity, so [Taylor's theorem](../../../../../../taylor-theorem.md) gives

$$
Z(s)=s(X+Y)+O(s^2).
$$

For each fixed real $t$ and all sufficiently large positive [integers](../../../../../../integer.md) $m$,

$$
\left[\exp(tX/m)\exp(tY/m)\right]^m=\exp\bigl(mZ(t/m)\bigr)
\longrightarrow\exp(t(X+Y)).
$$

Every term belongs to $H$, and $H$ is closed, proving $X+Y\in\mathfrak h$. Thus $\mathfrak h$ is a real [vector subspace](../../../../../../vector-subspace.md). It is also closed: if $X_j\to X$ with $X_j\in\mathfrak h$, continuity of the [Exponential map of a Lie group](../../../../../../exponential-map-of-a-lie-group.md) gives $\exp(tX)\in H$ for each $t$.

For the [Lie bracket](../../../../../../lie-bracket.md), use the [Adjoint representation of a Lie group](../../../../../../adjoint-representation-of-a-lie-group.md). Conjugating a [one-parameter subgroup](../../../../../../one-parameter-subgroup.md) gives

$$
\exp(sX)\exp(tY)\exp(-sX)=\exp\bigl(t\operatorname{Ad}_{\exp(sX)}Y\bigr)\in H.
$$

Consequently $\operatorname{Ad}_{\exp(sX)}Y\in\mathfrak h$. For $s\ne0$, linearity puts $\bigl(\operatorname{Ad}_{\exp(sX)}Y-Y\bigr)/s$ in $\mathfrak h$. Its limit as $s\to0$ is $\operatorname{ad}_XY=[X,Y]$. Closedness of $\mathfrak h$ therefore gives $[X,Y]\in\mathfrak h$, proving that the [Lie algebra of a closed subgroup](../../../../../../lie-algebra-of-a-closed-subgroup.md) is a [Lie subalgebra](../../../../../../lie-subalgebra.md) of $\mathfrak g$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
