<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\Box A=\operatorname{Pr}_{PA}(\ulcorner A\urcorner)$ for the standard [formal proof](../../../../../formal-proof.md) [predicate symbol](../../../../../predicate-symbol.md) and put

$$
\operatorname{Con}_{PA}=\neg\Box\bot.
$$

Use as given the arithmetization of syntax in PA, the [derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md), and the [diagonal lemma](../../../../../diagonal-lemma.md). The latter supplies the fixed point needed in (a), and the former conditions interpret its normal modal distribution, necessitation on theorems and axiom4. Thus the argument in (a) proves the internal Löb implication in PA. With $X=\bot$ it reads

$$
PA\vdash\Box(\Box\bot\to\bot)\to\Box\bot.
$$

The inner implication is the [first-order consistency](../../../../../first-order-consistency.md) [first-order sentence](../../../../../first-order-sentence.md) $\neg\Box\bot$, so contraposition gives

$$
\boxed{PA\vdash\operatorname{Con}_{PA}\to
\neg\operatorname{Pr}_{PA}(\ulcorner\operatorname{Con}_{PA}\urcorner).}
$$

This is the [arithmetic](../../../../../arithmetic-split.md) statement of the second incompleteness theorem proved within PA: if PA is [first-order consistent](../../../../../first-order-consistency.md), there is no PA [formal proof](../../../../../formal-proof.md) of its [first-order consistency](../../../../../first-order-consistency.md) [first-order sentence](../../../../../first-order-sentence.md). The displayed implication is a PA theorem without assuming that PA proves its antecedent.

For the corresponding external consequence, if a [first-order consistent](../../../../../first-order-consistency.md) PA proved $\operatorname{Con}_{PA}$, theoremhood would give a [formal proof](../../../../../formal-proof.md) of its boxed assertion. The displayed theorem together with the supposed [formal proof](../../../../../formal-proof.md) of [first-order consistency](../../../../../first-order-consistency.md) gives its [negation](../../../../../negation.md), contradicting [first-order consistency](../../../../../first-order-consistency.md). Hence an externally [first-order consistent](../../../../../first-order-consistency.md) PA does not prove its own [first-order consistency](../../../../../first-order-consistency.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
