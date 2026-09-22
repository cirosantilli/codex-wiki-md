# Squared-slack support vector machine

↑ **Parent:** [Soft-margin support vector machine](soft-margin-support-vector-machine.md)

The squared-slack [support vector machine](support-vector-machine.md) uses constraints $y_i(w\cdot x_i+b)\geq1-\xi_i$. With an unpenalized intercept, its [Lagrangian dual problem](lagrangian-dual-problem.md) maximizes $\sum_i\alpha_i-\tfrac12\sum_{i,j}\alpha_i\alpha_jy_iy_jK(x_i,x_j)-\tfrac1{4C}\sum_i\alpha_i^2$ subject to $\alpha_i\geq0$ and $\sum_i\alpha_i y_i=0$. The square adds a diagonal penalty in the dual rather than a finite upper box constraint. The [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) give $w=\sum_i\alpha_i y_i\phi(x_i)$ and $\xi_i=\alpha_i/(2C)$ for a [feature map](feature-map.md) realizing the [positive-semidefinite kernel](positive-semidefinite-kernel-split.md) $K$.

## ↑ Ancestors (10)

1. [Soft-margin support vector machine](soft-margin-support-vector-machine.md)
2. [Support vector machine](support-vector-machine.md)
3. [Classification in statistical learning](classification-in-statistical-learning.md)
4. [Statistical learning](statistical-learning-split.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-learning-theory/2/a/solution.md)
