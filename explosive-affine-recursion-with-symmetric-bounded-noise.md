# Explosive affine recursion with symmetric bounded noise

↑ **Parent:** [Autoregressive model](autoregressive-model.md)

For [independent](independent-random-variables.md) fair signs, $|X_n|\to\infty$ [almost surely](almost-sure-convergence.md) from every deterministic initial value. Outside $[-L,L]$ with $L>1/(a-1)$, the sign is preserved and $|X_{n+k}|\geq a^k(|X_n|-1/(a-1))+1/(a-1)$. To reach that region, choose $m$ so $(a^m-1)/(a-1)>L$. At the beginning of each $m$-step block, choose the sign of the current value; a block of that sign pushes the absolute value past $L$ and has conditional probability $2^{-m}$. The chance of remaining inside after $k$ blocks is at most $(1-2^{-m})^k$. This proof avoids any assumption about a density of the limiting random series.

## ↑ Ancestors (7)

1. [Autoregressive model](autoregressive-model.md)
2. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/2/c/solution.md)
