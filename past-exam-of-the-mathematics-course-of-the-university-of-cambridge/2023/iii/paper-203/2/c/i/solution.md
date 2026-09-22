<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $x>0$, the [Chordal Loewner equation](../../../../../../../chordal-loewner-equation.md) and $U_t=\sqrt\kappa B_t$ give

$$
dV_t^x=\frac2{V_t^x}dt-\sqrt\kappa\,dB_t.
$$

Put $D_t=V_t^r-V_t^1$. The common Brownian term cancels, so

$$
dD_t=-\frac{2D_t}{V_t^rV_t^1}dt.
$$

The [Itô formula](../../../../../../../ito-s-lemma.md) applied to $Z_t=\log D_t-\log V_t^1$ gives

$$
dZ_t
=\frac{\sqrt\kappa}{V_t^1}dB_t
+\left[
\frac{\kappa-4}{2(V_t^1)^2}
-\frac2{V_t^rV_t^1}
\right]dt.
$$

Since

$$
\frac{V_t^1}{V_t^r}=\frac1{1+e^{Z_t}},
$$

the clock $q(u)=\int_0^u(V_s^1)^{-2}ds$ and its inverse $\sigma$ turn the local-martingale term into Brownian motion by the [Dambis-Dubins-Schwarz theorem](../../../../../../../dambis-dubins-schwarz-theorem.md). Therefore

$$
d\widetilde Z_t
=\sqrt\kappa\,dW_t
+\left(
\frac{\kappa-4}{2}
-\frac2{1+e^{\widetilde Z_t}}
\right)dt,
\qquad
\widetilde Z_0=\log(r-1).
$$

This is the [SLE boundary-point logarithmic separation diffusion](../../../../../../../sle-boundary-point-logarithmic-separation-diffusion.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
