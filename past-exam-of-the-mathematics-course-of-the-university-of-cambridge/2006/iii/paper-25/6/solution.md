<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $M$ be an externally [countable](../../../../../countable-set.md) model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), and let $\kappa=(\omega_1)^M$. In $M$ form the forcing order

$$
\mathbb P=\{p:p\text{ is a finite partial function }\omega\longrightarrow\kappa\},\qquad q\le p\iff q\supseteq p.
$$

This is the [finite-function collapse to countable size](../../../../../finite-function-collapse-to-countable-size.md). For every $n\in\omega^M$ and $\alpha\in\kappa^M$, the internal [sets](../../../../../set-split.md)

$$
D_n=\{p:n\in\operatorname{dom}(p)\},\qquad E_\alpha=\{p:\alpha\in\operatorname{ran}(p)\}
$$

are dense: extend a finite [function](../../../../../function-split.md) by assigning a missing input, and use a fresh input to put any required value in its range.

Externally enumerate all the dense [subsets](../../../../../subset.md) of $\mathbb P$ which $M$ recognizes as dense. There are only countably many, because $M$ is [countable](../../../../../countable-set.md). Recursively choose $p_{i+1}\le p_i$ in the $i$th such dense [set](../../../../../set-split.md) and let $G$ be the upward closure of this descending chain. This produces a [generic filter](../../../../../generic-filter.md) over $M$. By the [forcing theorem](../../../../../forcing-theorem.md), its [generic extension](../../../../../generic-extension.md) $M[G]$ satisfies [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). The canonical [forcing name](../../../../../forcing-name.md) $\dot g=\bigcup\dot G$ is forced to be a [function](../../../../../function-split.md) with domain $\omega$ and range $\kappa$: the dense [sets](../../../../../set-split.md) $D_n$ and $E_\alpha$ ensure exactly these assertions. Therefore

$$
\boxed{M[G]\models\text{“the old }\omega_1\text{ is countable.”}}
$$

Its new first [uncountable](../../../../../uncountable-set.md) [ordinal](../../../../../ordinal.md) is accordingly different from $\kappa$.

For a transitive $M$, ordinary evaluation of names gives the familiar literal extension. The question only assumes a [countable](../../../../../countable-set.md) model, so one must also cover externally ill-founded models. In that case use the quotient of the internally defined [forcing names](../../../../../forcing-name.md) by forced equality modulo $G$, with membership defined by forced membership. The internal forcing identities and the forcing theorem hold in $M$ and give a well-defined [first-order structure](../../../../../first-order-structure.md) satisfying every standard [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) axiom. Check names embed the original membership structure, so identify their images with $M$. Its domain is a quotient of a [subset](../../../../../subset.md) of the [countable](../../../../../countable-set.md) domain of $M$, hence is externally [countable](../../../../../countable-set.md). Thus **the required extension exists even without assuming transitivity.** It is a membership extension, not an [elementary extension](../../../../../elementary-extension.md): the assertion that the parameter $\kappa$ is [uncountable](../../../../../uncountable-set.md) changes truth value.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
