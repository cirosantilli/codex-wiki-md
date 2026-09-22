# Kernel support vector machine

↑ **Parent:** [Support vector machine](support-vector-machine.md)

A kernel support vector machine trains a [support vector machine](support-vector-machine.md) using a [positive-definite kernel](positive-semidefinite-kernel.md) instead of explicit feature coordinates. The [kernel trick](kernel-trick.md) evaluates all required feature inner products through the training [Gram matrix](gram-matrix.md); prediction is $\sum_i\alpha_i y_i k(x_i,x)+b$. Nonzero dual coefficients identify [support vectors](support-vector.md). An unpenalized intercept supplies the dual equality $\sum_i\alpha_i y_i=0$. The [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md) construction explains why a positive-semidefinite kernel defines valid feature geometry.

## ↑ Ancestors (9)

1. [Support vector machine](support-vector-machine.md)
2. [Classification in statistical learning](classification-in-statistical-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/5/solution.md)
