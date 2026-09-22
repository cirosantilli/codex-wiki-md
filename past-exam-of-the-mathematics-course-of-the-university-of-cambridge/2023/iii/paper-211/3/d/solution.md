<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Order the support as $K_1<\cdots<K_N$ and put

$$
s_i=\frac{g(K_i)-g(K_{i-1})}{K_i-K_{i-1}}.
$$

On the finite support,

$$
g(S_T)=g(K_1)+\sum_{i=2}^Ns_i
\{(S_T-K_{i-1})^+-(S_T-K_i)^+\}.
$$

This follows by telescoping: at $S_T=K_j$, only terms through $j$ survive and reconstruct successive increments of $g$. The [static replication on a finite terminal support](../../../../../../static-replication-on-a-finite-terminal-support.md) therefore has no-arbitrage price

$$
\boxed{\pi_t=g(K_1)P_t^T+
\sum_{i=2}^N
\frac{g(K_i)-g(K_{i-1})}{K_i-K_{i-1}}
(C_t^{T,K_{i-1}}-C_t^{T,K_i}).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
