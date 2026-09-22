# EM transition-count update on a tree

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

For a common unconstrained [Markov kernel](markov-kernel.md) on the edges of a rooted [tree](tree-graph-theory.md), let $N_{ab}$ be the [conditional expectation](conditional-expectation.md) of the number of transitions $a\to b$, given observed leaves and the old [Markov kernel](markov-kernel.md). The [expectation-maximization algorithm](expectation-maximization-algorithm.md) maximizes $\sum_{a,b}N_{ab}\log K_{ab}$ over row [probability distributions](probability-distribution.md), giving $K_{ab}^{\mathrm{new}}=N_{ab}/\sum_cN_{ac}$. A row with zero total count is unrestricted by this objective. [Belief propagation](belief-propagation.md) computes the counts exactly on a [tree](tree-graph-theory.md).

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/2/solution.md)
