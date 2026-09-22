<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $T$ be [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) together with the assertion of unboundedly many [inaccessible cardinals](../../../../../../strongly-inaccessible-cardinal.md). Given a model of $T$, if it has no [inaccessible limit of inaccessibles](../../../../../../inaccessible-limit-of-inaccessibles.md), it already witnesses the required nonimplication. Otherwise let $\iota$ be its least [inaccessible limit of inaccessibles](../../../../../../inaccessible-limit-of-inaccessibles.md) and pass to its rank segment $V_\iota$.

Because $\iota$ is an [inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md), $V_\iota$ satisfies [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md). Its [ordinals](../../../../../../ordinal.md) are precisely those below $\iota$, and below $\iota$ the inaccessible cardinals are unbounded by the choice of $\iota$. Inaccessibility of any smaller ordinal is absolute to this segment: it has the same subsets and functions on all smaller ordinals, as in [strong-inaccessibility absoluteness from rank agreement](../../../../../../strong-inaccessibility-absoluteness-from-rank-agreement.md). Thus $V_\iota$ satisfies the unbounded-inaccessibles assertion.

No smaller ordinal can be an [inaccessible limit of inaccessibles](../../../../../../inaccessible-limit-of-inaccessibles.md), by minimality of $\iota$ and the same absoluteness. Also $\iota$ is not an ordinal of $V_\iota$ itself. Consequently

$$
\boxed{V_\iota\models T+\neg\mathrm{ILI}}.
$$

This [rank cutoff at the first inaccessible limit of inaccessibles](../../../../../../rank-cutoff-at-the-first-inaccessible-limit-of-inaccessibles.md) proves $\operatorname{Con}(T)\Rightarrow\operatorname{Con}(T+\neg\mathrm{ILI})$. The [soundness theorem for first-order logic](../../../../../../soundness-theorem-for-first-order-logic.md) then gives $T\not\vdash\mathrm{ILI}$ if $T$ is consistent. This is a model-theoretic relative-consistency argument, and does not infer external transitivity from mere consistency.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
