<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The general solution contains both decay of the initial xenon and continued feeding from the initial iodine.** Use $t=0$ for removal of the flux, and retain $\phi$ as the pre-shutdown value in the initial conditions. Neglect post-shutdown [nuclear fission](../../../../../../nuclear-fission.md) and [neutron capture](../../../../../../neutron-capture.md). Then

$$
I(t)=I_0e^{-\lambda_It},
\qquad
\dot X+\lambda_XX=\lambda_II_0e^{-\lambda_It}.
$$

Multiply this [first-order linear differential equation](../../../../../../first-order-linear-differential-equation.md) by the [integrating factor](../../../../../../integrating-factor.md) $e^{\lambda_Xt}$ and integrate:

$$
\boxed{
X(t)=X_0e^{-\lambda_Xt}
+\frac{\lambda_II_0}{\lambda_X-\lambda_I}
\left(e^{-\lambda_It}-e^{-\lambda_Xt}\right).
}
$$

With the preceding steady initial conditions, $\lambda_II_0=G=\gamma_I\Sigma_f\phi$ and $X_0=G/(\lambda_X+\phi\sigma_{aX})$, this is

$$
X(t)=G\left[
\frac{e^{-\lambda_Xt}}{\lambda_X+\phi\sigma_{aX}}
+\frac{e^{-\lambda_It}-e^{-\lambda_Xt}}{\lambda_X-\lambda_I}
\right].
$$

If $\lambda_X+\phi\sigma_{aX}\gg|\lambda_X-\lambda_I|$, the coefficient of the first exponential term is small compared with the coefficients of the feeding term, yielding

$$
\boxed{
X(t)\simeq
\frac{\gamma_I\Sigma_f\phi}{\lambda_X-\lambda_I}
\left(e^{-\lambda_It}-e^{-\lambda_Xt}\right).
}
$$

This approximation neglects the finite initial xenon population and is consequently not a small relative error at $t=0$, where its value is zero while the exact $X_0$ is positive. The exact expression supplies the initial value and satisfies $\dot X(0)=G-\lambda_XX_0$. For equal [nuclear decay constants](../../../../../../nuclear-decay-constant.md), the continuous limit of the exact solution is $X(t)=(X_0+\lambda_II_0t)e^{-\lambda_It}$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Module NE1](../../../../paper-ne1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../../split.md)
7. [MPhil in nuclear energy course of the University of Cambridge](../../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
