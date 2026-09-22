# Cure model

↑ **Parent:** [Survival analysis](survival-analysis-split.md)

A [cure model](cure-model.md) mixes an individual class with identically zero [hazard function](hazard-function.md) and a susceptible class with [survivor function](survival-function.md) $S_*$. For $0\leq\pi<1$, its representation as a [proportional frailty model](proportional-frailty-model.md) with $\mathbb E U=1$ is $U=0$ with probability $\pi$ and $U=1/(1-\pi)$ otherwise, with [baseline hazard](baseline-hazard.md) $h_0=(1-\pi)h_*$. The frailty law is a mixture of two [Dirac measures](dirac-measure.md), rather than an ordinary density. Its [Laplace transform](laplace-transform.md) evaluated at $H_0$ gives the displayed [survivor function](survival-function.md). The limiting survival equals $\pi$ when $S_*(t)\to0$; otherwise the plateau also includes susceptible individuals who never experience the event.

## ↑ Ancestors (5)

1. [Survival analysis](survival-analysis-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cure model](cure-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44/3/solution.md)
