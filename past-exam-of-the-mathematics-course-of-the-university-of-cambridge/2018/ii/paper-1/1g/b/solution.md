<h1 id="1g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose distinct [primes](../../../../../../prime-number.md) $p_1,\ldots,p_{1000}$. The moduli $p_k^2$ are pairwise [coprime](../../../../../../coprime-integers.md), so the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) supplies an integer $N$ satisfying

$$
N\equiv p_k-k\pmod {p_k^2}
\qquad(1\leq k\leq1000).
$$

Consequently

$$
N+k\equiv p_k\pmod {p_k^2},
$$

so $p_k\mid N+k$ but $p_k^2\nmid N+k$. By the definition of a [squarefull number](../../../../../../powerful-number.md), $N+k$ is therefore not squarefull. Adding a sufficiently large multiple of $\prod_kp_k^2$ makes $N$ positive without changing any congruence. **The integers $N+1,\ldots,N+1000$ are the required consecutive integers.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1G](../../1g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
