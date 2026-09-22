<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mu=\mathbb EZ$ and $h(u)=(1+u)\log(1+u)-u$. For $\lambda>0$, the [Chernoff bound](../../../../../../chernoff-bound.md) and the assumed cumulant-generating-function estimate give

$$
\mathbb P(Z-\mu\geq t)
\leq\inf_{\lambda>0}
\exp\{-\lambda t+\mu(e^\lambda-\lambda-1)\}.
$$

The optimizer satisfies $e^\lambda=1+t/\mu$, and hence

$$
\mathbb P(Z-\mu\geq t)
\leq e^{-\mu h(t/\mu)}
\leq\exp\!\left(-\frac{t^2}{2\mu+2t/3}\right).
$$

For the left tail, apply the same argument at a negative parameter. If $0<t<\mu$ the optimizer satisfies $e^{-\lambda}=1-t/\mu$, giving

$$
\mathbb P(Z-\mu\leq-t)
\leq\exp\{-\mu[(1-t/\mu)\log(1-t/\mu)+t/\mu]\}
\leq e^{-t^2/(2\mu)}.
$$

For $t\geq\mu$, nonnegativity of $Z$ makes the strict lower-tail event empty, with the boundary handled directly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
