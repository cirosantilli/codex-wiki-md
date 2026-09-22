<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The rank characterization holds for a set relation, or a [set-like](../../../../../../../set-like-relation.md) class relation.** For such a [well-founded relation](../../../../../../../well-founded-relation.md), use [well-founded recursion](../../../../../../../well-founded-recursion.md) to define

$$
\boxed{\rho(y)=\sup\{\rho(x)+1:xRy\}.}
$$

The predecessor set is a set, so the [supremum](../../../../../../../supremum.md) is an [ordinal](../../../../../../../ordinal.md). For a [set-like](../../../../../../../set-like-relation.md) class relation, the closure of the predecessors of any one point under finitely many predecessor steps is a set; perform the ordinary set recursion there. Uniqueness makes these local definitions agree, producing a class rank function. The formula immediately gives $xRy\Rightarrow\rho(x)<\rho(y)$.

Conversely, suppose such an ordinal-valued function exists. For any nonempty subset, or nonempty subclass in the class formulation, take an element whose rank is least among the ranks occurring. It has no predecessor in that subset or subclass, because a predecessor would have smaller rank. This proves well-foundedness.

There is a qualification in the printed class formulation. If well-founded class relations are defined to include [set-likeness](../../../../../../../set-like-relation.md), it is already implicit and the assertion is correct. Under the minimal-element definition alone, it must be supplied. Without [set-likeness](../../../../../../../set-like-relation.md), let $X=\operatorname{Ord}\cup\{u\}$, where $u=\{1\}$ is not an [ordinal](../../../../../../../ordinal.md), and put every ordinal below $u$, with the usual ordinal order below it. Every nonempty subclass has a minimal element, so the relation is well founded. But [transfinite induction](../../../../../../../transfinite-induction.md) forces $\rho(\alpha)\geq\alpha$ for all ordinals, whereas $\rho(u)$ would have to exceed every $\rho(\alpha)$. No such ordinal exists. Thus the unrestricted class assertion is false; **set-likeness is necessary for this standard rank proof**.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
