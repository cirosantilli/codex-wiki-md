<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $X_1\sim\operatorname{Binomial}(22,\pi_0)$ be interim responses and independently $X_2\sim\operatorname{Binomial}(32,\pi_0)$ be second-stage responses. The design rejects immediately when $X_1\geq e_1=10$, continues when $r_1<X_1<e_1$, and after continuation rejects when $X_1+X_2\geq r=20$. Hence at $\pi_0=0.3$,

$$
\alpha=
\sum_{x=10}^{22}b(22,0.3,x)
+\sum_{x=8}^{9}b(22,0.3,x)
\sum_{y=20-x}^{32}b(32,0.3,y).
$$

This is the type-I error of the specified [two-stage clinical trial design](../../../../../../two-stage-clinical-trial-design.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
