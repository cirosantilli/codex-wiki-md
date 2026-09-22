# Neural tangent kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)

For a differentiable [neural network](neural-network.md) $f(\theta,x)$ and initialization law $P$, the expected neural tangent kernel is $k_{\mathrm{NTK}}(x,x')=\mathbb E_{\theta\sim P}\langle\nabla_\theta f(\theta,x),\nabla_\theta f(\theta,x')\rangle$, assuming finite diagonal [expectations](expected-value-split.md). At a fixed parameter value the corresponding [inner product](inner-product-split.md) defines the empirical neural tangent kernel. Both are [positive-semidefinite kernels](positive-semidefinite-kernel-split.md), since a finite [quadratic form](quadratic-form-split.md) is respectively an expected squared [norm](norm.md) or a squared [norm](norm.md). In suitable infinite-width scalings, the empirical [kernel matrix](kernel-matrix.md) converges to a deterministic limit and remains constant during training. Squared-error [gradient flow](gradient-flow.md) then has the same training-prediction dynamics as [kernel regression](kernel-regression.md) with this limit, provided the initial predictions match.

## ↑ Ancestors (5)

1. [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/2/c/ii/solution.md)
- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/2/c/iv/solution.md)
