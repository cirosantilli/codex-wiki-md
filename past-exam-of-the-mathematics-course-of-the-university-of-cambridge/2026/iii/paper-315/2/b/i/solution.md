<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\tau_1$ and $\tau_2$ be the top-down optical depths at $P_1$ and $P_2$, and let $\mu$ be the outward direction cosine. The [formal solution of the radiative transfer equation](../../../../../../../formal-solution-of-the-radiative-transfer-equation.md) gives

$$
\boxed{
I_\nu(0,\mu)
=B_\nu(T_1)(1-e^{-\tau_1/\mu})
+B_\nu(T_2)(e^{-\tau_1/\mu}-e^{-\tau_2/\mu})
+I_{\nu,0}e^{-\tau_2/\mu}}.
$$

For a semi-infinite lower layer in [local thermodynamic equilibrium](../../../../../../../local-thermodynamic-equilibrium.md), $I_{\nu,0}=B_\nu(T_3)$.

Define

$$
E_3(x)=\int_0^1\mu e^{-x/\mu}\,d\mu.
$$

The emergent planetary surface flux is

$$
F_{p,\nu}=2\pi\left[
B_1\left(\frac12-E_3(\tau_1)\right)
+B_2(E_3(\tau_1)-E_3(\tau_2))
+B_3E_3(\tau_2)\right].
$$

Hence the band-centre planet-star ratio is

$$
\boxed{
\frac{F_p}{F_*}
=\left(\frac{R_p}{R_*}\right)^2
\frac{2[B_1(1/2-E_3(\tau_1))
+B_2(E_3(\tau_1)-E_3(\tau_2))+B_3E_3(\tau_2)]}
{B_\nu(T_*)}}.
$$

If $T_1=T_2=T_3=T_p$, the weights telescope to $1/2$, so $F_{p,\nu}=\pi B_\nu(T_p)$ and the expression reduces to the blackbody [thermal eclipse depth](../../../../../../../thermal-eclipse-depth.md), about $72\,\mathrm{ppm}$ for $T_p=600\,\mathrm K$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
