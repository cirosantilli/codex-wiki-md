<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

Let $p$ be a [permutation](../../../../../permutation.md) of the finite set. Starting from $a$, repeatedly apply $p$. Some iterate repeats; because $p$ is invertible, the first repeat closes the sequence at $a$. More explicitly, if $p^i(a)=p^j(a)$ with $0\le i<j$, applying $p^{-i}$ gives $p^{j-i}(a)=a$. If $r$ is the least positive return time, the elements $a,p(a),\ldots,p^{r-1}(a)$ are distinct and form one [permutation cycle](../../../../../permutation-cycle.md). If the set is not exhausted, start again at an unused element. Two such sets cannot overlap: an overlap lets an inverse iterate express either starting point as an iterate of the other, making the sets identical. Thus this process partitions the set into [disjoint permutation cycles](../../../../../disjoint-permutation-cycles.md). On each part its cycle acts exactly as $p$ and the other cycles fix the elements. Their product therefore equals $p$. This proves existence of the [cycle decomposition of a permutation](../../../../../cycle-decomposition-of-a-permutation.md), including one-cycles for fixed points.

Use the composition convention that the rightmost [permutation](../../../../../permutation.md) acts first. For the specified product, the images are

$$
1\mapsto2\mapsto3\mapsto1,\qquad4\mapsto5\mapsto4,\qquad6\mapsto7\mapsto8\mapsto6.
$$

Hence

$$
\boxed{\sigma\tau=(123)(45)(678),\qquad\operatorname{ord}(\sigma\tau)=6.}
$$

The [order of a group element](../../../../../order-of-a-group-element.md) here is the least positive exponent making every cycle return to the identity. It must be divisible by each cycle length, and any common multiple does make every cycle return. The [least common multiple](../../../../../least-common-multiple.md) of $3,2,3$ is six.

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
