<h1 id="20h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $T_j=\inf\{n\geq1:X_n=j\}$. By the [Strong Markov property](../../../../../../strong-markov-property.md), the probability of hitting $j$ and subsequently returning to $i$ is $f_{ij}f_{ji}$. This event implies a return to $i$, so **$f_{ii}\geq f_{ij}f_{ji}$**. For $i=j$, interpret the event as two successive returns.

Set $T_i^{(0)}=0$ and let $T_i^{(r)}$ be the $r$th successive return. Repeated use of the [Strong Markov property](../../../../../../strong-markov-property.md) gives $\mathbb P_i(T_i^{(r)}<\infty)=f_{ii}^r$. The total number $N_i$ of visits, including time zero, is both $\sum_{n\geq0}\mathbf1_{\{X_n=i\}}$ and $\sum_{r\geq0}\mathbf1_{\{T_i^{(r)}<\infty\}}$. By [Tonelli theorem](../../../../../../tonelli-theorem.md),

$$
\boxed{\sum_{n=0}^\infty\mathbb P_i(X_n=i)=\mathbb E_iN_i=\sum_{r=0}^\infty f_{ii}^r.}
$$

The identity is valid with value $+\infty$. In particular, divergence of the return-probability sum is equivalent to [Markov-chain recurrence](../../../../../../recurrent-markov-chain.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
