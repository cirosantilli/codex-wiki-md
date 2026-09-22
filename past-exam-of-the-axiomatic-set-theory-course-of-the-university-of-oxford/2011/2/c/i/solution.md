<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

There is a [bounded definition of omega](../../../../../bounded-definition-of-omega.md). Transitivity has the bounded definition $\operatorname{Trans}(x)\equiv\forall u\in x\,\forall v\in u\,(v\in x)$. An [ordinal](../../../../../ordinal-split.md) is a [transitive set](../../../../../transitive-set.md) of [transitive sets](../../../../../transitive-set.md) on which membership is a strict total order; this too has a [bounded formula in set theory](../../../../../bounded-formula-in-set-theory.md), since [ZF](../../../../../zermelo-fraenkel-set-theory.md) supplies well-foundedness by the [Axiom of foundation](../../../../../axiom-of-regularity.md).

Define the bounded predicate

$$
L(x)\equiv\operatorname{Ord}(x)\land x\ne\varnothing\land\forall y\in x\,\exists z\in x\,(y\in z).
$$

For an [ordinal](../../../../../ordinal-split.md), this says that it is a nonzero [limit ordinal](../../../../../limit-ordinal.md). It follows in [ZF](../../../../../zermelo-fraenkel-set-theory.md) that

$$
\boxed{x=\omega\iff L(x)\land\forall y\in x\,\neg L(y),}
$$

since $\omega$ is the least nonzero [limit ordinal](../../../../../limit-ordinal.md). The right side is a [bounded formula in set theory](../../../../../bounded-formula-in-set-theory.md); consequently it is absolute between the specified [transitive models](../../../../../transitive-model.md). This also shows directly that those models have the same $\omega$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Axiomatic set theory course of the University of Oxford](../../../../../axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
