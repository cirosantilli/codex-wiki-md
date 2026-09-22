# Wigner semicircle distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wigner_semicircle_distribution)

The unit-radius [Wigner semicircle distribution](wigner-semicircle-distribution.md) has the displayed [probability density function](probability-density-function.md). Its graph is a rescaled upper semicircle. The area of the unit semicircle is $\pi/2$, so the factor $2/\pi$ normalizes it. Symmetry gives mean zero, and the substitution $x=\sin\theta$ gives variance $1/4$.

A scaled radius-$R$ version has density $2\sqrt{R^2-x^2}/(\pi R^2)$ on $(-R,R)$ and variance $R^2/4$. [Rejection sampling](rejection-sampling.md) from a uniform proposal on $(-1,1)$ accepts a proposed $x$ with probability $\sqrt{1-x^2}$; its average acceptance probability is $\pi/4$. Thus the number of proposals for one output has [geometric distribution](geometric-distribution.md) with expectation $4/\pi$. This law also describes the limiting empirical eigenvalue density in standard ensembles of large symmetric [random matrices](random-matrix.md).

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2011/s/1/b/solution.md)
- [Wigner semicircle distribution](wigner-semicircle-distribution.md)
