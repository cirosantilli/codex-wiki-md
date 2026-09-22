# Squared-error backpropagation

↑ **Parent:** [Backpropagation](backpropagation.md)

For squared loss $E=\sum_k(t_k-z_k)^2/2$, let $e_k=(t_k-z_k)g_k'(x_k)$ and $e_j=g_j'(x_j)\sum_kw_{jk}e_k$. The [chain rule](chain-rule.md) gives $\partial E/\partial w_{jk}=-e_kz_j$ and $\partial E/\partial w_{ij}=-e_jz_i$. A [gradient descent](gradient-descent.md) step of size $\eta$ uses $\Delta w_{jk}=\eta e_kz_j$ and $\Delta w_{ij}=\eta e_jz_i$, with every derivative evaluated at the same pre-update weights.

## ↑ Ancestors (10)

1. [Backpropagation](backpropagation.md)
2. [Feedforward neural network](feedforward-neural-network.md)
3. [Neural network](neural-network.md)
4. [Statistical learning](statistical-learning-split.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/2/a/solution.md)
