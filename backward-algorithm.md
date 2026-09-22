# Backward algorithm

↑ **Parent:** [Hidden Markov model](hidden-markov-model.md)

The [backward algorithm](backward-algorithm.md) computes suffix likelihoods in a [Hidden Markov model](hidden-markov-model.md). With $\beta_t(i)=P(o_{t+1},\ldots,o_T\mid Z_t=i)$, its recurrence is $\beta_t(i)=\sum_j a_{ij}b_j(o_{t+1})\beta_{t+1}(j)$. Together with the [forward algorithm](forward-algorithm.md), it gives posterior state probabilities proportional to $\alpha_t(i)\beta_t(i)$. The terminal condition must include any explicit End-state transition.

## ↑ Ancestors (7)

1. [Hidden Markov model](hidden-markov-model.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Backward algorithm](backward-algorithm.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/2/e/solution.md)
