<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Writing $P_ng=n^{-1}\sum_{i=1}^ng(X_i)$ and $Pg=\mathbb Eg(X)$, the class $\mathcal G$ satisfies a [uniform law of large numbers](../../../../../../uniform-law-of-large-numbers.md) when

$$
\sup_{g\in\mathcal G}|P_ng-Pg|\longrightarrow0
$$

in probability; a strong ULLN uses almost-sure convergence.

Fix $\varepsilon>0$ and choose finitely many brackets $[g_j^L,g_j^U]$ of $L^1(P)$ width at most $\varepsilon$. The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md), simultaneously for their finitely many endpoints, gives

$$
\max_j\{|P_ng_j^L-Pg_j^L|,|P_ng_j^U-Pg_j^U|\}\to0.
$$

If $g_j^L\leq g\leq g_j^U$, bracketing both $P_ng$ and $Pg$ shows

$$
|P_ng-Pg|\leq\max\{|P_ng_j^L-Pg_j^L|,
|P_ng_j^U-Pg_j^U|\}+P(g_j^U-g_j^L).
$$

Taking the supremum gives a limit superior at most $\varepsilon$. Since $\varepsilon$ is arbitrary, the ULLN follows.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
