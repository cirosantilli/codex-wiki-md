<h1 id="11/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An [inner model](../../../../../../inner-model.md) of [ZF](../../../../../../zermelo-fraenkel-set-theory.md) is a [transitive class](../../../../../../transitive-class.md) $N$ containing all [ordinals](../../../../../../ordinal.md) and satisfying [ZF](../../../../../../zermelo-fraenkel-set-theory.md) with the inherited membership relation. The “all [ordinals](../../../../../../ordinal.md)” requirement is important: an arbitrary transitive [set](../../../../../../set-split.md) model or a rank segment is not an inner model in this sense.

Every such inner model contains the ambient [constructible universe](../../../../../../constructible-universe.md) $L$. Here is the reason. Inductively $L_\alpha^N=L_\alpha$. The zero stage is the same [empty set](../../../../../../empty-set.md). If the stages at $\alpha$ agree, satisfaction for the common [set](../../../../../../set-split.md) structure $(L_\alpha,\in)$ is absolute: atomic [first-order formulas](../../../../../../first-order-formula.md) agree, Boolean operations agree, and quantified variables range over the identical [set](../../../../../../set-split.md). The codes of finite [first-order formulas](../../../../../../first-order-formula.md) are also the same because a [transitive model](../../../../../../transitive-model.md) of [ZF](../../../../../../zermelo-fraenkel-set-theory.md) has the actual [natural numbers](../../../../../../natural-number.md). Consequently definability with parameters from $L_\alpha$ produces exactly the same [subsets](../../../../../../subset.md) in both models, so their successor constructible stages agree. At a [limit ordinal](../../../../../../limit-ordinal.md) both constructions take the [union](../../../../../../set-union.md) of the same earlier stages. This proves agreement at every stage and hence $L\subseteq N$.

The [constructible universe theorem](../../../../../../constructible-universe-theorem.md) provides models of [ZF](../../../../../../zermelo-fraenkel-set-theory.md) satisfying $V=L$ and the [axiom of choice](../../../../../../axiom-of-choice.md), whenever [ZF](../../../../../../zermelo-fraenkel-set-theory.md) is consistent. In such a universe any inner model $N$ of [ZF](../../../../../../zermelo-fraenkel-set-theory.md) satisfies

$$
L=V\subseteq N\subseteq V,
$$

so $N=V$ and it also satisfies choice. Therefore

$$
\boxed{\text{No uniform inner-model construction from arbitrary ZF models can establish }\neg\mathsf{AC}.}
$$

Passing to $L$ proves the consistency of choice, but the same downward method cannot prove its negation from an arbitrary starting model: it has no possible output when the starting universe is constructible. This is the precise obstruction intended in an inner-model independence argument. It is not a claim that every inner model of every choice universe satisfies choice; symmetric submodels of suitable forcing extensions can fail choice, and that method first changes the ambient universe.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11](../../11.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
