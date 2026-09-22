<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [measurable cardinal](../../../../../measurable-cardinal.md) is an uncountable [cardinal](../../../../../cardinal-number.md) $\kappa$ carrying a [kappa-complete](../../../../../kappa-complete-filter.md) [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $U$ on $\kappa$. An [elementary embedding](../../../../../elementary-embedding.md) $j:M\to N$ preserves all [first-order formulas](../../../../../first-order-formula.md) with parameters:

$$
M\models\varphi(a_1,\ldots,a_r)\quad\Longleftrightarrow\quad
N\models\varphi(j(a_1),\ldots,j(a_r)).
$$

For a measurable $\kappa$, the [Łoś theorem](../../../../../los-theorem.md) gives an elementary map from the universe into its [ultrapower](../../../../../ultrapower.md). Countable completeness makes that ultrapower well founded, so the [Mostowski collapse](../../../../../mostowski-collapse.md) gives a transitive target $M$ and an [ultrapower embedding](../../../../../ultrapower-embedding.md) $j:V\to M$. The least moved ordinal, its [critical point of an elementary embedding](../../../../../critical-point-of-an-elementary-embedding.md), is $\kappa$: every function into an ordinal below $\kappa$ is constant on a $U$-large set by [kappa-completeness](../../../../../kappa-complete-filter.md), whereas the identity function on $\kappa$ represents an ordinal above every constant ordinal below $\kappa$ and below the image of $\kappa$. Conversely a suitably available embedding with critical point $\kappa$ defines the measure $U=\{X\subseteq\kappa:\kappa\in j(X)\}$.

The identity $V\to V$ is elementary. **In ZFC there is no nonidentity elementary class embedding $j:V\to V$**, by the [Kunen inconsistency theorem](../../../../../kunen-inconsistency-theorem.md). Here the embedding is a class for which restrictions to sets and the critical sequence are available, as in the usual class-theoretic formulation. The [axiom of choice](../../../../../axiom-of-choice.md) is part of this conclusion; it is not a claimed contradiction for the choice-free Reinhardt-cardinal hypothesis.

Here is the stationary-set proof. A nonidentity $j$ has a least moved ordinal $\kappa$; if all ordinals were fixed, induction on rank would fix every set. Put $\kappa_0=\kappa$, $\kappa_{n+1}=j(\kappa_n)$ and $\lambda=\sup_{n<\omega}\kappa_n$. Since $j$ fixes $\omega$ and shifts this sequence, $j(\lambda)=\lambda$. It therefore fixes the regular [successor cardinal](../../../../../successor-cardinal.md) $\delta=\lambda^+$. The [stationarity of ordinals of prescribed cofinality](../../../../../stationarity-of-ordinals-of-prescribed-cofinality.md) gives the stationary set

$$
S=\{\beta<\delta:\operatorname{cf}(\beta)=\omega\}.
$$

Use the [stationary partition at a successor cardinal](../../../../../stationary-partition-at-a-successor-cardinal.md) to split $S$ into $\kappa$ disjoint stationary pieces $\langle S_\alpha:\alpha<\kappa\rangle$, merging pieces if necessary. Applying $j$ gives a partition $\langle T_\alpha:\alpha<j(\kappa)\rangle$ of the same $S$ into stationary pieces. The additional piece $T_\kappa$ is stationary.

The closure points

$$
C=\{\beta<\delta:(\forall\gamma<\beta)\ j(\gamma)<\beta\}
$$

form a [club set](../../../../../club-set.md). For unboundedness, repeatedly close a bound under the values of $j$ below it and take the supremum of the resulting countable sequence; regularity of $\delta$ keeps it below $\delta$. Closure under limits is immediate. Choose $\beta\in C\cap T_\kappa$ and an increasing sequence $\langle\beta_n:n<\omega\rangle$ cofinal in $\beta$. Then

$$
j(\beta)=\sup_{n<\omega}j(\beta_n)\le\beta,
$$

while every ordinal satisfies $j(\beta)\ge\beta$, so $j(\beta)=\beta$. There is an $\alpha<\kappa$ with $\beta\in S_\alpha$. Since $j(\alpha)=\alpha$, elementarity gives $\beta=j(\beta)\in j(S_\alpha)=T_\alpha$, contrary to disjointness from $T_\kappa$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
