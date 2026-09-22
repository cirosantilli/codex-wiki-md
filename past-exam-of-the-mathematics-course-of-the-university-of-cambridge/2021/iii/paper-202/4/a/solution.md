<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Continuity gives $X_{\tau_a}=a$ on $\{\tau_a<\infty\}$. The stopped process $X^{\tau_a}$ is bounded by $a$ and is therefore a true martingale. Hence

$$
1=\mathbb E X_{t\wedge\tau_a}
=a\mathbb P(\tau_a\leq t)+\mathbb E[X_t\mathbf1_{\{\tau_a>t\}}].
$$

The second term tends to zero by bounded convergence because $X_t\to0$ and it is bounded by $a$. Thus

$$
\boxed{\mathbb P(\tau_a<\infty)=\mathbb P(\sup_{t\geq0}X_t>a)=\frac1a}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
