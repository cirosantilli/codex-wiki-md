# Birthday problem

↑ **Parent:** [Probability and statistics](probability-and-statistics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birthday_problem)

For $n$ independent uniform draws from $m$ labels, the probability of all labels being distinct is $\prod_{j=0}^{n-1}(1-j/m)$ when $n\leq m$, and zero otherwise. Applying $1-x\leq e^{-x}$ gives a collision probability at least $1-\exp[-n(n-1)/(2m)]$. The transition therefore occurs at sample size of order $\sqrt m$, not $m$: many pairs can collide before many labels have been sampled.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Classical collision query bound for Simon's problem](classical-collision-query-bound-for-simon-s-problem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/4f/solution.md)
