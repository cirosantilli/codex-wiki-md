# Proximal gradient method

↑ **Parent:** [Proximal operator](proximal-operator.md)

The proximal gradient method minimizes $g+h$, where $g$ has an $L$-Lipschitz gradient and $h$ is convex with a tractable [proximal operator](proximal-operator.md), by $x_{r+1}=\operatorname{prox}_{\alpha h}(x_r-\alpha\nabla g(x_r))$. A standard choice $0<\alpha\leq1/L$ gives objective error $O(1/r)$ in the general convex case.

This basic forward-backward update is one of the [proximal gradient methods for learning](proximal-gradient-methods-for-learning.md).

**Table of contents**

- [Alternating proximal-gradient operator](alternating-proximal-gradient-operator.md)
  - [Implicit nonsmooth block in alternating proximal-gradient iteration](implicit-nonsmooth-block-in-alternating-proximal-gradient-iteration.md)
  - [Mixed-point norm identity for alternating updates](mixed-point-norm-identity-for-alternating-updates.md)
- [Iterative soft-thresholding algorithm](iterative-soft-thresholding-algorithm.md)

## ↑ Ancestors (6)

1. [Proximal operator](proximal-operator.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Discrete isotropic total variation](discrete-isotropic-total-variation.md)
- [Iterative soft-thresholding algorithm](iterative-soft-thresholding-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-339/2/e/solution.md)
- [Projected gradient descent](projected-gradient-descent.md)
- [Proximal gradient methods for learning](proximal-gradient-methods-for-learning.md)
