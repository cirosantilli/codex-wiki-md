<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The open descendants of any vertex form a [Galton-Watson process](../../../../../../galton-watson-process.md) with offspring distribution $\operatorname{Bin}(k,p)$. If $kp\leq1$, it dies out almost surely, so $N_\infty=0$.

If $kp>1$, let $\theta>0$ be its survival probability. At level $n$, each vertex begins an independent descendant subtree; the event that its edge to its parent is closed while its descendant open cluster is infinite has probability $(1-p)\theta>0$. Thus the number of such vertices at level $n$ is binomial with $k^n$ trials and a fixed positive success probability. For every fixed $M$, the probability of at least $M$ successes tends to one. Their infinite clusters are separated by their closed parent edges, so $\mathbb P(N_\infty\geq M)=1$ for every $M$, and hence $N_\infty=\infty$ almost surely.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
