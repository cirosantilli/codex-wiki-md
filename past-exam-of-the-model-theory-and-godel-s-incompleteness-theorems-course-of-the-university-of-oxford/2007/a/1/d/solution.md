<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Start with the supplied bounded-complete, [one-consistent](../../../../../one-consistency.md) [first-order theory](../../../../../first-order-theory.md) $T$ proving a false [first-order sentence](../../../../../first-order-sentence.md) $F$. Replace it by its deductive closure, which preserves these properties and contains $F$. Enumerate the [arithmetic](../../../../../arithmetic-split.md) [first-order sentences](../../../../../first-order-sentence.md) as $X_0,X_1,\ldots$. Recursively extend the current [first-order theory](../../../../../first-order-theory.md) by either $X_n$ or $\neg X_n$, choosing an extension which remains [one-consistent](../../../../../one-consistency.md) as permitted by the supplied lemma, and then take its deductive closure. Call the resulting increasing sequence $T_n$, with $T_0$ the initial [first-order theory](../../../../../first-order-theory.md), and put $S=\bigcup_nT_n$.

Every stage is still bounded-complete. By (b), every stage has [Sigma-1 soundness](../../../../../sigma-1-soundness.md). If $S$ proved a false Sigma-1 [first-order sentence](../../../../../first-order-sentence.md), the finite [formal proof](../../../../../formal-proof.md) would use assumptions from one stage $T_n$, contradicting its [Sigma-1 soundness](../../../../../sigma-1-soundness.md). Thus $S$ has [Sigma-1 soundness](../../../../../sigma-1-soundness.md) and is bounded-complete, so (b) makes it [one-consistent](../../../../../one-consistency.md).

This [soundness of an arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) argument is essential: the definition of [one-consistency](../../../../../one-consistency.md) involves infinitely many standard refutations, so it would be insufficient merely to say that a violation has a finite [formal proof](../../../../../formal-proof.md). What has a finite [formal proof](../../../../../formal-proof.md) is the false [existential sentence](../../../../../existential-sentence.md), and [bounded completeness of an arithmetic theory](../../../../../bounded-completeness-of-an-arithmetic-theory.md) is what turns [one-consistency](../../../../../one-consistency.md) into the needed [soundness of an arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) condition.

The [union](../../../../../set-union.md) is deductively closed because each [formal proof](../../../../../formal-proof.md) has finitely many assumptions. It contains either $X$ or $\neg X$ for every [first-order sentence](../../../../../first-order-sentence.md), by the [numeralwise enumeration in arithmetic](../../../../../numeralwise-enumeration-in-arithmetic.md), and contains the false [first-order sentence](../../../../../first-order-sentence.md) $F$. If it were omega-consistent, (c) would make it correct on all [first-order sentences](../../../../../first-order-sentence.md), contradicting $F$. We have therefore constructed

$$
\boxed{S\text{ complete and one-consistent, but not omega-consistent}.}
$$

[Omega-consistency](../../../../../omega-consistency-of-an-arithmetic-theory.md) always implies [one-consistency](../../../../../one-consistency.md) by restricting its matrices. This counterexample proves that the converse is strictly false.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
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
