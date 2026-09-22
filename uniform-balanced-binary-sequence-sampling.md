# Uniform balanced binary sequence sampling

↑ **Parent:** [Randomized algorithm](randomized-algorithm.md)

A balanced [binary sequence](bitstream.md) of length $2n$ has $n$ entries of each kind. Uniformly sample an $n$-element [subset](subset.md) of the positions and place the first kind there. If $2n$ is a power of two, repeatedly draw uniform positions using $\log_2(2n)$ fair random [bits](bit.md), reject previously selected positions, and stop after $n$ distinct positions. Each new position is uniform among those remaining, making every $n$-element [subset](subset.md) equally likely. The expected number of draws is $\sum_{s=0}^{n-1}2n/(2n-s)<2n$, giving $O(n\log n)$ expected random [bits](bit.md).

## ↑ Ancestors (4)

1. [Randomized algorithm](randomized-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/probability-and-computing/3/c/solution.md)
