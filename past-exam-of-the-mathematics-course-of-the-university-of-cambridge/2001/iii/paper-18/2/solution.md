<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [well-quasi-ordering](../../../../../well-quasi-ordering.md) rules out bad infinite [sequences](../../../../../sequence.md): every sequence has $i<j$ with $x_i\le x_j$. It behaves well under finite products and finite [words](../../../../../string.md), but infinitary constructions expose a limitation. [Better-quasi-ordering](../../../../../better-quasi-ordering.md), introduced by Nash-Williams, strengthens the sequence test to a test on families of finite initial segments, and thereby provides a robust theory of infinitary closure.

For an infinite $A\subseteq\mathbb N$, a [barrier in better-quasi-order theory](../../../../../barrier-in-better-quasi-order-theory.md) is a family $B$ of nonempty finite increasing sequences from $A$ such that every infinite subset of $A$ has a member of $B$ as an initial segment, and no distinct members of $B$ are included in one another. The initial segment is unique. Write $s\triangleleft t$ when some increasing sequence $u$ has $s$ as an initial segment and $t$ as an initial segment after the least member of $u$ is deleted. For instance, in $[A]^2$ this means $(a,b)\triangleleft(b,c)$ with $a<b<c$.

A map $f:B\to Q$ is good if some $s\triangleleft t$ satisfies $f(s)\le_Q f(t)$. A [preorder](../../../../../preorder.md) $Q$ is a [better-quasi-ordering](../../../../../better-quasi-ordering.md) when every such barrier map is good. Singleton barriers recover ordinary infinite [sequences](../../../../../sequence.md), so

$$
\boxed{\mathrm{BQO}\ \Longrightarrow\ \mathrm{WQO}.}
$$

Equivalently, take a [continuous array in better-quasi-order theory](../../../../../continuous-array-in-better-quasi-order-theory.md) $F:[A]^\omega\to Q$, where infinite subsets have their usual product topology and $Q$ is discrete. Put $X^-=X\setminus\{\min X\}$. Better-quasi-ordering excludes arrays with $F(X)\not\le F(X^-)$ for every $X$. A barrier map gives a locally constant array by reading the unique initial segment; the converse uses refinement of the front of finite segments on which a continuous map becomes constant. This viewpoint makes the shift, rather than mere inclusion of subsets, central.

The implication is strict. The [Rado order](../../../../../rado-order.md) consists of pairs $(m,n)$ with $m<n$, ordered by

$$
(m,n)\le_R(k,l)\quad\Longleftrightarrow\quad[m=k\text{ and }n\le l]\text{ or }[n<k].
$$

It is a [well-quasi-ordering](../../../../../well-quasi-ordering.md). In any infinite sequence, either the first coordinates are unbounded, giving a later first coordinate above the earlier second coordinate, or one first coordinate occurs infinitely often and its second coordinates have a nondecreasing pair. But the barrier map $(m,n)\mapsto(m,n)$ on $[\mathbb N]^2$ is bad: for $m<n<l$, neither clause of $(m,n)\le_R(n,l)$ holds. Thus **the Rado order is WQO but not BQO**.

The same example explains why strengthening the definition is useful. Order subsets by the [Hoare domination preorder](../../../../../hoare-domination-preorder.md), $P\le_H Q$ when every member of $P$ is below some member of $Q$. The infinite rows $R_m=\{(m,n):n>m\}$ form an [antichain](../../../../../antichain.md). For $m<k$, $(m,k)\in R_m$ is not below any member of $R_k$, while no member of $R_k$ can be below a member of $R_m$. Thus the full [power set](../../../../../power-set.md) of a [well-quasi-ordering](../../../../../well-quasi-ordering.md) need not be a [well-quasi-ordering](../../../../../well-quasi-ordering.md).

In contrast, [power-set closure of better-quasi-orderings](../../../../../power-set-closure-of-better-quasi-orderings.md) has a short array proof. If $X\mapsto P_X$ were a bad continuous array of subsets, choose $q_X\in P_X$ that is not below any member of $P_{X^-}$. Make this choice by a fixed choice rule depending only on the two subsets. They are locally constant, so $X\mapsto q_X$ is continuous. Since $q_{X^-}\in P_{X^-}$, it is a bad array into the original [better-quasi-ordering](../../../../../better-quasi-ordering.md), a contradiction. Empty subsets cannot be the source of a bad comparison. Thus the full [power set](../../../../../power-set.md), not just its finite subsets, preserves better-quasi-ordering under domination.

Further examples and closure principles show the scope of the theory. Every [well-order](../../../../../well-order.md) is a [better-quasi-ordering](../../../../../better-quasi-ordering.md): a bad array would give a strictly descending ordinal sequence by successively deleting the least member of one infinite set. Every finite equality order is a [better-quasi-ordering](../../../../../better-quasi-ordering.md) by the [Nash-Williams barrier partition theorem](../../../../../nash-williams-barrier-partition-theorem.md), which makes a finite coloring of a barrier constant on an infinite restriction. The same theorem proves closure under finite products: color a bad product array by the first coordinate in which the shifted comparison fails, and pass to a homogeneous infinite restriction to obtain a bad coordinate array. Finite disjoint unions work by first homogenizing the component.

Nash-Williams' extension to countable transfinite [sequences](../../../../../sequence.md) says that sequences of labels from a [better-quasi-ordering](../../../../../better-quasi-ordering.md), of arbitrary countable ordinal length, are again better-quasi-ordered by increasing label-monotone embeddings. It is an infinitary counterpart of [Higman's lemma](../../../../../higman-s-lemma.md). Its formulation and logical strength are studied in [https://arxiv.org/abs/math/9408204](https://arxiv.org/abs/math/9408204) . The point is not that every closure proof becomes elementary, but that barriers and continuous arrays supply the stable induction and partition framework absent from ordinary sequence tests. The modern account [https://arxiv.org/pdf/1604.05866](https://arxiv.org/pdf/1604.05866) develops this framework and the barrier partition theorem.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
