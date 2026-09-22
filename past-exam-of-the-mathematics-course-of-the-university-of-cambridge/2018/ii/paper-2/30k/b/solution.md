<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V(p)$ be the maximal expected future reward minus search costs at posterior $p=(p_1,\ldots,p_n)$, with stopping value zero. Searching $i$ costs $c_i$, succeeds with probability $\alpha_ip_i$ and earns $R_i$, and otherwise produces the posterior $p^{(i)}$ displayed in part (a). The [rewarded Bayesian box search Bellman equation](../../../../../../rewarded-bayesian-box-search-bellman-equation.md) is

$$
\boxed{
V(p)=\max\left\{0,
\max_i\left[-c_i+\alpha_ip_iR_i
+(1-\alpha_ip_i)V(p^{(i)})\right]\right\}.}
$$

Suppose $\sum_i c_i/(\alpha_iR_i)<1$. At every posterior $p$, some index must satisfy

$$
p_i>\frac{c_i}{\alpha_iR_i};
$$

otherwise summing the reverse inequalities would give $1=\sum_i p_i<1$. For this box,

$$
-c_i+\alpha_ip_iR_i>0,
$$

even if one stops immediately after a failed search. Hence $V(p)>0$ at every posterior, and **stopping before discovery is never optimal**.

Once search necessarily continues until the ball is found, the expected reward $\sum_i p_iR_i$ is independent of the order of searches. Maximizing expected net reward therefore amounts to minimizing expected search cost. Part (a) applies, so **the policy maximizing $\alpha_iP_i^t/c_i$ remains optimal**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
