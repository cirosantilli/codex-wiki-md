# Marginal and pair probabilities in sampling without replacement

↑ **Parent:** [Sampling without replacement](sampling-without-replacement.md)

Take a uniformly random [permutation](permutation.md) of $N>1$ distinguishable objects, of which $K$ are marked. Let $B_i$ mean that position $i$ is marked. Every object is equally likely at a specified position, so $\mathbb P(B_i)=K/N$. For distinct positions $i,j$, their ordered pair is uniform among $N(N-1)$ distinct-object pairs, of which $K(K-1)$ are marked pairs. This proves the second formula. For $K>0$, the [conditional probability](conditional-probability.md) is $\mathbb P(B_i\mid B_j)=(K-1)/(N-1)$.

For the count $M_m$ of marked objects among the first $m$ positions, [indicator random variables](indicator-random-variable.md) and [linearity of expectation](linearity-of-expectation.md) give $\mathbb E[M_m]=mK/N$. These draws are [exchangeable](exchangeable-random-variables.md) but generally dependent; equal marginal [probabilities](probability.md) do not imply [independence](independent-random-variables.md).

## ↑ Ancestors (7)

1. [Sampling without replacement](sampling-without-replacement.md)
2. [Probability sampling](probability-sampling.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/16/a/iii/solution.md)
