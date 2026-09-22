# Sign-truncated normal sampling

↑ **Parent:** [Truncated normal distribution](truncated-normal-distribution.md)

To draw $N(\mu,1)$ restricted to a positive value, let $a=\Phi(-\mu)$ and return $\mu+\Phi^{-1}(a+(1-a)U)$ for uniform $U\in(0,1)$. For restriction to a negative value use $\mu+\Phi^{-1}(aU)$. These are [inverse transform sampling](inverse-transform-sampling.md) constructions. Repeatedly drawing an untruncated normal until its sign agrees is also exact, but inefficient for rare signs.

## ↑ Ancestors (8)

1. [Truncated normal distribution](truncated-normal-distribution.md)
2. [Truncated distribution](truncated-distribution.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/3/solution.md)
