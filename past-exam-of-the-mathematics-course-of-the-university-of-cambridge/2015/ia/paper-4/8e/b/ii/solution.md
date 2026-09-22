<h1 id="8e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [integers](../../../../../../../integer.md) are countable: $j(z)=2z+1$ for $z\ge0$ and $j(z)=-2z$ for $z<0$ is an [injection](../../../../../../../injective-function.md) $\mathbb Z\to\mathbb N$. Hence $\mathbb Z\times\mathbb N$ is a [countable set](../../../../../../../countable-set.md). The map $(a,b)\mapsto a/b$ is a [surjection](../../../../../../../surjective-function.md) onto the [rational numbers](../../../../../../../rational-number.md), so the image result already proved gives **$\mathbb Q$ is countable**. Unique reduced fractions are not required for this [surjection](../../../../../../../surjective-function.md) argument.

For the final unheaded geometry request, suppose for contradiction that no two distinct circles in the collection intersect. Restrict to the subcollection $\mathcal C_0$ of circles tangent to the $x$-axis. Each such nondegenerate [circle](../../../../../../../circle.md) has a unique tangency point, and the tangency-point map $\mathcal C_0\to\mathbb R$ is a [surjection](../../../../../../../surjective-function.md) by the hypothesis.

The closed disk of a circle tangent at $(a,0)$ meets the $x$-axis only at $(a,0)$. Two distinct members of $\mathcal C_0$ cannot have nested disks: if one disk were inside the other, its tangency point would belong to the larger disk, so both tangency points would be equal and both circle boundaries would pass through it. That already contradicts nonintersection. Circles with disjoint boundaries and no nesting have disjoint disks. Thus their open disks are pairwise disjoint.

By the [density of the rational numbers](../../../../../../../density-of-the-rational-numbers.md), every nonempty open disk contains a point of $\mathbb Q^2$, which is a [countable set](../../../../../../../countable-set.md). Fix an enumeration of $\mathbb Q^2$ and assign to each disk the first enumerated point inside it. Disjointness makes this assignment an [injection](../../../../../../../injective-function.md). This is the [countability of pairwise disjoint open disks](../../../../../../../countability-of-pairwise-disjoint-open-disks.md), and proves that $\mathcal C_0$ is a [countable set](../../../../../../../countable-set.md). Its [surjection](../../../../../../../surjective-function.md) onto $\mathbb R$ would make the [real numbers](../../../../../../../real-number.md) countable, contrary to the [Cantor diagonal argument](../../../../../../../cantor-diagonal-argument.md). Therefore

$$
\boxed{\text{The collection contains two distinct intersecting circles.}}
$$

The proof allows circles on either side of the axis and counts tangential contact as intersection; it does not assume that all circles in the original collection are tangent to the axis.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8E](../../../8e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
