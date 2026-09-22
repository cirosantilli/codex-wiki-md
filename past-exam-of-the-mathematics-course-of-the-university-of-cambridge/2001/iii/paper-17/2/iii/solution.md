<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [preservation obstructions to extending an adjoint chain](../../../../../../preservation-obstructions-to-extending-an-adjoint-chain.md): a [functor](../../../../../../functor.md) having a further [left adjoint](../../../../../../adjoint-functors.md) must preserve [categorical limits](../../../../../../categorical-limit.md), while one having a further [right adjoint](../../../../../../adjoint-functors.md) must preserve [colimits](../../../../../../colimit.md).

At the left end of the [presheaf category](../../../../../../presheaf-category.md) chain, $\Lambda$ does not preserve the [terminal object](../../../../../../terminal-object.md). The terminal [categorical presheaf](../../../../../../presheaf-category-theory.md) has singleton value everywhere, whereas $(\Lambda1)(S)=\varnothing$ because $S\ne\varnothing$. Thus $\Lambda$ cannot itself be a [right adjoint](../../../../../../adjoint-functors.md). At the right end, $\nabla$ does not preserve the [initial object](../../../../../../initial-object.md): $(\nabla\varnothing)(\varnothing)=\{*\}$ since the empty open set is proper. Thus $\nabla$ cannot itself be a [left adjoint](../../../../../../adjoint-functors.md).

For the [category of small categories](../../../../../../category-of-small-categories.md) chain, take two [functors](../../../../../../functor.md) from the [terminal category](../../../../../../terminal-category.md) $1$ to the two-object [indiscrete category](../../../../../../indiscrete-category.md) $I\{0,1\}$, selecting its distinct objects. Their [equalizer](../../../../../../equaliser.md) is the empty [category](../../../../../../category-split.md). But their images under $C=\pi_0$ are the same function between singleton [sets](../../../../../../set-split.md), whose [equalizer](../../../../../../equaliser.md) is a singleton. Hence $C$ does not preserve [equalizers](../../../../../../equaliser.md) and has no further [left adjoint](../../../../../../adjoint-functors.md). Finally, $I1\amalg I1$ is the two-object [discrete category](../../../../../../discrete-category.md), while $I(1\amalg1)$ has arrows between its distinct objects. The canonical comparison is not an [isomorphism of categories](../../../../../../isomorphism-of-categories.md), so $I$ fails to preserve this [coproduct](../../../../../../coproduct.md) and has no further [right adjoint](../../../../../../adjoint-functors.md).

**Neither chain extends in either direction.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
