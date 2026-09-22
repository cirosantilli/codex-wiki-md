<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $C=R/(1-k)$. The hypothesis scales to every residual $r\in F$: if $r\ne0$, apply it to $r/\|r\|$ and multiply the resulting vector by $\|r\|$ to obtain an approximate preimage of [norm](../../../../../norm.md) at most $R\|r\|$ with error at most $k\|r\|$. For $r=0$, choose zero.

Start with $r_0=y$. Inductively choose $u_j\in E$ so that

$$
\|u_j\|\leq R\|r_{j-1}\|,\qquad r_j=r_{j-1}-Tu_j,\qquad \|r_j\|\leq k\|r_{j-1}\|.
$$

Then $\|r_j\|\leq k^j\|y\|$ and $\sum_j\|u_j\|\leq R\|y\|/(1-k)$. [Completeness](../../../../../completeness.md) of the [Banach space](../../../../../banach-space-split.md) $E$ gives $x=\sum_j u_j$. Boundedness of $T$ gives

$$
\|Tx-y\|\leq\|T\|\left\|x-\sum_{j=1}^n u_j\right\|+\|r_n\|\longrightarrow0.
$$

Thus

$$
\boxed{Tx=y,\qquad \|x\|\leq\frac{R}{1-k}\|y\|}.
$$

This [geometric correction for approximate surjectivity](../../../../../geometric-correction-for-approximate-surjectivity.md) uses no [completeness](../../../../../completeness.md) assumption on $F$: every infinite sum was formed in $E$.

To establish the [completeness forced by uniformly bounded lifting](../../../../../completeness-forced-by-uniformly-bounded-lifting.md), let $(y_n)$ be a [Cauchy sequence](../../../../../cauchy-sequence.md) in $F$. Choose a subsequence $(y_{n_j})$ with $\|y_{n_{j+1}}-y_{n_j}\|\leq2^{-j}$. Lift $y_{n_1}$ to $v_0\in E$ and each difference to $v_j\in E$ with $Tv_j=y_{n_{j+1}}-y_{n_j}$ and $\|v_j\|\leq C2^{-j}$. The series $v_0+\sum_jv_j$ converges in $E$, and its image under $T$ is the limit of the subsequence. The original [Cauchy sequence](../../../../../cauchy-sequence.md) has that same limit, by the triangle inequality. Hence **$F$ is complete**.

The [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md) states that a bounded surjective [linear map](../../../../../linear-map.md) between [Banach spaces](../../../../../banach-space-split.md) is open. In particular, a bounded linear bijection has a bounded inverse. This is the theorem the question permits us to state without proof.

For the [closed graph theorem](../../../../../closed-graph-theorem.md), suppose $T:E\to F$ is everywhere-defined and linear with closed graph $G(T)$. The product [norm](../../../../../norm.md) $\|(x,y)\|=\|x\|+\|y\|$ makes $E\times F$ a [Banach space](../../../../../banach-space-split.md), so its closed subspace $G(T)$ is complete. Projection $\pi:G(T)\to E$, $(x,Tx)\mapsto x$, is a bounded linear bijection. Its inverse is bounded by the [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md); therefore

$$
\|x\|+\|Tx\|=\|\pi^{-1}x\|\leq C_1\|x\|.
$$

It follows that $T$ is bounded, proving the [closed graph theorem](../../../../../closed-graph-theorem.md) rather than assuming it.

For the final clause, $S$ is the [separating space of a linear map](../../../../../separating-space-of-a-linear-map.md). It contains zero, and if $x_n\to0$, $Tx_n\to y$ and $z_n\to0$, $Tz_n\to w$, then $\alpha x_n+\beta z_n\to0$ and its image tends to $\alpha y+\beta w$. Thus $S$ is a [vector subspace](../../../../../vector-subspace.md). If $y_j\in S$ and $y_j\to y$, choose one vector $w_j$ from a witnessing sequence for $y_j$ with

$$
\|w_j\|<1/j,\qquad \|Tw_j-y_j\|<1/j.
$$

Then $w_j\to0$ and $Tw_j\to y$, so $y\in S$: it is closed. If $T$ is continuous, every defining image limit is zero, hence $S=\{0\}$. Conversely, if $S=\{0\}$ and $x_n\to x$, $Tx_n\to y$, then $x_n-x\to0$ and $T(x_n-x)\to y-Tx\in S$, so $y=Tx$. The graph is sequentially closed and therefore closed in the normed, metrizable product. The proved [closed graph theorem](../../../../../closed-graph-theorem.md) now gives continuity. Consequently

$$
\boxed{S\text{ is a closed linear subspace of }F,\qquad T\text{ is continuous}\iff S=\{0\}}.
$$

The original PDF places $S$ in $F$; the TeX's first reference to a subset of $E$ is a transcription error.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
