<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

It suffices to obtain a [model of ZFC without weakly inaccessible cardinals](../../../../../../model-of-zfc-without-weakly-inaccessible-cardinals.md). Starting with any model of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md), pass to its [constructible universe](../../../../../../constructible-universe.md), which satisfies [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) and the [Generalized continuum hypothesis](../../../../../../generalized-continuum-hypothesis.md). If it has no [inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md), use that model. Otherwise pass to its rank segment at its least [inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) $\delta$. This segment satisfies [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md), retains the [Generalized continuum hypothesis](../../../../../../generalized-continuum-hypothesis.md), and has no [inaccessible cardinals](../../../../../../strongly-inaccessible-cardinal.md). Under the [Generalized continuum hypothesis](../../../../../../generalized-continuum-hypothesis.md), every [weakly inaccessible cardinal](../../../../../../weakly-inaccessible-cardinal.md) is strongly inaccessible: if $\lambda<\kappa$ and $\kappa$ is a [limit cardinal](../../../../../../limit-cardinal.md), then $2^\lambda=\lambda^+<\kappa$. Thus in either case the resulting model $N$ has no [weakly inaccessible cardinals](../../../../../../weakly-inaccessible-cardinal.md).

Work inside $N$. If $\alpha$ is a nonzero [limit ordinal](../../../../../../limit-ordinal.md), let $\lambda=\sup_{\beta<\alpha}\sigma_\beta$. It is an uncountable [limit cardinal](../../../../../../limit-cardinal.md). If it were regular, it would be a [weakly inaccessible cardinal](../../../../../../weakly-inaccessible-cardinal.md), which is impossible in $N$. It is therefore singular, and the [singular cardinal enumeration](../../../../../../singular-cardinal-enumeration.md) is continuous at this index:

$$
\sigma_\alpha=\sup_{\beta<\alpha}\sigma_\beta.
$$

The [cofinality of an increasing ordinal supremum](../../../../../../cofinality-of-an-increasing-ordinal-supremum.md) now gives

$$
\boxed{\operatorname{cf}(\sigma_\alpha)=\operatorname{cf}(\alpha)}
$$

for every nonzero [limit ordinal](../../../../../../limit-ordinal.md) $\alpha$ in $N$. Hence $N$ satisfies the negation of the proposed existential assertion. By the [soundness theorem for first-order logic](../../../../../../soundness-theorem-for-first-order-logic.md), consistency of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) prevents [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) from proving that assertion. The model construction is a relative-consistency argument; it does not assume that consistency alone supplies a [countable transitive model](../../../../../../countable-transitive-model.md). Here, as usual, a [limit ordinal](../../../../../../limit-ordinal.md) excludes zero.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
