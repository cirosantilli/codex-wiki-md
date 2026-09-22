# Repeated singleton-removal allocation

↑ **Parent:** [Uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md)

In repeated [uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md), remove each ball that is alone in its bin and independently reallocate all remaining balls in the next round. If $B_j$ balls remain, the [conditional expectation](conditional-expectation.md) of the next count is $B_j[1-(1-1/n)^{B_j-1}]$ for $B_j\geq2$, and zero for $B_j\leq1$. The surviving-ball [indicator random variables](indicator-random-variable.md) need not be [independent](independent-random-variables.md). For two balls and two bins, both remain with [probability](probability.md) $2^{-j}$ after $j$ rounds, so $\mathbb E B_j=2^{1-j}$.

## ↑ Ancestors (9)

1. [Uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md)
2. [Multinomial distribution](multinomial-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Probability and computing](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/probability-and-computing-split.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/probability-and-computing/2/d/solution.md)
