# Existential quantification

↑ **Parent:** [First-order formula](first-order-formula.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Existential_quantification)

[Existential quantification](existential-quantification.md) forms $\exists x\,\varphi(x,\mathbf y)$. In a [first-order structure](first-order-structure.md), it is true at an assignment to $\mathbf y$ when some domain element makes the instance true. In [natural deduction](natural-deduction.md), elimination uses a fresh variable for the hypothetical witness; that variable may not escape into the conclusion or the remaining undischarged assumptions.

Existence requires at least one witness, not exactly one. Over the [natural numbers](natural-number.md) $\mathbb N=\{0,1,2,\ldots\}$, $\exists m\,(m>5)$ is true: $m=6$ works, as do $7,8,\ldots$. In [intuitionistic first-order logic](intuitionistic-first-order-logic.md), a direct proof supplies a witness together with a proof of the corresponding instance; merely rejecting nonexistence is generally weaker.

Placing [existential quantification](existential-quantification.md) before [universal quantification](universal-quantification.md) requires a single witness that works throughout:

$$
\exists m\in\mathbb N\,\forall n\in\mathbb N\;(m>n).
$$

This [first-order sentence](first-order-sentence.md) is false. For any proposed $m$, choose $n=m$: the required inequality becomes $m>m$. For example, $m=3$ works for $n=0,1,2$ but fails at $n=3$. No finite list of successful checks establishes [universal quantification](universal-quantification.md) over the [natural numbers](natural-number.md).

**Table of contents**

- [Existential formula](existential-formula.md)

## ↑ Ancestors (7)

1. [First-order formula](first-order-formula.md)
2. [First-order logic](first-order-logic.md)
3. [Mathematical logic](mathematical-logic-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Coherent logic](coherent-logic.md)
- [Existence](existence.md)
- [Existential quantification](existential-quantification.md)
- [Existential second-order logic](existential-second-order-logic.md)
- [Mathematical logic](mathematical-logic-split.md)
- [Nondeterministic finite automaton](nondeterministic-finite-automaton.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-74/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-20/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-23/1/a/solution.md)
- [Primitive positive formula](primitive-positive-formula.md)
- [Quantifier](quantifier.md)
- [Second-order logic](second-order-logic.md)
- [Set union](set-union.md)
- [Uniform convergence](uniform-convergence.md)
- [Universal quantification](universal-quantification.md)
