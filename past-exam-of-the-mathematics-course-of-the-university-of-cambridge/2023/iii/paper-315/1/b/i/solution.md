<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Along a ray, the [radiative transfer equation](../../../../../../../radiative-transfer-equation.md) has the [formal solution of the radiative transfer equation](../../../../../../../formal-solution-of-the-radiative-transfer-equation.md)

$$
I_{\nu,i}=I_{\nu,b}e^{-\tau_{\nu,i}/\mu}
+B_\nu(T_i)(1-e^{-\tau_{\nu,i}/\mu})
$$

for each isothermal region in [local thermodynamic equilibrium](../../../../../../../local-thermodynamic-equilibrium.md), neglecting scattering. For a self-luminous atmosphere with no incident intensity from below at the relevant photosphere, and in the optically thick limit, $I_{\nu,i}=B_\nu(T_i)$.

The observed [radiative flux](../../../../../../../radiative-flux.md) is the projected-disc integral

$$
F_{\nu,p}=\frac{2\pi R_p^2}{d^2}
\int_0^{\pi/2}I_\nu(\theta)\cos\theta\sin\theta\,d\theta.
$$

The inner region occupies projected fraction $f=\sin^2\theta_T$, hence

$$
\boxed{
F_{\nu,p}=\frac{\pi R_p^2}{d^2}
\left[
B_\nu(T_1)\sin^2\theta_T
+B_\nu(T_2)\cos^2\theta_T
\right]}.
$$

For finite optical depths, each [Planck law](../../../../../../../planck-s-law.md) function in this formula is replaced by its corresponding emergent intensity above.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
