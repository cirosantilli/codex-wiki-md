<h1 id="26i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Only arrivals at times $u\leq t$ remain after the window closes. Such an arrival survives until $t+v$ exactly when its service time exceeds $t+v-u$. The same [independent](../../../../../../independent-random-variables.md) Poisson thinning gives

$$
\boxed{X(t+v)\sim\operatorname{Poisson}\left(\lambda\int_v^{t+v}\mathbb P(S>s)\,ds\right).}
$$

At $v=0$ this agrees with part (b), while for large $v$ the parameter tends to zero.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [26I](../../26i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
