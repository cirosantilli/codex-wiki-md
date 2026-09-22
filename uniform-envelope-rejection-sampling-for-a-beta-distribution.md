# Uniform-envelope rejection sampling for a beta distribution

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

For $a,b>1$, the maximum of $r$ on $[0,1]$ occurs at $(a-1)/(a+b-2)$. If one parameter is one, the maximum is attained at the corresponding endpoint; if both are one, $r$ is constant. Let $M=\sup r$. Accept an [independent](independent-random-variables.md) [uniform distribution](continuous-uniform-distribution.md) proposal $X$ when another uniform draw is at most $r(X)/M$. The accepted [probability density function](probability-density-function.md) is the [Beta distribution](beta-distribution.md), and acceptance [probability](probability.md) is $B(a,b)/M$.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/3/iii/solution.md)
