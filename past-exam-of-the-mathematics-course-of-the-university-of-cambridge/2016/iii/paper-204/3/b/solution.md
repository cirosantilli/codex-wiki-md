<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A_n$ be the event that the origin has an open [graph path](../../../../../../path-in-a-graph.md) to the boundary of $[-n,n]^d\cap\mathbb Z^d$. The [graph path](../../../../../../path-in-a-graph.md) can be stopped on its first boundary visit, so $A_n$ depends on only finitely many sites. Its [probability](../../../../../../probability.md) $f_n(p)=\mathbb P_p(A_n)$ is a finite sum of terms $p^a(1-p)^b$, and is therefore a [continuous function](../../../../../../continuous-function.md) of $p$. Also $A_{n+1}\subseteq A_n$, and the [König infinity lemma](../../../../../../konig-s-lemma.md) gives $\bigcap_n A_n=\{0\leftrightarrow\infty\}$. By [continuity from above of a measure](../../../../../../continuity-from-above-of-a-measure.md),

$$
\theta(p)=\inf_{n\geq1}f_n(p).
$$

The [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md) described below shows that $\theta$ is nondecreasing. For $p<1$, its right [limit of a function](../../../../../../limit-of-a-function.md) $\theta(p+)$ exists and is at least $\theta(p)$. For every fixed $n$,

$$
\theta(p+)\leq\lim_{r\downarrow p}f_n(r)=f_n(p).
$$

Taking the infimum in $n$ proves **$\theta(p+)=\theta(p)$**. This proves [right continuity of percolation probability](../../../../../../right-continuity-of-percolation-probability.md) throughout $[0,1)$; at $1$ right continuity is understood relative to the parameter domain. The argument does not interchange two uncontrolled limits.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
