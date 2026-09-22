<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

We give a relative-consistency argument using a [finite-function collapse to countable size](../../../../../../finite-function-collapse-to-countable-size.md). The assumed consistency implies that [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) is consistent. Passing to the [constructible universe](../../../../../../constructible-universe.md) gives consistency of $\mathsf{ZFC}+V=L$, which also satisfies the [Generalized continuum hypothesis](../../../../../../generalized-continuum-hypothesis.md). Work in this ground theory, let $\delta=\omega_1^L$, and force with finite [partial functions](../../../../../../partial-function.md) $\omega\rightharpoonup\delta$, ordered by reverse inclusion.

The union of a [generic filter](../../../../../../generic-filter.md) $H$ is a total surjection $h:\omega\to\delta$: prescribing a new domain coordinate is dense, and putting any specified $\gamma<\delta$ into the range is dense. Hence $\delta$ becomes countable. Set forcing preserves ordinals, and [absoluteness of constructible levels](../../../../../../absoluteness-of-constructible-levels.md) implies that the extension has the same constructible universe as the ground model. Its $\omega_1^L$ is therefore still the old $\delta$, so it satisfies the stated [countability of constructible omega-one](../../../../../../countability-of-constructible-omega-one.md) condition.

We must also verify GCH after the collapse. The order has ground-model size $\delta$, hence the $\delta^+$-chain condition. By [cardinal preservation by chain-condition forcing](../../../../../../cardinal-preservation-by-chain-condition-forcing.md), all old cardinals at least $\delta^+$ survive. Every old ordinal below $\delta^+$ has size at most $\delta$ and becomes countable, so the old $\delta^+$ is exactly the new $\omega_1$.

A name for a subset of a fixed ground-model ordinal $\lambda$ can be chosen as a set of pairs $(\check\xi,p)$ with $\xi<\lambda$ and $p$ a condition: use an antichain deciding membership at each coordinate. Thus the number of such names in the ground model is at most $2^{|\lambda\times\mathbb P|}$. For subsets of $\omega$ this is $2^\delta=\delta^+$ by ground-model GCH. In the extension it gives $2^{\aleph_0}\leq\delta^+=\aleph_1$, and [Cantor theorem](../../../../../../cantor-s-theorem.md) gives the reverse lower bound. For every old cardinal $\lambda\geq\delta^+$ the bound is

$$
2^{\lambda\cdot\delta}=2^\lambda=\lambda^+
$$

in the ground model. Both $\lambda$ and $\lambda^+$ remain cardinals, so again the upper bound and [Cantor theorem](../../../../../../cantor-s-theorem.md) give the extension's equality $2^\lambda=\lambda^+$. These are all its uncountable cardinals. This proves [GCH preservation by a finite-function collapse](../../../../../../gch-preservation-by-a-finite-function-collapse.md) in the required case.

The forcing relative-consistency theorem now yields

$$
\boxed{\operatorname{Con}(\mathsf{ZFC}+\mathrm{NC})\ \Longrightarrow\ \operatorname{Con}(\mathsf{ZFC}+\mathrm{NC}+\mathrm{GCH}).}
$$

The construction in fact only needs consistency of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md). This argument uses the formal inner-model and forcing consistency theorems; it does not infer the existence of a [countable transitive model](../../../../../../countable-transitive-model.md) merely from consistency.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
