# Iterative soft-thresholding algorithm

↑ **Parent:** [Proximal gradient method](proximal-gradient-method.md)

The iterative soft-thresholding algorithm applies the [proximal gradient method](proximal-gradient-method.md) to $\|x\|_1+\tfrac12\|Ax-y\|_2^2$:

$$
x^{k+1}=S_\tau(x^k-\tau A^T(Ax^k-y)),\qquad0<\tau\le\|A\|_{2\to2}^{-2}.
$$

Here $S_\tau$ is coordinatewise [soft thresholding](soft-thresholding.md). The objective is [convex](convex-function.md) and coercive, so iterates converge to a minimizer in finite dimensions; uniqueness requires additional hypotheses.

## ↑ Ancestors (7)

1. [Proximal gradient method](proximal-gradient-method.md)
2. [Proximal operator](proximal-operator.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/5/d/solution.md)
