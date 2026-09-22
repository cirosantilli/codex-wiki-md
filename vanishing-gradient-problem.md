# Vanishing gradient problem

↑ **Parent:** [Neural network](neural-network.md)

Repeated differentiation through a deep or recurrent [neural network](neural-network.md) can make [gradients](gradient.md) associated with distant layers or earlier sequence positions extremely small. A simple mechanism is a product of step [Jacobian matrices](jacobian-matrix.md) whose [operator norms](operator-norm.md) are all bounded above by some $a<1$: the product [operator norm](operator-norm.md) is then at most $a^L$ over $L$ steps by submultiplicativity. This can impede learning long-range dependencies in a [recurrent neural network](recurrent-neural-network.md).

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
