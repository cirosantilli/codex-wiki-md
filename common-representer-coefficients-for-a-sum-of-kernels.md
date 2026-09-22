# Common representer coefficients for a sum of kernels

↑ **Parent:** [Sum of reproducing-kernel Hilbert spaces](sum-of-reproducing-kernel-hilbert-spaces.md)

For a real-valued [loss function](loss-function.md) depending only on evaluations at $x_1,\ldots,x_n$, and a positive squared-norm penalty, any minimizing tuple in a [sum of reproducing-kernel Hilbert spaces](sum-of-reproducing-kernel-hilbert-spaces.md) has the form

$$
\widehat f_j=\sum_{i=1}^n\widehat\alpha_i k_j(\cdot,x_i)
$$

with the same coefficient [vector](vector.md) for every component. The tuple must be the unique minimum-norm decomposition of its sum. Apply the [representer theorem](representer-theorem.md) to that sum and note that the displayed tuple has total squared [norm](norm.md) $\sum_j\widehat\alpha^TK_j\widehat\alpha=\widehat\alpha^T(\sum_jK_j)\widehat\alpha$, exactly the [norm](norm.md) of the sum. This argument is conditional on existence of a [minimizer](global-minimizer.md); arbitrary [loss functions](loss-function.md) need not attain their infimum.

## ↑ Ancestors (7)

1. [Sum of reproducing-kernel Hilbert spaces](sum-of-reproducing-kernel-hilbert-spaces.md)
2. [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)
3. [Positive-semidefinite kernel](positive-semidefinite-kernel.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/1/solution.md)
