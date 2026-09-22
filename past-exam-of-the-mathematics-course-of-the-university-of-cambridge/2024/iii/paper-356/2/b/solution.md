<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\xi_{1,n},\xi_{2,n}$ be [independent random variables](../../../../../../independent-random-variables.md) with the [standard normal distribution](../../../../../../standard-normal-distribution.md). The unconstrained [Milstein method](../../../../../../milstein-method.md) step is

$$
\widetilde X_{n+1}
=X_n+a_1\Delta t+\sqrt{2\Delta t}\,\xi_{1,n},
$$



$$
\widetilde Y_{n+1}
=Y_n+a_2(X_n,Y_n)\Delta t
+\sigma(Y_n)\sqrt{\Delta t}\,\xi_{2,n}
+\frac12\sigma(Y_n)\sigma'(Y_n)\Delta t
\left(\xi_{2,n}^2-1\right).
$$

The $X$ noise is additive, so its Milstein correction vanishes. The diagonal, independent noise fields commute, so no cross iterated stochastic integral is required.

Implement each [reflecting boundary condition for a diffusion](../../../../../../reflecting-boundary-condition-for-a-diffusion.md) by folding the proposed coordinate back into $[-1,1]$. One formula that also handles multiple overshoots is

$$
R(z)=1-\left|\big((z+1)\bmod4\big)-2\right|.
$$

The complete update is

$$
\boxed{X_{n+1}=R(\widetilde X_{n+1}),\qquad
Y_{n+1}=R(\widetilde Y_{n+1}).}
$$

Under the usual smoothness assumptions, the Milstein discretization has [strong order of convergence](../../../../../../strong-convergence-of-a-stochastic-numerical-method.md) one and [weak order of convergence](../../../../../../weak-convergence-of-a-stochastic-numerical-method.md) one. The reflection enforces the boundary pathwise.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
