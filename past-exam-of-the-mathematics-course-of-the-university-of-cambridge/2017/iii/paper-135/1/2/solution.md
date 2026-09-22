<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\mathcal T(D)$ for the [recursively repetition-free labelled trees](../../../../../../recursively-repetition-free-labelled-tree.md). Each [rooted tree](../../../../../../rooted-tree.md) is finite because the inductive definition forms it from an already constructed finite list of finite child [rooted trees](../../../../../../rooted-tree.md). Its label list is obtained by visiting the root first, then each child subtree in its prescribed order, using a [depth-first traversal of a tree](../../../../../../depth-first-traversal-of-a-tree.md). This list can have repetitions. In particular, different branches may use the same label; the children are required to be distinct [rooted trees](../../../../../../rooted-tree.md), not to have distinct root labels.

For any finite label pool $F$, prove by [mathematical induction](../../../../../../mathematical-induction.md) on $|F|$ that $\mathcal T(F)$ is finite. For $F=\varnothing$ it is empty. For each root $d\in F$, the children form a [finite repetition-free sequence](../../../../../../finite-repetition-free-sequence.md) from $\mathcal T(F\setminus\{d\})$, which is finite by [mathematical induction](../../../../../../mathematical-induction.md). There are therefore finitely many child lists for that root, and the finite union over $d\in F$ is finite. More explicitly, if $t_m$ is the number of [rooted trees](../../../../../../rooted-tree.md) on a pool of $m$ labels, then

$$
t_0=0,\qquad t_m=m\sum_{k=0}^{t_{m-1}}\frac{t_{m-1}!}{(t_{m-1}-k)!}.
$$

There is no countable choice in this finite [mathematical induction](../../../../../../mathematical-induction.md).

Now suppose $T_0,T_1,\ldots$ were an injective enumeration of a countably infinite subset of $\mathcal T(D)$. Their canonical traversal lists give an explicit enumeration of all labels used. If infinitely many different labels occur, the least-first-occurrence procedure gives a countably infinite subset of $D$, a contradiction. Otherwise all labels belong to one [finite set](../../../../../../finite-set.md) $F$. Every $T_n$ then belongs to $\mathcal T(F)$: recursively its root lies in $F$ and its child [rooted trees](../../../../../../rooted-tree.md) use only $F$ with that root removed. But $\mathcal T(F)$ is finite by the preceding [mathematical induction](../../../../../../mathematical-induction.md), again a contradiction. Finally $d\mapsto$ the single-vertex [rooted tree](../../../../../../rooted-tree.md) labelled $d$ is injective, so $\mathcal T(D)$ is infinite. Hence [recursively repetition-free labelled trees preserve Dedekind-finiteness](../../../../../../recursively-repetition-free-labelled-trees-preserve-dedekind-finiteness.md):

$$
\boxed{\mathcal T(D)\text{ is an infinite Dedekind-finite set.}}
$$

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 135](../../../paper-135-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
