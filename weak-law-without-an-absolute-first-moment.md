# Weak law without an absolute first moment

↑ **Parent:** [Weak law of large numbers](weak-law-of-large-numbers.md)

Let $X$ have a [symmetric probability distribution](symmetric-probability-distribution.md) with $\mathbb P(|X|>x)=1/(x\log x)$ for $x\ge e$, mass $1-1/e$ at zero, and no mass with $0<|X|<e$. Then $\mathbb E|X|=\infty$, but independent copies satisfy the [weak law of large numbers](weak-law-of-large-numbers.md) with limit zero. Indeed $n\mathbb P(|X|>n)=1/\log n\to0$. Their symmetric truncations $Y_{n,j}=X_j\mathbf1_{\{|X_j|\le n\}}$ have mean zero and second moment $O(n/\log n)$, so [Chebyshev's inequality](chebyshev-inequality.md) gives $n^{-1}\sum_{j\le n}Y_{n,j}\to0$ in probability. A union bound shows that the original and truncated sums differ with probability tending to zero. This also gives a differentiable [characteristic function](characteristic-function.md) at zero whose derivative cannot be interpreted as an absolutely convergent expectation.

## ↑ Ancestors (8)

1. [Weak law of large numbers](weak-law-of-large-numbers.md)
2. [Convergence in probability](convergence-in-probability.md)
3. [Convergence of random variables](convergence-of-random-variables-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31/3/solution.md)
