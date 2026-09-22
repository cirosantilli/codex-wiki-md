# Two-sided interarrival test for overlap

↑ **Parent:** [Poisson process](poisson-process-split.md)

Consider a homogeneous [Poisson process](poisson-process-split.md) of arrival rate $\lambda$, with each arrival staying for a fixed duration $d>0$. For any fixed arrival index $k\geq2$, its visit overlaps another visit if the preceding interarrival time is below $d$ or the following interarrival time is below $d$. If the nearest preceding arrival has already left then all earlier ones have left; if the next arrival is too late then all later ones are too late. These two gaps are independent [exponential random variables](exponential-distribution.md), so the probability of no overlap is $e^{-\lambda d}e^{-\lambda d}$. Taking its complement gives the formula. This is an unconditional statement for a fixed indexed arrival; conditioning on a fixed calendar closing time would change the problem.

## ↑ Ancestors (6)

1. [Poisson process](poisson-process-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2013/m/1/c/solution.md)
