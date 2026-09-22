<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $w_i=(Aq)_i$. For each row put $S_i=\{j:a_{ij}>0\}$; the positive row entries $\alpha_i=(a_{ij})_{j\in S_i}$ form a [probability distribution](../../../../probability-distribution-split.md) because the row [sum](../../../../sum.md) is one. When $w_i>0$, define the [probability distribution](../../../../probability-distribution-split.md)

$$
r_i(j)=\frac{a_{ij}q_j}{w_i}\qquad(j\in S_i).
$$

Part (a), applied on this row [support](../../../../support.md), gives $d(r_i,\alpha_i)\geq0$. Its weighted [sum](../../../../sum.md) expands as

$$
\begin{aligned}
\sum_{i:w_i>0}w_i d(r_i,\alpha_i)
&=\sum_{i,j}a_{ij}q_j\log_2\frac{q_j}{w_i}\\
&=\sum_jq_j\log_2q_j\sum_i a_{ij}-\sum_iw_i\log_2w_i\\
&=H(w)-H(q).
\end{aligned}
$$

Rows with $w_i=0$ contribute zero, since all $a_{ij}q_j$ in such a row vanish. Using the convention that zero-weight logarithmic terms are zero, the result is

$$
\boxed{H(W)-H(V)=\sum_{i:w_i>0}w_i d(r_i,\alpha_i)\geq0.}
$$

Both stochasticity conditions have a role: row sums normalize the comparison distributions, while column sums preserve the total contribution from $q$.

This is [entropy increase under doubly stochastic mixing](../../../../entropy-increase-under-doubly-stochastic-mixing.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
