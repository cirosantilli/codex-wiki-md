<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

A [probability space](../../../../../probability-space.md) consists of a sample space $\Omega$, a [sigma-algebra](../../../../../sigma-algebra.md) $\mathcal F$ of events, and a [probability measure](../../../../../probability-measure.md) $\mathbb P$ satisfying:

- $\mathbb P(A)\geq0$ for every $A\in\mathcal F$.
- $\mathbb P(\Omega)=1$.
- For pairwise disjoint events, $\mathbb P(\bigcup_{j\ge1}A_j)=\sum_{j\ge1}\mathbb P(A_j)$.

For arbitrary events, **[Boole's inequality](../../../../../boole-s-inequality.md) is $\mathbb P(\bigcup_jA_j)\leq\sum_j\mathbb P(A_j)$**. To prove it, replace each $A_j$ by $D_j=A_j\setminus\bigcup_{i<j}A_i$. The $D_j$ are disjoint, have the same union, and satisfy $D_j\subseteq A_j$. Countable additivity and monotonicity give $\mathbb P(\bigcup_jA_j)=\sum_j\mathbb P(D_j)\leq\sum_j\mathbb P(A_j)$. Finite unions are included by taking subsequent events empty.

Let $H_i$ be the $i$th heads event. For every $m$, the event of infinitely many heads lies inside $\bigcup_{i\ge m}H_i$. By the [union bound](../../../../../boole-s-inequality.md), its probability is at most $\sum_{i\ge m}p_i$, which tends to zero. Thus **the probability of infinitely many heads is $0$**. This is the [First Borel-Cantelli lemma](../../../../../borel-cantelli-first-lemma.md), and requires no [independence](../../../../../independent-random-variables.md) of the coin tosses.

For the dice experiment there are $4$ ordered outcomes giving a sum of $5$ and $6$ giving $7$, out of $36$. Each trial therefore has $p_5=1/9$, $p_7=1/6$ and irrelevant-outcome probability $13/18$. By [independence](../../../../../independent-random-variables.md) between trials, summing over the number of initial irrelevant outcomes gives

$$
\boxed{\mathbb P(5\text{ before }7)=\sum_{k\ge0}\left(\frac{13}{18}\right)^k\frac19=\frac{p_5}{p_5+p_7}=\frac25.}
$$

The geometric series also shows that one of the two relevant sums eventually appears almost surely. Equivalently, [first-step analysis](../../../../../first-step-analysis.md) gives $p=p_5+(13/18)p$.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
