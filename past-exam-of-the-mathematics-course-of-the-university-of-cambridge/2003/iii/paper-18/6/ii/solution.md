<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D(S)$ be the [discrete category](../../../../../../discrete-category.md) on $S$, and $I(S)$ the [indiscrete category](../../../../../../indiscrete-category.md), with exactly one morphism between each ordered pair of objects. A [functor](../../../../../../functor.md) $D(S)\to\mathcal A$ is precisely a map $S\to O(\mathcal A)$; a [functor](../../../../../../functor.md) $\mathcal A\to I(S)$ is precisely a map $O(\mathcal A)\to S$. Thus $D\dashv O\dashv I$.

Let $C(\mathcal A)=\pi_0\mathcal A$ be the set of connected components, where objects are related by finite zigzags of morphisms in either direction. A [functor](../../../../../../functor.md) $\mathcal A\to D(S)$ must take the endpoints of every morphism to the same point, so it is exactly a map $\pi_0\mathcal A\to S$. This gives the [adjoint chain for the objects of a category](../../../../../../adjoint-chain-for-the-objects-of-a-category.md)

$$
\boxed{C\dashv D\dashv O\dashv I.}
$$

It cannot extend to the left. The two [functors](../../../../../../functor.md) from the terminal category to $I(\{0,1\})$ selecting distinct objects have empty [equalizer](../../../../../../equaliser.md) in $\mathbf{Cat}$. Applying $C$ gives two identical maps between singleton sets, whose [equalizer](../../../../../../equaliser.md) is a singleton. Thus $C$ does not preserve [equalizers](../../../../../../equaliser.md) and cannot be a right adjoint.

It cannot extend to the right either. The coproduct of two copies of $I(1)$ in $\mathbf{Cat}$ is the discrete two-object category. But $I(1\amalg1)$ is the indiscrete two-object category, with morphisms between its distinct objects. They are not isomorphic, or even equivalent. Hence $I$ does not preserve binary coproducts and cannot be a left adjoint. **Neither end of this chain has a further adjoint.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
