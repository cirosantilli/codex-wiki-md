<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the real diffusive interpretation $\gamma>0$, $U,\mu_0\in\mathbb R$, with $\nu>0$. Without a positive real diffusion coefficient the printed ordering inequality and real oscillator coordinate would need different hypotheses. Remove the drift by $\eta=e^{Ux/(2\gamma)}v$. Direct differentiation reduces the [linear complex Ginzburg-Landau equation](../../../../../../linear-complex-ginzburg-landau-equation.md) to

$$
v_t=\gamma v_{xx}+\left(\mu_0-\frac{U^2}{4\gamma}-\nu\epsilon^2x^2\right)v.
$$

Set $v=b(\xi)e^{-i(\omega_0+\epsilon\omega_1)t}$ and $\xi=\sqrt\epsilon f x$. The resulting equation is

$$
\gamma\epsilon f^2b''+\left[\mu_0-\frac{U^2}{4\gamma}+i\omega_0+\epsilon i\omega_1-\frac{\nu\epsilon}{f^2}\xi^2\right]b=0.
$$

Canceling its order-one coefficient and normalizing the quadratic term gives

$$
\boxed{\omega_0=i\left(\mu_0-\frac{U^2}{4\gamma}\right),\qquad f=(\nu/\gamma)^{1/4},\qquad \lambda=\frac{i\omega_1}{\sqrt{\nu\gamma}},\qquad b''+(\lambda-\xi^2)b=0.}
$$

The supplied decay quantization has $\lambda=2j+1$, $j=0,1,2,\ldots$. Equivalently the [Hermite functions](../../../../../../hermite-function.md) $b_j=e^{-\xi^2/2}H_j(\xi)$ solve this harmonic-oscillator problem, where $H_j$ is the physicists' [Hermite polynomial](../../../../../../hermite-polynomial.md). Thus $\omega_1=-i(2j+1)\sqrt{\nu\gamma}$ and the exact temporal [growth rates](../../../../../../growth-rate.md) are

$$
\boxed{s_j=-i(\omega_0+\epsilon\omega_1)=\mu_0-\frac{U^2}{4\gamma}-\epsilon(2j+1)\sqrt{\nu\gamma}.}
$$

The [global modes of a quadratically confined Ginzburg-Landau equation](../../../../../../global-modes-of-a-quadratically-confined-ginzburg-landau-equation.md) are

$$
\eta_j(x,t)=C_j e^{Ux/(2\gamma)-\epsilon f^2x^2/2}H_j(\sqrt\epsilon f x)e^{s_jt}.
$$

For every fixed positive $\epsilon$, the negative quadratic spatial exponent dominates the linear drift exponent and the [polynomial](../../../../../../polynomial-split.md) at both infinities; all these [normal modes](../../../../../../normal-mode.md) are spatially bounded. The largest [growth rate](../../../../../../growth-rate.md) is $s_0$, so the least-node [normal mode](../../../../../../normal-mode.md) is temporally non-growing, and all [normal modes](../../../../../../normal-mode.md) are non-growing, when

$$
\boxed{\mu_0\leq\frac{U^2}{4\gamma}+\epsilon\sqrt{\nu\gamma}.}
$$

Equality is a neutral ground-state [normal mode](../../../../../../normal-mode.md); strict inequality gives decay. This proves the printed sufficient condition for a bounded stable global [normal mode](../../../../../../normal-mode.md) and identifies its stronger meaning: stability of the leading global [normal mode](../../../../../../normal-mode.md). Existence of merely some stable higher-$j$ [normal mode](../../../../../../normal-mode.md) is not equivalent to the inequality, since sufficiently large $j$ gives $s_j<0$ even above the leading-mode threshold. In the quadratic-coefficient model the reduction and [eigenvalues](../../../../../../eigenvalue.md) are exact, not just a first-order approximation to a more general profile.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
