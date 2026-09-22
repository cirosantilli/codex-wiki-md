<h1 id="proof-of-wald-s-equation-by-stopping-indicators">Proof of Wald's equation by stopping indicators</h1>

↑ **Parent:** [Wald's equation](wald-s-equation.md)

If $M$ is a [stopping time](stopping-time.md) for independent identically distributed integrable variables $X_i$ and $\mathbb EM<\infty$, then $\{M\geq i\}$ depends only on $X_1,\ldots,X_{i-1}$ and is independent of $X_i$. Hence

$$
\mathbb E\sum_{i=1}^M X_i
=\sum_{i\geq1}\mathbb E[X_i\mathbf1_{\{M\geq i\}}]
=\mathbb EX_1\sum_{i\geq1}\mathbb P(M\geq i)
=\mathbb EX_1\,\mathbb EM.
$$

The interchange is justified because the same calculation with $|X_i|$ gives finite expected absolute sum.

## ↑ Ancestors (6)

1. [Wald's equation](wald-s-equation.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
