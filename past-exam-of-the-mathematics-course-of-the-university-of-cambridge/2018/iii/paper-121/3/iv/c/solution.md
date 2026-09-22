<h1 id="3/iv/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $M$ satisfies the [countable chain condition for forcing](../../../../../../../countable-chain-condition-for-forcing.md). We prove [cardinal preservation by chain-condition forcing](../../../../../../../cardinal-preservation-by-chain-condition-forcing.md) using the [possible-values lemma for chain-condition forcing](../../../../../../../possible-values-lemma-for-chain-condition-forcing.md), and give the argument explicitly for ccc.

Let $\kappa$ be an uncountable cardinal of $M$. If it ceased to be a cardinal, some ordinal $\mu<\kappa$ would admit a surjection onto $\kappa$ in an extension. By the [forcing theorem](../../../../../../../forcing-theorem.md), there would be a condition $p$ and a [forcing name](../../../../../../../forcing-name.md) $\dot f$ such that

$$
p\Vdash\dot f:\check\mu\twoheadrightarrow\check\kappa.
$$

Inside $M$, for each $\xi<\mu$ choose a maximal [antichain in a forcing order](../../../../../../../antichain-in-a-forcing-order.md) below $p$ deciding the ordinal value of $\dot f(\xi)$. Conditions deciding that value are dense below $p$. The chain condition makes the chosen antichain countable in $M$, so the corresponding set $B_\xi\subseteq\kappa$ of possible decided values is countable in $M$.

A [generic filter](../../../../../../../generic-filter.md) containing $p$ meets the downward closure of every such maximal antichain, so its value $f(\xi)$ belongs to $B_\xi$. Therefore its whole range lies in the ground-model set

$$
B=\bigcup_{\xi<\mu}B_\xi,\qquad |B|^M\leq|\mu|^M\cdot\aleph_0<\kappa.
$$

The last inequality is [infinite cardinal arithmetic](../../../../../../../infinite-cardinal-arithmetic.md) and uses only that $\kappa$ is uncountable and $\mu<\kappa$; no regularity of $\kappa$ is needed. Some ordinal in $\kappa\setminus B$ exists already in $M$ and cannot occur in the range, contradicting the forced surjectivity.

Finite cardinals cannot collapse, and $\omega$ cannot become finite: a finite domain has finite image, and transitive models agree on the [natural numbers](../../../../../../../natural-number.md). Old non-cardinals cannot become cardinals because their old bijections persist. Thus

$$
\boxed{\mathbb P\text{ is ccc in }M\quad\Longrightarrow\quad\operatorname{Card}^{M[G]}=\operatorname{Card}^{M}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Iv](../../iv.md)
3. [3](../../../3.md)
4. [Paper 121](../../../../paper-121-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
