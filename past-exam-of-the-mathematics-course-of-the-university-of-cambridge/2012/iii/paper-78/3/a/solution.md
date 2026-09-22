<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [scattering potential](../../../../../../scattering-potential.md) convention $V=k_0^2(n^2-1)$. With time dependence $e^{-i\omega t}$ the outgoing [Green function](../../../../../../green-s-function.md) is $G_0(r,r')=e^{ik_0|r-r'|}/(4\pi|r-r'|)$ and satisfies $(\Delta+k_0^2)G_0=-\delta$. The total-field [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md) is

$$
\psi(r)=\psi_0(r)+\int_DG_0(r,r')V(r')\psi(r')\,d^3r'.
$$

Replacing the field in the integral by the incident field gives the first [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md):

$$
\boxed{\psi_B=\psi_0+\psi_1,\qquad \psi_1(r)=\int_DG_0(r,r')V(r')\psi_0(r')\,d^3r'.}
$$

For the first [Rytov approximation](../../../../../../rytov-approximation.md), write $\psi=\psi_0e^\chi$ on a region where the incident field is nonzero and a continuous [complex logarithm](../../../../../../complex-logarithm.md) can be chosen. The [logarithmic wave perturbation](../../../../../../logarithmic-wave-perturbation.md) equation is

$$
\Delta\chi+2\nabla\log\psi_0\cdot\nabla\chi+\nabla\chi\cdot\nabla\chi=-V.
$$

The last dot product is bilinear, not a squared modulus. Dropping it leaves a linear equation for $\chi_1$. Multiplication by $\psi_0$ shows that $\psi_0\chi_1$ satisfies the same outgoing inhomogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md) as $\psi_1$. Hence

$$
\boxed{\chi_1=\frac{\psi_1}{\psi_0},\qquad \psi_R=\psi_0\exp\left(\frac{\psi_1}{\psi_0}\right).}
$$

Introduce a small multiplier $\lambda$ on $V$. Then $\psi_1=O(\lambda)$ and

$$
\psi_R=\psi_0+\psi_1+\frac{\psi_1^2}{2\psi_0}+O(\lambda^3)=\psi_B+O(\lambda^2).
$$

**The two total-field approximations agree to first order.** Exponentiating the first [logarithmic wave perturbation](../../../../../../logarithmic-wave-perturbation.md) does not supply the generally missing second-order [Born series](../../../../../../born-series.md) contribution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
