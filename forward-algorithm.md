# Forward algorithm

↑ **Parent:** [Hidden Markov model](hidden-markov-model.md)

The [forward algorithm](forward-algorithm.md) computes sequence likelihoods by summing over all hidden paths through a [Hidden Markov model](hidden-markov-model.md). For emitting states, $\alpha_t(i)=P(o_1,\ldots,o_t,Z_t=i)$ obeys $\alpha_{t+1}(j)=b_j(o_{t+1})\sum_i\alpha_t(i)a_{ij}$. It reuses partial sums rather than enumerating exponentially many state sequences. Silent states require additional transitions without consuming an observation. Scaling or [log-sum-exp](log-sum-exp-function.md) prevents [floating-point underflow](floating-point-underflow.md).

## ↑ Ancestors (7)

1. [Hidden Markov model](hidden-markov-model.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Backward algorithm](backward-algorithm.md)
- [Forward algorithm](forward-algorithm.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/2/b/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/2/c/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/2/e/solution.md)
