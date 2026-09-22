<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the [optical depth](../../../../../../optical-depth.md) to increase inward and let $\mu>0$ denote an outward ray. For thermal absorption and emission in [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md), the [radiative transfer source function](../../../../../../radiative-transfer-source-function.md) is the [Planck function](../../../../../../planck-function.md), so the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) is

$$
\mu\frac{dI_\lambda}{d\tau}=I_\lambda-B_\lambda[T(\tau)].
$$

This assumes negligible scattering, or a source function genuinely thermalized to $B_\lambda$; LTE by itself does not turn an arbitrary scattering source into a [Planck function](../../../../../../planck-function.md). Multiply by $e^{-\tau/\mu}$, integrate between the two boundaries, and solve for the outward [specific intensity](../../../../../../specific-intensity.md):

$$
\boxed{I_\lambda(\tau_2,\mu)=I_\lambda(\tau_1,\mu)e^{-(\tau_1-\tau_2)/\mu}+\int_{\tau_2}^{\tau_1}\frac{B_\lambda[T(\tau)]}{\mu}e^{-(\tau-\tau_2)/\mu}\,d\tau.}
$$

The bottom boundary value is the quantity denoted $I_\lambda(0)$ in the supplied notation; it is not an optical-depth-zero boundary. The first term is attenuated incident radiation, and the second is emission from the intervening layers. This is the [formal solution of the radiative transfer equation](../../../../../../formal-solution-of-the-radiative-transfer-equation.md).

For an [isothermal atmosphere](../../../../../../isothermal-atmosphere.md) at temperature $T$, the [Planck function](../../../../../../planck-function.md) is constant and the integral can be evaluated:

$$
I_\lambda(\tau_2,\mu)=B_\lambda(T)+[I_\lambda(\tau_1,\mu)-B_\lambda(T)]e^{-(\tau_1-\tau_2)/\mu}.
$$

For a bounded bottom intensity and $\tau_1\to\infty$, **$I_\lambda=B_\lambda(T)$ in every outgoing direction, and $F_\lambda=\pi B_\lambda(T)$**. Thus the emergent spectrum is a [blackbody](../../../../../../blackbody.md) spectrum. The [blackbody limit of an isothermal atmosphere](../../../../../../blackbody-limit-of-an-isothermal-atmosphere.md) does not require a temperature gradient: it follows from complete thermalization in an optically thick medium.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
