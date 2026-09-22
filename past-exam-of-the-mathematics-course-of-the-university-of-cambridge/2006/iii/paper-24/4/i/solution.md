<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [left adjoint](../../../../../../adjoint-functors.md) to the morphism-set [functor](../../../../../../functor.md) is the [free category on independent arrows](../../../../../../free-category-on-independent-arrows.md):

$$
L(S)=\coprod_{s\in S}[1].
$$

Each copy has two objects, their identities, and one nonidentity arrow from the first object to the second. A [functor](../../../../../../functor.md) $L(S)\to\mathcal C$ is specified by one arbitrary arrow of $\mathcal C$ for each $s$, since that arrow specifies the images of both objects as well. This proves the natural adjunction bijection with functions $S\to\operatorname{Mor}(\mathcal C)$.

The induced [monad](../../../../../../monad.md) on sets has $T(S)=S\times\{\text{source identity},\text{generator},\text{target identity}\}$. For a singleton $S$, its multiplication is a function from the nine-element set $T^2S$ to the three-element set $TS$, so it cannot be invertible. **This adjunction is not idempotent.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
