# Four-input parity network

↑ **Parent:** [Feedforward neural network](feedforward-neural-network.md)

Let $S$ be the number of active inputs. Four [hidden units](hidden-unit.md) $h_m=H(S-m+1/2)$, $m=1,2,3,4$, detect successively larger counts. A [binary threshold unit](binary-threshold-unit.md) with weights $(1,-1,1,-1)$ on these features and threshold $1/2$ returns one precisely for $S=1,3$. Each hidden input weight is one. This computes parity with a single hidden layer, but representability does not guarantee easy learning by [backpropagation](backpropagation.md).

## ↑ Ancestors (9)

1. [Feedforward neural network](feedforward-neural-network.md)
2. [Neural network](neural-network.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/2/d/solution.md)
