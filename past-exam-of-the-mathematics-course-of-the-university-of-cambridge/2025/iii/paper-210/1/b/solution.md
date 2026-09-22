<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Glivenko-Cantelli theorem](../../../../../../glivenko-cantelli-theorem.md) states that for the empirical distribution function $F_n$ of iid real observations with distribution function $F$,

$$
\sup_{t\in\mathbb R}|F_n(t)-F(t)|\longrightarrow0
$$

almost surely.

Apply part (a) to $\mathcal G=\{\mathbf1_{(-\infty,t]}:t\in\mathbb R\}$. For each $\varepsilon>0$, choose finitely many quantile cutpoints so that the $P$-mass between consecutive cutpoints is at most $\varepsilon$, treating atoms as cutpoints themselves. Indicators at adjacent cutpoints give finite $L^1(P)$ brackets of width at most $\varepsilon$. Using the strong law for the finite bracket endpoints and then intersecting the probability-one events for $\varepsilon=1/m$ gives the almost-sure conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
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
