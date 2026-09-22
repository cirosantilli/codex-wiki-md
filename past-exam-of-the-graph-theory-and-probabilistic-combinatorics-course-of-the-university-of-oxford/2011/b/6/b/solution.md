<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Explore the family [tree](../../../../../tree-graph-theory-split.md) one individual at a time, maintaining a [queue](../../../../../queue-queueing-theory.md) of individuals not yet explored. Initially its size is $Y_0=1$. Exploring individual $t$ removes it and adds its [independent](../../../../../independent-random-variables.md) offspring $Z_t$, so before the [queue](../../../../../queue-queueing-theory.md) empties,

$$
Y_t=1+\sum_{j=1}^t(Z_j-1).
$$

One may define the [independent increments](../../../../../independent-increments.md) indefinitely, but the [tree](../../../../../tree-graph-theory-split.md) exploration stops at $T=\inf\{t:Y_t=0\}$. This [hitting time](../../../../../first-passage-time.md) is the [total progeny](../../../../../total-progeny-of-a-branching-process.md), including the ancestor. Since each increment is at least $-1$, a [queue](../../../../../queue-queueing-theory.md) cannot jump below zero before hitting zero. If it never hits zero, the family has infinitely many individuals.

Suppose $kp<1$. A [Chernoff bound](../../../../../chernoff-bound.md) in moment-generating-function form says that for [independent](../../../../../independent-random-variables.md) $W_j$ and $\theta>0$,

$$
\mathbb P\left(\sum_{j=1}^nW_j\geq0\right)\leq\prod_{j=1}^n\mathbb E e^{\theta W_j}.
$$

Here take $W_j=Z_j-1$, with

$$
M(\theta)=\mathbb E e^{\theta(Z-1)}=e^{-\theta}(1-p+pe^\theta)^k.
$$

We have $M(0)=1$ and $M'(0)=kp-1<0$, so some $\theta>0$ has $M(\theta)<1$. Let $c=-\log M(\theta)>0$. If $T>n$, the [queue](../../../../../queue-queueing-theory.md) is still positive after $n$ explorations; its [integer](../../../../../integer-split.md) value is at least one, giving $\sum_{j=1}^n(Z_j-1)\geq0$. Therefore

$$
\boxed{\mathbb P(T>n)\leq M(\theta)^n=e^{-cn},\qquad n\geq1.}
$$

This proves the claimed bound without appealing to a general branching-process tail theorem.

The argument proves the more general [exponential total progeny tail for bounded subcritical offspring](../../../../../exponential-total-progeny-tail-for-bounded-subcritical-offspring.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
