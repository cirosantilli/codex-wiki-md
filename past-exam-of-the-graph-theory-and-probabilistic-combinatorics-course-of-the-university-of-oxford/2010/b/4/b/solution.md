<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an indicator $I_i$, $\operatorname{Var}(I_i)=P(A_i)(1-P(A_i))\leq P(A_i)$. Covariances vanish for independent pairs. For dependent distinct pairs,

$$
\operatorname{Cov}(I_i,I_j)=P(A_i\cap A_j)-P(A_i)P(A_j)
\leq P(A_i\cap A_j).
$$

Expanding the [variance](../../../../../variance-split.md), with ordered pairs as in the definition of $\Delta$, gives

$$
\boxed{\operatorname{Var}(X)=\sum_i\operatorname{Var}(I_i)+
\sum_i\sum_{j\sim i}\operatorname{Cov}(I_i,I_j)
\leq\mathbb EX+\Delta.}
$$

For sufficiently large $n$, $\mu_n>0$. By [Chebyshev inequality](../../../../../chebyshev-s-inequality.md),

$$
P(X_n=0)\leq P(|X_n-\mu_n|\geq\mu_n)
\leq\frac{\operatorname{Var}(X_n)}{\mu_n^2}
\leq\frac1{\mu_n}+\frac{\Delta_n}{\mu_n^2}\longrightarrow0.
$$

This is the [second moment method](../../../../../second-moment-method.md): a vanishing relative [variance](../../../../../variance-split.md) makes a zero count unlikely.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
