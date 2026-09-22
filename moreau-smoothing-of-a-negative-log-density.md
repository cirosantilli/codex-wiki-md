# Moreau smoothing of a negative log-density

↑ **Parent:** [Moreau envelope](moreau-envelope.md)

For a [proper convex function](proper-convex-function.md) with [sequential lower semicontinuity](sequential-lower-semicontinuity.md) $U=-\log\mu$, form $U_\lambda(x)=\inf_y\{U(y)+\lambda\|x-y\|^2\}$ with $\lambda>0$. The [Moreau envelope](moreau-envelope.md) theorem gives $\nabla U_\lambda(x)=2\lambda(x-\operatorname{prox}_{U/(2\lambda)}(x))$. If $e^{-U_\lambda}$ is integrable, it defines a smooth surrogate [probability density function](probability-density-function.md). Infimizing the [logarithm](logarithm.md) of a [probability density function](probability-density-function.md) with a positive quadratic penalty has the opposite sign and does not generally smooth it. For the [Laplace distribution](laplace-distribution.md), that incorrect operation leaves $-\log2-|x|-1/(4\lambda)$, which is not differentiable at zero.

## ↑ Ancestors (7)

1. [Moreau envelope](moreau-envelope.md)
2. [Proximal operator](proximal-operator.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/6/solution.md)
