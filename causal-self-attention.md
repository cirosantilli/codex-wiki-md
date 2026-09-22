# Causal self-attention

↑ **Parent:** [Self-attention](self-attention.md)

[Self-attention](self-attention.md) whose output at sequence position $t$ may depend only on positions at or before $t$. In a score [matrix](matrix.md), set forbidden future-position scores to negative infinity before applying the [softmax function](softmax-function.md); the corresponding weights become zero. This permits parallel computation over a known training sequence without allowing future tokens to influence earlier predictions.

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

## ← Incoming links (4)

- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/3/a/i/solution.md)
- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/3/a/ii/solution.md)
- [Self-attention](self-attention.md)
- [Transformer model](transformer-model.md)
