<h1 id="30k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Because $A$ is nondecreasing and $A_{n+1}$ is $\mathcal F_n$-measurable,

$$
\{\tau^*\leq n\}=\{A_{n+1}>0\}\in\mathcal F_n.
$$

The convention $A_{N+1}=\infty$ ensures $\tau^*\leq N$, so $\tau^*$ is a bounded stopping time.

By minimality, $A_{\tau^*}=0$ and $A_{\tau^*+1}-A_{\tau^*}>0$. Part (d) then gives

$$
V_{\tau^*}=Z_{\tau^*}.
$$

Moreover $M_{\tau^*}=V_{\tau^*}+A_{\tau^*}=Z_{\tau^*}$. Optional sampling for the martingale $M$ now yields

$$
\boxed{
\mathbb E[Z_{\tau^*}]
=\mathbb E[M_{\tau^*}]
=M_0=V_0.}
$$

Together with part (a), this proves that $\tau^*$ is optimal and $V_0$ is the optimal stopping value.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
