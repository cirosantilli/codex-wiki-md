<h1 id="a/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [C-embedded subset](../../../../../c-embedded-subset.md) $Y\subseteq X$ is one when every [continuous](../../../../../continuous-function.md) [real-valued function](../../../../../real-valued-function.md) on $Y$ extends continuously to $X$. It is a [Cb-embedded subset](../../../../../cb-embedded-subset.md) when this is required for every bounded [continuous](../../../../../continuous-function.md) [real-valued function](../../../../../real-valued-function.md), with a bounded extension. These definitions concern the [subspace topology](../../../../../subspace-topology.md) on $Y$.

Here is the bounded Tietze extension construction from [Urysohn's lemma](../../../../../urysohn-s-lemma.md). Let $g:Y\to\mathbb R$ be [continuous](../../../../../continuous-function.md) with $|g|\le M$. The case $M=0$ has the zero extension. For $M>0$, the [sets](../../../../../set-split.md) $A=\{g\le-M/3\}$ and $B=\{g\ge M/3\}$ are disjoint and closed in $X$, since $Y$ is closed. [Urysohn's lemma](../../../../../urysohn-s-lemma.md) gives a [continuous](../../../../../continuous-function.md) $u_0:X\to[-M/3,M/3]$ taking the endpoint values on $A,B$. On $Y$,

$$
|g-u_0|\le2M/3.
$$

Indeed on $A$ or $B$ this follows from the prescribed endpoint; on their complement both $|g|$ and $|u_0|$ are at most $M/3$.

Repeat on the residual. With $M_n=M(2/3)^n$, choose [continuous](../../../../../continuous-function.md) $u_n$ satisfying $\|u_n\|_\infty\le M_n/3$ and reducing the residual on $Y$ to at most $M_{n+1}$. The [series](../../../../../series-mathematics.md) $F=\sum_{n\ge0}u_n$ converges uniformly by the geometric majorant. Its sum is [continuous](../../../../../continuous-function.md), has $|F|\le\sum M_n/3=M$, and restricts to $g$, since the residual tends uniformly to zero. Thus **every bounded [continuous function](../../../../../continuous-function.md) extends, with its bound preserved**, proving $C^b$-embeddedness without assuming the extension theorem being proved.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
