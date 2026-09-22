# Lagged Fibonacci generator

↑ **Parent:** [Pseudorandom number generator](pseudorandom-number-generator.md)

A [pseudorandom number generator](pseudorandom-number-generator.md) whose state sequence combines earlier values at two fixed lags, for example $S_n=(S_{n-j}+S_{n-k})\bmod m$ with $0<j<k$. A seed supplies the first $k$ values. A circular buffer of $k$ entries suffices for generation because each update uses only the retained lag window.

## ↑ Ancestors (6)

1. [Pseudorandom number generator](pseudorandom-number-generator.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
