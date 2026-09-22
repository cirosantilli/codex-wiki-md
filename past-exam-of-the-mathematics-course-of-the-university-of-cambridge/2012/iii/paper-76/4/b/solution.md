<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Retain the factor $\epsilon$ in the last temporal phase, as printed in the original PDF. Let $a=U/(2\gamma)$ and put $\eta=e^{ax}b(\xi)e^{st}$ with $s=-i\omega_0-i\epsilon\omega_1$. The [drift-removing substitution for a Dirichlet Sturm-Liouville problem](../../../../../../drift-removing-substitution-for-a-dirichlet-sturm-liouville-problem.md) cancels the first derivative:

$$
sb=\gamma b_{xx}+\left(\mu_0-\frac{U^2}{4\gamma}-\nu\epsilon^2x^2\right)b.
$$

With $\xi=\sqrt\epsilon f x$, this becomes

$$
b_{\xi\xi}+\left[\frac{\mu_0-U^2/(4\gamma)+i\omega_0+i\epsilon\omega_1}{\gamma\epsilon f^2}-\frac\nu{\gamma f^4}\xi^2\right]b=0.
$$

Choose the positive scale $f=(\nu/\gamma)^{1/4}$. To leave an order-one spectral parameter, cancel the numerator's order-one term. Then

$$
\boxed{\omega_0=i\left(\mu_0-\frac{U^2}{4\gamma}\right),\qquad f=(\nu/\gamma)^{1/4},\qquad\lambda=\frac{i\omega_1}{\sqrt{\gamma\nu}}.}
$$

The assumed decaying solutions of the [Hermite differential equation](../../../../../../hermite-differential-equation.md) require $\lambda=2j+1$, $j=0,1,\ldots$. They are proportional to $e^{-\xi^2/2}H_j(\xi)$, with physicists' [Hermite polynomials](../../../../../../hermite-polynomial.md). Therefore the [global modes of a quadratically confined Ginzburg-Landau equation](../../../../../../global-modes-of-a-quadratically-confined-ginzburg-landau-equation.md) have

$$
\boxed{\omega_1=-i(2j+1)\sqrt{\gamma\nu},\qquad s_j=\mu_0-\frac{U^2}{4\gamma}-\epsilon(2j+1)\sqrt{\gamma\nu}.}
$$

For every fixed positive $\epsilon$, multiplying the Hermite-Gaussian by $e^{Ux/(2\gamma)}$ still gives decay at both infinities. The strongest mode is $j=0$, so the whole-line system is **globally unstable precisely when**

$$
\boxed{\mu_0>\frac{U^2}{4\gamma}+\epsilon\sqrt{\gamma\nu}.}
$$

Equality is a neutral ground mode. This spectrum is exact for the stated quadratic profile, even though the notation organizes it as an expansion in $\epsilon$.

The homogeneous absolute-instability threshold in part (a) is $\mu=U^2/(4\gamma)$. The global threshold approaches that value as the profile varies increasingly slowly, but at finite $\epsilon$ the quadratic confinement adds the loss $\epsilon\sqrt{\gamma\nu}$. A locally absolutely unstable patch at the profile maximum is necessary but must be strong and broad enough to overcome that loss. Merely having positive local temporal growth $\mu_0>0$, which can be only [convective wave-packet instability](../../../../../../convective-wave-packet-instability.md), is insufficient for a growing decaying global [normal mode](../../../../../../normal-mode.md). This connects the local impulse classification to the discrete global spectrum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
