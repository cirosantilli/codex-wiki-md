<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**False as printed: separativity alone does not guarantee a new generic filter.** A [separative forcing order](../../../../../../separative-forcing-order.md) means that if $p\not\leq q$, some $r\leq p$ is incompatible with $q$. The one-point order $\mathbb P=\{p\}$ is separative vacuously. Its only [generic filter](../../../../../../generic-filter.md) is $\{p\}=\mathbb P$, and this belongs to $M$. Thus no $G\notin M$ exists in this example.

The natural missing hypothesis is that the nonempty order is an [atomless forcing order](../../../../../../atomless-forcing-order.md). Under that hypothesis the intended argument works. Since $M$ is a [countable transitive model](../../../../../../countable-transitive-model.md), enumerate externally its dense subsets as $D_0,D_1,\ldots$. Choose $p_{n+1}\leq p_n$ with $p_{n+1}\in D_n$. Then

$$
G=\{q\in\mathbb P:\exists n\ p_n\leq q\}
$$

is a directed upward-closed [filter in an ordered set](../../../../../../filter-mathematics.md) and meets every $D_n$. This is the [Rasiowa–Sikorski lemma](../../../../../../rasiowa-sikorski-lemma.md), giving a [generic filter](../../../../../../generic-filter.md) over $M$.

If $G\in M$, the [set difference](../../../../../../set-difference.md) $D=\mathbb P\setminus G$ would belong to $M$. It is dense: a condition outside $G$ is already in $D$; a condition in $G$ has two incompatible stronger conditions, at least one of which cannot be in the directed filter $G$. Genericity would require $G\cap D\ne\varnothing$, a contradiction. Thus

$$
\boxed{\text{with atomlessness, a generic }G\text{ exists and }G\notin M.}
$$

This uses [generic filter for an atomless order is new](../../../../../../generic-filter-for-an-atomless-order-is-new.md). A [forcing atom](../../../../../../forcing-atom.md) is precisely the obstruction illustrated by the counterexample; separativity does not remove it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
