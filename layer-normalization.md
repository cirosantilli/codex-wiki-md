# Layer normalization

↑ **Parent:** [Neural network](neural-network.md)

For $z\in\mathbb R^d$, define $\bar z=d^{-1}\sum_jz_j$ and $s_z^2=d^{-1}\sum_j(z_j-\bar z)^2$. Layer normalization returns $\gamma\odot(z-\bar z\mathbf1)/\sqrt{s_z^2+\varepsilon}+\beta$, with learned coordinatewise scale $\gamma$, shift $\beta$, and fixed $\varepsilon>0$. In a [transformer block](transformer-block.md), this normalization is applied across feature coordinates separately within each example and sequence position; it does not average over a batch.

## ↑ Ancestors (8)

1. [Neural network](neural-network.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/3/a/i/solution.md)
- [Transformer block](transformer-block.md)
