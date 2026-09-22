# Rare-jump counterexample to a strong law with convergent first-moment averages

↑ **Parent:** [Strong law of large numbers](strong-law-of-large-numbers.md)

Take independent [random variables](random-variable-split.md) equal to $1+n$ and $1-n$ with probability $1/(2n\log n)$ each, and otherwise equal to one. Their first absolute deviations are $1/\log n\to0$, so $X_n\to1$ in [L1 convergence](convergence-in-l1.md). The same triangle-inequality argument gives convergence in $L^1$ of their arithmetic averages to one. For $p>1$, however, $\mathbb E|X_n-1|^p=n^{p-1}/\log n\to\infty$.

The exceptional jumps occur infinitely often almost surely by the [Borel-Cantelli second lemma](borel-cantelli-second-lemma.md), since $\sum1/(n\log n)=\infty$. If the arithmetic averages $S_n/n$ converged to any finite value along a sample path, then $X_{n+1}/n=S_n/n-[(n-1)/n][S_{n-1}/(n-1)]$ would tend to zero. At each exceptional jump its magnitude is at least one. Thus the averages have no finite almost sure limit. Independence and convergence of first-moment averages do not alone give a [strong law of large numbers](strong-law-of-large-numbers.md).

## ↑ Ancestors (8)

1. [Strong law of large numbers](strong-law-of-large-numbers.md)
2. [Almost sure convergence](almost-sure-convergence.md)
3. [Convergence of random variables](convergence-of-random-variables-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2011/a/2/c/iii/solution.md)
