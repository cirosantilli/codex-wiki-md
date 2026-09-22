<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is a small incompatibility in the printed [cutoff function](../../../../../cutoff-function.md) assumptions. No $\varphi\in C_c^\infty(B_1)$ can equal one on $B_{1/2}$ and satisfy $|\nabla\varphi|\leq2$: for a unit vector $e$, choose $t<1$ beyond its [support](../../../../../support.md). Continuity gives $\varphi(e/2)=1$, while the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) would give $1\leq2(t-1/2)<1$. Replace the number $2$ by a fixed sufficiently large absolute constant $C_0$; such a [cutoff function](../../../../../cutoff-function.md) exists, and the requested [Caccioppoli inequality](../../../../../caccioppoli-inequality.md) is unchanged apart from its constant. We keep $M=\|\nabla\varphi\|_\infty$ in the calculation, which also yields the formal bound under the printed assumptions.

The [weak formulation](../../../../../weak-formulation.md) is $\int_{B_1}A\nabla u\cdot\nabla\zeta=0$ for [test functions](../../../../../test-function.md) $\zeta$. Since $A$ is bounded, this extends by [density of smooth functions in a Sobolev space](../../../../../density-of-smooth-functions-in-a-sobolev-space.md) to every $\zeta\in H_0^1(B_1)$. Part (a)(ii), followed by [mollification](../../../../../mollification.md) inside the [compact support](../../../../../compact-support.md), makes $\varphi^2(u-k)$ an admissible choice. The [product rule](../../../../../product-rule.md) gives

$$
0=\int\varphi^2 A\nabla u\cdot\nabla u
+2\int\varphi(u-k)A\nabla u\cdot\nabla\varphi.
$$

Put $X=\int\varphi^2|\nabla u|^2$ and $Y=\int(u-k)^2|\nabla\varphi|^2$. The lower and upper [uniform ellipticity](../../../../../uniformly-elliptic-operator.md) bounds, together with [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), imply

$$
\lambda X\leq2\Lambda X^{1/2}Y^{1/2}.
$$

If $X=0$ the conclusion is immediate. Otherwise divide by $X^{1/2}$ and square to obtain $X\leq4\Lambda^2\lambda^{-2}Y$. Since $\varphi=1$ on $B_{1/2}$,

$$
\boxed{\int_{B_{1/2}}|\nabla u|^2\,dx
\leq\frac{4\Lambda^2 M^2}{\lambda^2}\int_{B_1}(u-k)^2\,dx.}
$$

For a fixed valid [cutoff function](../../../../../cutoff-function.md), $M\leq C_0$, this has the required constant independent of $k$. Formally inserting the printed value $M=2$ gives $16\Lambda^2/\lambda^2$. No derivative of $A$ was taken, so differentiability of the coefficients is unnecessary.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
