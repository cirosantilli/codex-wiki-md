# Hebbian memory weights for a Hopfield network

↑ **Parent:** [Hopfield network](hopfield-network.md)

For $M$ binary units and desired patterns $\xi^\mu$, use these symmetric weights and set $w_{ii}=0$. For one pattern, the field at that pattern is $(M-1)\xi_i/M$, so it is stable. Several patterns add cross-talk terms; storage by this rule alone does not guarantee stability of every arbitrary collection of patterns.

Writing $m_\mu=M^{-1}\sum_j\xi_j^\mu x_j$ gives

$$
\sum_{j\ne i}w_{ij}x_j=\sum_\mu\xi_i^\mu m_\mu-\frac{P}{M}x_i,
$$

for $P$ stored patterns. The subtraction removes the forbidden self-couplings. It makes explicit how the desired association competes with all other stored patterns. An unintended stable state can therefore arise even though every update obeys [asynchronous Hopfield energy descent](asynchronous-hopfield-energy-descent.md).

**Table of contents**

- [Hopfield recall from a corrupted cue](hopfield-recall-from-a-corrupted-cue.md)

## ↑ Ancestors (9)

1. [Hopfield network](hopfield-network.md)
2. [Neural network](neural-network.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Hebbian learning](hebbian-learning.md)
- [Hopfield recall from a corrupted cue](hopfield-recall-from-a-corrupted-cue.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/3/d/solution.md)
