<h1 id="7h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $h(i)$ be the probability of reaching state $3$ before state $0$. The boundary values are $h(0)=0$ and $h(3)=1$. [First-step analysis](../../../../../../first-step-analysis.md) at states $1$ and $2$ gives

$$
h(1)=\frac12h(2),
\qquad
h(2)=\frac12h(1)+\frac12.
$$

Therefore $h(1)=h(1)/4+1/4$, so the requested [hitting probability](../../../../../../hitting-probability.md) is

$$
\boxed{h(1)=\frac13}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7H](../../7h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
