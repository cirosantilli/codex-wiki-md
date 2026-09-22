<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\widehat\Omega^{(k)}$ solve the $k$th diagonal-block problem and set

$$
\widetilde\Omega=
\begin{bmatrix}\widehat\Omega^{(1)}&0\\0&\widehat\Omega^{(2)}\end{bmatrix}.
$$

Its inverse is block diagonal. On each diagonal block, the [Graphical-Lasso Karush-Kuhn-Tucker conditions](../../../../../../graphical-lasso-karush-kuhn-tucker-conditions.md) hold by the definition of $\widehat\Omega^{(k)}$. On the off-diagonal blocks choose

$$
Z^{(12)}=-S^{(12)}/\lambda,
\qquad Z^{(21)}=-S^{(21)}/\lambda.
$$

The assumed inequalities $|S_{ij}|\leq\lambda$ ensure that every entry lies in $[-1,1]$, exactly the allowed [subgradient](../../../../../../subgradient.md) at a zero entry of $\widetilde\Omega$.

**Thus $-\widetilde\Omega^{-1}+S+\lambda Z=0$ on every block. The KKT conditions and the fact that the objective is [strictly convex](../../../../../../strictly-convex-function.md) prove that $\widetilde\Omega=\widehat\Omega$, giving the claimed block decomposition.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
