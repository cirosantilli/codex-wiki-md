<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $F(x)=\tfrac12\|Ax-y\|_2^2$, with $\nabla F(x)=A^T(Ax-y)$ and Lipschitz constant $L=\|A\|_{2\to2}^2$, and $H(x)=\|x\|_1$. The [proximal operator](../../../../../../proximal-operator.md) separates over coordinates. Solving the scalar [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) $0\in\partial|z|+(z-v)/\tau$ gives [soft thresholding](../../../../../../soft-thresholding.md) $S_\tau(v)=\operatorname{sgn}(v)(|v|-\tau)_+$. Therefore the [iterative soft-thresholding algorithm](../../../../../../iterative-soft-thresholding-algorithm.md) is

$$
\boxed{x^{k+1}=S_\tau\bigl(x^k-\tau A^T(Ax^k-y)\bigr),\qquad0<\tau\le\|A\|_{2\to2}^{-2}.}
$$

Here [soft thresholding](../../../../../../soft-thresholding.md) is applied coordinatewise. The objective is [convex](../../../../../../convex-function.md) and coercive because of its $\ell^1$ term, so minimizers exist and the [proximal gradient method](../../../../../../proximal-gradient-method.md) converges to a minimizer. Uniqueness need not hold if $A$ has a nontrivial [null space](../../../../../../kernel-of-a-linear-map.md). If $A=0$, the unique minimizer is zero and any positive step size is admissible.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
