<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [proper convex function](../../../../../../proper-convex-function.md) $E$ that is [lower semicontinuous](../../../../../../lower-semicontinuity.md) on a [Hilbert space](../../../../../../hilbert-space-split.md), its [proximal operator](../../../../../../proximal-operator.md) at scale $\gamma>0$ is

$$
\boxed{\operatorname{prox}_{\gamma E}(z)=\arg\min_x\left\{\frac12\|x-z\|^2+\gamma E(x)\right\}=(I+\gamma\partial E)^{-1}z.}
$$

The minimizer is unique because the objective is [strongly convex](../../../../../../strongly-convex-function.md); existence follows from the closed proper convex functional and the coercive quadratic, using an affine lower bound. The [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) is $0\in x-z+\gamma\partial E(x)$, which is exactly the displayed [resolvent of a monotone operator](../../../../../../resolvent-of-a-monotone-operator.md) relation. Setting $\gamma=1$ gives the unscaled proximity or resolvent operator requested here. This is a nonlinear resolvent of the [subdifferential](../../../../../../subdifferential.md), distinct from the spectral resolvent of a linear operator.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
