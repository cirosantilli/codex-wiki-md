<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

I would defend the assertion as a description of what good abstraction achieves, provided it is not taken to mean that finding the abstraction is easy. [Category theory](../../../../../category-theory-split.md) makes recurring arguments consequences of a common [universal property](../../../../../universal-property.md), instead of requiring a new calculation in every setting.

The [Yoneda lemma](../../../../../yoneda-lemma.md) is an instructive example. A [natural transformation](../../../../../natural-transformation.md) from $\mathcal C(c,-)$ to a set-valued functor $F$ is determined by its value on $1_c$; naturality forces its value at $u:c\to d$ to be $F(u)$ of that element. Once the right question is asked, the proof is short. Yet the statement explains why representable functors encode objects faithfully, and why a functor can be reconstructed from its elements. The simplicity belongs to the organized argument, not to a claim that these consequences were obvious beforehand.

Likewise, the fact that a [right adjoint](../../../../../adjoint-functors.md) preserves [categorical limits](../../../../../categorical-limit.md) does not need separate proofs for products, equalizers and pullbacks in every example. The [adjunction](../../../../../adjoint-functors.md) converts a map into the proposed limit into a compatible family of maps, and the [natural bijection](../../../../../natural-bijection.md) converts that family back. This one argument explains preservation of many different constructions. It also makes the canonical comparison maps clear, which matters more than merely guessing an isomorphism of the resulting objects.

The [monoidal coherence theorem](../../../../../monoidal-coherence-theorem.md) shows a different benefit. Complicated calculations with bracketed [tensor products](../../../../../tensor-product.md) can become transparent because every structural rebracketing is the unique map between its formal source and target. However, the proof that the pentagon and triangle suffice is real work. Suppressing brackets is justified by that proof; it cannot serve as a substitute for it. Abstraction is valuable precisely because it separates an essential compatibility argument from subsequent routine bookkeeping.

There is also a necessary caution. The [general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) requires a [solution-set condition](../../../../../solution-set-condition.md); small-limit preservation by itself does not produce a left adjoint. The reverse-ordinal example makes the missing condition concrete. Similarly, the [monad](../../../../../monad.md) of an adjunction need not capture all the structure in the original category: the tower of [nested partial unary operation categories](../../../../../nested-partial-unary-operation-category.md) has arbitrary finite [monadic length](../../../../../monadic-length.md), despite its long composites sharing their first induced monad. These examples prevent formal language from hiding a size problem or an unjustified reconstruction claim.

**The persuasive interpretation is that abstraction makes the reason for a result visible and reusable.** It often turns the final step into a direct consequence of definitions, while leaving the discovery of those definitions and the verification of their hypotheses as substantial mathematics.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
