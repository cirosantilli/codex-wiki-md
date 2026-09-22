<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $u_k\rightharpoonup u$ in $H^1(\Omega)$. Then $Du_k\rightharpoonup Du$ in $L^2(\Omega;\mathbb R^n)$. Since $F$ is a differentiable [convex function](../../../../../../convex-function.md), its supporting inequality is

$$
F(p)\geq F(q)+DF(q)\cdot(p-q).
$$

Take $p=Du_k(x)$, $q=Du(x)$ and integrate. Part (i) shows that every energy is finite and that the fixed field $DF(Du)$ belongs to $L^2$, so

$$
\mathcal F(u_k)\geq\mathcal F(u)+\int_\Omega DF(Du)\cdot(Du_k-Du).
$$

The last integral tends to zero by the definition of [weak convergence](../../../../../../weak-convergence.md) in $L^2$. Therefore

$$
\boxed{\mathcal F(u)\leq\liminf_{k\to\infty}\mathcal F(u_k).}
$$

This is [weak lower semicontinuity of convex gradient energies](../../../../../../weak-lower-semicontinuity-of-convex-gradient-energies.md). It uses a fixed supporting [gradient](../../../../../../gradient.md) at the limit; [weak convergence](../../../../../../weak-convergence.md) alone would not justify passing pointwise through the nonlinear integrand.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
