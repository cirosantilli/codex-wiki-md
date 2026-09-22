# Multiselection by balanced rank partitioning

↑ **Parent:** [Algorithm](algorithm-split.md)

To find the order statistics at ranks $k,2k,\ldots,n$ when $n/k$ is a power of two, partition into equal lower and upper rank halves and recurse, stopping at blocks of size $k$. Return each leaf block's maximum. Half boundaries are multiples of $k$, so these leaf maxima are exactly the requested ranks. Linear-time [selection](selection-algorithm.md) gives total $\Theta(n)$ partition work per internal level and $\Theta(n)$ leaf work, hence $\Theta(n(1+\log(n/k)))$ overall. The shorter displayed bound applies when $n/k\geq2$.

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/8/d/solution.md)
