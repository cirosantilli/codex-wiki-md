<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [arithmetic](../../../../../arithmetic-split.md) [logical formula](../../../../../logical-formula.md) is $\Sigma_0$, or bounded, if all its [quantifiers](../../../../../quantifier.md) are bounded by arithmetical [first-order terms](../../../../../first-order-term.md). A $\Sigma_1$ [logical formula](../../../../../logical-formula.md) has an initial block of [existential quantifiers](../../../../../existential-quantification.md) followed by a bounded matrix, up to the usual logical transformations. [Soundness of an arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) at a given level means that every [first-order sentence](../../../../../first-order-sentence.md) of that level proved by the [first-order theory](../../../../../first-order-theory.md) is true in the standard [natural numbers](../../../../../natural-number.md). Here $\Sigma_0$-completeness means that every true [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md) is provable.

A [first-order theory](../../../../../first-order-theory.md) is [one-consistent](../../../../../one-consistency.md) if there is no [bounded arithmetic formula](../../../../../arithmetic-bounded-formula.md) $A(x)$ for which it proves $\exists xA(x)$ while proving $\neg A(\bar n)$ for every standard [natural number](../../../../../natural-number.md) $n$. This is a restricted form of [omega-consistency](../../../../../omega-consistency-of-an-arithmetic-theory.md). In particular [one-consistency](../../../../../one-consistency.md) implies [first-order consistency](../../../../../first-order-consistency.md), since an inconsistent [first-order theory](../../../../../first-order-theory.md) proves every [first-order sentence](../../../../../first-order-sentence.md) and its [negation](../../../../../negation.md).

Suppose a $\Sigma_0$-complete [first-order theory](../../../../../first-order-theory.md) $S$ is [first-order consistent](../../../../../first-order-consistency.md). If it proved a false [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md) $\theta$, the true [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md) $\neg\theta$ would also be provable by completeness, contradicting [first-order consistency](../../../../../first-order-consistency.md). Thus $S$ is $\Sigma_0$-sound. Conversely $\Sigma_0$-soundness excludes inconsistency because an inconsistent [first-order theory](../../../../../first-order-theory.md) proves the false [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md) $0=1$. Therefore

$$
\boxed{\Sigma_0\text{-complete}:\quad\operatorname{Con}(S)\iff\Sigma_0\text{-soundness}.}
$$

If $S$ is [one-consistent](../../../../../one-consistency.md) but proved a false [existential sentence](../../../../../existential-sentence.md) $\exists xA(x)$ with bounded matrix, every standard instance $\neg A(\bar n)$ would be true and hence provable. This violates [one-consistency](../../../../../one-consistency.md). Thus it is $\Sigma_1$-sound. Conversely, $\Sigma_1$-soundness implies [first-order consistency](../../../../../first-order-consistency.md) by the previous argument, since [bounded arithmetic sentences](../../../../../bounded-arithmetic-sentence.md) are included at the existential level. If $S$ proved $\exists xA(x)$, [soundness of an arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) would give a standard witness $n$ with $A(n)$ true. [Bounded completeness of an arithmetic theory](../../../../../bounded-completeness-of-an-arithmetic-theory.md) would then give $S\vdash A(\bar n)$, so [first-order consistency](../../../../../first-order-consistency.md) prevents simultaneous [formal proofs](../../../../../formal-proof.md) of all the negated instances. Hence

$$
\boxed{\Sigma_0\text{-complete}:\quad1\text{-consistency}\iff\Sigma_1\text{-soundness}.}
$$

Multiple existential [logical variables](../../../../../logical-variable.md) can be treated as a finite [tuple](../../../../../finite-tuple.md) of witnesses; the same reasoning applies.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
