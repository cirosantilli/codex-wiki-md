<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the reverse description, a fixed card avoids selection in one shuffle with probability $1-k/n$. After $t$ shuffles, a union bound gives

$$
\mathbb P(\tau>t)
\leq n(1-k/n)^t
\leq ne^{-kt/n}.
$$

For a strong stationary time, the [separation distance](../../../../../../../separation-distance.md) and hence [total variation distance](../../../../../../../total-variation-distance.md) at time $t$ are at most $\mathbb P(\tau>t)$. Taking

$$
t=\frac nk\log n+\frac nk\log(1/\varepsilon)
$$

makes this at most $\varepsilon$. Since $k\geq1$, the second term is at most $C(\varepsilon)n$, proving

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)
\leq\frac nk\log n+C(\varepsilon)n.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 215](../../../../paper-215-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
