<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [Lebesgue measurable function](../../../../../lebesgue-measurable-function.md) $f:\mathbb R\to\mathbb R$, the [preimage](../../../../../preimage.md) $f^{-1}(U)$ of every open [set](../../../../../set-split.md) $U$ is a [Lebesgue measurable set](../../../../../lebesgue-measurable-set.md). For a [Borel measurable function](../../../../../borel-measurable-function.md), each such preimage must instead be a [Borel set](../../../../../borel-set.md). Equivalently, both definitions can test all Borel target sets: the collection

$$
\mathcal C_f=\{B\subseteq\mathbb R:f^{-1}(B)\text{ belongs to the source sigma-algebra}\}
$$

is a [sigma-algebra](../../../../../sigma-algebra.md), since preimages preserve complements and countable unions. Containing all open sets therefore makes it contain the [Borel sigma-algebra](../../../../../borel-sigma-algebra.md).

Now let $U$ be open. Since $h$ is a [Borel measurable function](../../../../../borel-measurable-function.md), $h^{-1}(U)$ is Borel. Since $g$ is a [Lebesgue measurable function](../../../../../lebesgue-measurable-function.md), $g^{-1}(h^{-1}(U))$ is a Lebesgue measurable set. But

$$
(h\circ g)^{-1}(U)=g^{-1}(h^{-1}(U)).
$$

Thus **$h\circ g$ is a [Lebesgue measurable function](../../../../../lebesgue-measurable-function.md)**. The intermediate sigma-algebra is Borel; this is why [Borel postcomposition preserves Lebesgue measurability](../../../../../borel-postcomposition-preserves-lebesgue-measurability.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
