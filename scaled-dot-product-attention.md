# Scaled dot-product attention

↑ **Parent:** [Self-attention](self-attention.md)

With query and key dimension $d_k$, form the score [matrix](matrix.md) $QK^T/\sqrt{d_k}$, apply the [softmax function](softmax-function.md) row by row, and multiply by the values $V$. If query and key coordinates have independent unit [variance](variance-split.md), their dot product has [variance](variance-split.md) $d_k$; division by $\sqrt{d_k}$ keeps that score scale of order one. Optional additive masks exclude forbidden keys before the [softmax function](softmax-function.md).

## ↑ Ancestors (10)

1. [Self-attention](self-attention.md)
2. [Transformer model](transformer-model.md)
3. [Neural network](neural-network.md)
4. [Statistical learning](statistical-learning-split.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Multi-head attention](multi-head-attention.md)
- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/3/a/i/solution.md)
- [Self-attention](self-attention.md)
