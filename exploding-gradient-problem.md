# Exploding gradient problem

↑ **Parent:** [Neural network](neural-network.md)

Repeated differentiation through a deep or recurrent [neural network](neural-network.md) can make some [gradient](gradient.md) components extremely large. In the scalar recurrence $h_t=ah_{t-1}$, the derivative with respect to $h_0$ is $a^t$, which grows exponentially if $|a|>1$. Large individual matrix norms alone do not imply such growth, because directions can change or cancel; the full product of step [Jacobian matrices](jacobian-matrix.md) determines the effect.

## ↑ Ancestors (8)

1. [Neural network](neural-network.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022/5/solution.md)
