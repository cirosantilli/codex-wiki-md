<h1 id="14g/solution">Solution</h1>

↑ **Parent:** [14G](../14g.md)

The [complete metric space](../../../../../complete-metric-space.md) $\mathbb R$ supplies a counterexample: $A_n=[n,\infty)$ are descending nonempty [closed sets](../../../../../closed-set.md), but no real number belongs to them all.

Now assume shrinking [diameters](../../../../../diameter.md). Choose $x_n\in A_n$. Given $\varepsilon>0$, choose $N$ so that $\operatorname{diam}(A_N)<\varepsilon$. Whenever $m,n\geq N$, both chosen points lie in $A_N$, so $d(x_m,x_n)<\varepsilon$. Thus $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md). By [completeness](../../../../../completeness.md) it converges to some $x\in X$. For each fixed $N$, the tail lies in the [closed set](../../../../../closed-set.md) $A_N$, so its limit lies there too. Hence $x\in\bigcap_nA_n$. Any two points of this intersection have distance at most every $\operatorname{diam}(A_n)$, so their distance is zero. **The shrinking intersection contains exactly one point.** This is the [Cantor intersection theorem](../../../../../cantor-s-intersection-theorem.md).

For the dense-open conclusion, begin inside an arbitrary nonempty [open set](../../../../../open-set.md) $O\subseteq X$; taking $O=X$ gives the requested existence. Since $U_1$ is a [dense subset](../../../../../dense-set.md), choose $x_1\in O\cap U_1$ and $0<r_1\leq1/2$ small enough that the [closed ball](../../../../../closed-ball.md) $A_1=\overline B(x_1,r_1)$ is contained in $O\cap U_1$. Here $\overline B$ denotes the closed ball, not an assumption about the closure of the open ball.

Inductively, the open ball $B(x_n,r_n)$ meets the dense [open set](../../../../../open-set.md) $U_{n+1}$. Choose $x_{n+1}$ in that intersection and a positive radius $r_{n+1}\leq2^{-(n+1)}$ so small that

$$
\overline B(x_{n+1},r_{n+1})\subseteq B(x_n,r_n)\cap U_{n+1}.
$$

Such a radius exists by openness and the [triangle inequality](../../../../../triangle-inequality.md). These nonempty [closed sets](../../../../../closed-set.md) descend and have [diameters](../../../../../diameter.md) at most $2r_n\to0$. The preceding result gives a point in every $A_n$, hence in $O$ and every $U_n$. Therefore **$\bigcap_nU_n$ is nonempty; in fact it is dense in $X$**. This proves the relevant [Baire category theorem](../../../../../baire-category-theorem.md) directly, without assuming closed balls are compact.

## ↑ Ancestors (10)

1. [14G](../14g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
