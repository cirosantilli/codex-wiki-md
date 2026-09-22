<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose an [independent set](../../../../../../independent-set-graph-theory.md) uniformly and let $X_i$ indicate whether it contains vertex $i$. Then $H(X)=\log_2 i(G)$. Put $P_i=N(i)\cap[i-1]$ and $b_i=|P_i|$. Form a multiset containing every nonempty $P_i$ and $b_i$ copies of singleton $\{i\}$. Each coordinate $j$ occurs exactly $d_j$ times: in $d_j-b_j$ later-neighbor sets and in $b_j$ singleton copies.

For a set $A$ in this multiset, weight it by $1/\min_{j\in A}d_j$. These weights form a fractional cover, since each of the $d_j$ occurrences of $j$ has weight at least $1/d_j$. Apply the upper [Madiman-Tetali inequality](../../../../../../madiman-tetali-entropy-inequality.md). Since every $j\in P_i$ precedes $i$, one has $d_j\geq d_i$; enlarging that set's weight to $1/d_i$ and removing conditioning only enlarges its nonnegative contribution. For singleton terms retain the useful conditioning on $P_i$. Thus

$$
H(X)\leq\sum_i\frac1{d_i}\left[H(X_{P_i})+b_iH(X_i\mid X_{P_i})\right].
$$

For $b_i>0$, let $q_i=\mathbb P(X_{P_i}=0)$. Every nonzero neighbor assignment forces $X_i=0$, while the all-zero assignment allows at most two values. The [maximum entropy on a finite alphabet](../../../../../../maximum-entropy-on-a-finite-alphabet.md) gives

$$
H(X_{P_i})+b_iH(X_i\mid X_{P_i})\leq h_2(q_i)+(1-q_i)\log_2(2^{b_i}-1)+b_iq_i\leq\log_2(2^{b_i+1}-1).
$$

The last inequality is the binary entropy maximization formula, or the [log-sum inequality](../../../../../../log-sum-inequality.md), with group sizes $2^{b_i}$ and $2^{b_i}-1$. If $b_i=0$ the whole term is zero, also agreeing with the formula. Exponentiating proves the [degree-ordered independent-set entropy bound](../../../../../../degree-ordered-independent-set-entropy-bound.md)

$$
\boxed{i(G)\leq\prod_i(2^{b_i+1}-1)^{1/d_i}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
