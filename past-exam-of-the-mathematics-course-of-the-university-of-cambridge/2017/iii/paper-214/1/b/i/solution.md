<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $q_k(n)=\mathbb P_p((0,0)\leftrightarrow(n,0)\text{ inside }T_k)$, with $q_k(0)=1$. The connection event is increasing in the open [edges](../../../../../../../edge-of-a-graph.md). Apply the [Harris-FKG inequality](../../../../../../../harris-fkg-inequality.md) to connection from $(0,0)$ to $(n,0)$ and connection from $(n,0)$ to $(n+m,0)$, both constrained to the strip. Their intersection implies connection between the outer endpoints, while horizontal translation invariance makes the second event's [probability](../../../../../../../probability.md) $q_k(m)$. Hence

$$
q_k(n+m)\geq q_k(n)q_k(m).
$$

These events may depend on infinitely many strip [edges](../../../../../../../edge-of-a-graph.md). To justify the inequality directly, first restrict each connecting [graph path](../../../../../../../path-in-a-graph.md) to a finite box, apply [Harris-FKG inequality](../../../../../../../harris-fkg-inequality.md) in the finite independent [edge](../../../../../../../edge-of-a-graph.md) family, and then let the box grow. Every connection has a finite witness [graph path](../../../../../../../path-in-a-graph.md), so continuity from below gives the stated inequality.

The direct horizontal [graph path](../../../../../../../path-in-a-graph.md) supplies $q_k(n)\geq p^n>0$, and [probabilities](../../../../../../../probability.md) are at most one. Thus $a_k(n)=-\log q_k(n)$ is a finite nonnegative [subadditive sequence](../../../../../../../subadditive-sequence.md) with $a_k(n)\leq-n\log p$. The [Fekete lemma](../../../../../../../fekete-s-lemma.md) now gives a finite [connection decay rate in a percolation strip](../../../../../../../connection-decay-rate-in-a-percolation-strip.md):

$$
\boxed{f_k(p)=\lim_{n\to\infty}\frac{a_k(n)}n=\inf_{n\geq1}\frac{a_k(n)}n,\qquad0\leq f_k(p)\leq-\log p.}
$$

Each individual ratio is at least its [infimum](../../../../../../../infimum.md), so $-\log q_k(n)\geq nf_k(p)$ and therefore

$$
\boxed{q_k(n)\leq e^{-nf_k(p)}.}
$$

At $n=0$ this reads $1\leq1$. Only nonnegative separations are intended by this notation; horizontal reflection supplies the analogous bound with $|n|$ for negative separations.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
