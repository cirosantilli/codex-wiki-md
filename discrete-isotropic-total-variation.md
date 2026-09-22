# Discrete isotropic total variation

↑ **Parent:** [Total variation denoising](total-variation-denoising.md)

With zero forward differences at the grid boundary, discrete isotropic total variation is the sum of the Euclidean lengths of the two-component forward gradients. Its dual constraint is the product of unit Euclidean balls, and minimizing $\tfrac12\|g-D^*p\|_2^2$ over that product yields $u_*=g-D^*p_*$. The exact difference [adjoint operator](adjoint-operator.md) is essential. A dual [proximal gradient method](proximal-gradient-method.md) projects $p+\tau D(g-D^*p)$ pointwise onto unit balls; $0<\tau\le1/8$ is safe on an unscaled square grid.

**Table of contents**

- [Projection residual for discrete total variation](projection-residual-for-discrete-total-variation.md)
  - [Projected-gradient dual total variation algorithm](projected-gradient-dual-total-variation-algorithm.md)

## ↑ Ancestors (9)

1. [Total variation denoising](total-variation-denoising.md)
2. [Total variation seminorm on a domain](total-variation-seminorm-on-a-domain.md)
3. [Variational regularization](variational-regularization.md)
4. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
5. [Inverse problem](inverse-problem-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Box-constrained TV-L1 denoising](box-constrained-tv-l1-denoising.md)
- [Global discrete gradient-norm denoising](global-discrete-gradient-norm-denoising.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/5/c/solution.md)
