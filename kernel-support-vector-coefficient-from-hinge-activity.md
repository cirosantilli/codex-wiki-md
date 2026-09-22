# Kernel support-vector coefficient from hinge activity

↑ **Parent:** [Soft-margin support vector machine](soft-margin-support-vector-machine.md)

For the kernel [support vector machine](support-vector-machine.md) objective $n^{-1}\sum_i(1-Y_i(\mu+K_i^T\alpha))_++\lambda\alpha^TK\alpha$, assume $Y_i\in\{-1,1\}$, $\lambda>0$, and that the [kernel matrix](kernel-matrix.md) $K$ is invertible. The [subdifferential](subdifferential.md) optimality equation gives

$$
\alpha_i=Y_it_i/(2n\lambda),\qquad t_i=\begin{cases}1&Y_i(\mu+K_i^T\alpha)<1,\\{}[0,1]&Y_i(\mu+K_i^T\alpha)=1,\\0&Y_i(\mu+K_i^T\alpha)>1.\end{cases}
$$

Thus strict margins greater than one force zero coefficients, while misclassified observations have nonzero coefficients. Invertibility matters: a singular [kernel matrix](kernel-matrix.md) allows coefficient changes in its [null space](kernel-of-a-linear-map.md) without changing the fitted [function](function-split.md) or objective.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/5/solution.md)
