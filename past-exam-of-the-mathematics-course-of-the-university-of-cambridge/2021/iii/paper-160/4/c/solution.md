<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mu=C_p(\lambda)$, put $m=|\mu|$, and let the first-level $p$-quotient partitions have sizes $n_0,\ldots,n_{p-1}$. Then

$$
n=m+p\sum_jn_j.
$$

Repeated [subadditivity of the base-p digit sum](../../../../../../subadditivity-of-the-base-p-digit-sum.md) gives

$$
d_p(n)-d_p(m)
\leq d_p\left(\sum_jn_j\right)
\leq\sum_jd_p(n_j).
$$

For any partition $\nu$ of size $s$, iterating the core-quotient relation $s=|C_p(\nu)|+p|Q_p(\nu)|$ and the same digit-sum inequality gives

$$
d_p(s)\leq\sum_{r\geq0}|TC_p(\nu)_r|.
$$

Apply this to every first-level quotient partition. Their core towers concatenate to levels $r\geq1$ of $TC_p(\lambda)$, so

$$
d_p(n)-d_p(m)
\leq\sum_{r\geq1}|TC_p(\lambda)_r|.
$$

Part a applied to $\lambda$ and to its $p$-core $\mu$, whose higher core-tower levels are empty, now gives

$$
\begin{aligned}
(p-1)\left(v_p(\chi^\lambda(1))-v_p(\chi^\mu(1))\right)
&=\sum_{r\geq1}|TC_p(\lambda)_r|-d_p(n)+d_p(m)\\
&\geq0.
\end{aligned}
$$

Therefore the [Character-degree valuation does not increase on taking the p-core](../../../../../../character-degree-valuation-does-not-increase-on-taking-the-p-core.md):

$$
\boxed{v_p(\chi^\lambda(1))\geq v_p(\chi^{C_p(\lambda)}(1))}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 160](../../../paper-160-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
