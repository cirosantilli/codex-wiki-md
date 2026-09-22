<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [well-order](../../../../../../well-order.md) of the [natural numbers](../../../../../../natural-number.md) to list $A$ in increasing order. Define recursively

$$
f(0)=\min A,\qquad f(n+1)=\min\bigl(A\setminus\{f(0),\ldots,f(n)\}\bigr).
$$

The remaining [set](../../../../../../set-split.md) is nonempty because $A$ is infinite and only a [finite set](../../../../../../finite-set.md) has been removed. Each chosen value is larger than the preceding one, so $f$ is an [injective function](../../../../../../injective-function.md).

To prove it is a [surjective function](../../../../../../surjective-function.md), fix $a\in A$. If $a$ were never selected, every selected minimum would be at most $a$. This would put infinitely many distinct values into the [finite set](../../../../../../finite-set.md) $\{0,\ldots,a\}$, a contradiction. Hence

$$
\boxed{f:\mathbb N\longrightarrow A\text{ is a bijection}.}
$$

The [increasing enumeration of an infinite subset of natural numbers](../../../../../../increasing-enumeration-of-an-infinite-subset-of-natural-numbers.md) uses no arbitrary choice: each next element is the uniquely determined minimum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
