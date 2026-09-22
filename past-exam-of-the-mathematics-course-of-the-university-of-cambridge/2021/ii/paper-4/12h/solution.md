<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Multiplying the matrices inductively gives columns $(p_n,q_n)^T$ and $(p_{n-1},q_{n-1})^T$. Their determinant is $(-1)^{n-1}$, and writing $x=(p_nx_{n+1}+p_{n-1})/(q_nx_{n+1}+q_{n-1})$ gives

$$
|x-p_n/q_n|={1\over q_n(q_nx_{n+1}+q_{n-1})}\leq{1\over q_nq_{n+1}}.
$$

If $Ay^2+By+C=0$, then for rationals $p/q$ near $y$, factorization against the conjugate root gives $|p/q-y|\geq M/q^2$; rationals away from $y$ are handled by reducing $M$. Finally $q_{n+1}\geq a_{n+1}q_n$, so the upper bound is at most $1/(a_{n+1}q_n^2)$. Unbounded partial quotients contradict the fixed lower bound for a quadratic irrational.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
