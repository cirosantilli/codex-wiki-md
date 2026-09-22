<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let the belt contain $n(D)dD=CD^{-\alpha}dD$ bodies. Its total mass fixes

$$
\boxed{C=
\frac{6M(4-\alpha)}
{\pi\rho\left(D_{\max}^{4-\alpha}-D_{\min}^{4-\alpha}\right)}}
\simeq\frac{6M(4-\alpha)}{\pi\rho D_{\max}^{4-\alpha}}.
$$

For equal [mass density](../../../../../../density.md), an impactor of diameter $D$ supplies [specific impact energy](../../../../../../specific-impact-energy.md)

$$
Q=\frac12\left(\frac{D}{D_t}\right)^3v_{\rm rel}^2.
$$

Thus catastrophic disruption requires $D\geq D_{\rm cc}=X_cD_t$, where

$$
\boxed{X_c=\left(\frac{2Q_D^*}{v_{\rm rel}^2}\right)^{1/3}}.
$$

The impactor [number density](../../../../../../number-density.md) per diameter is $CD^{-\alpha}/V$. Neglecting [gravitational focusing](../../../../../../gravitational-focusing.md), the [geometric collision cross-section](../../../../../../geometric-collision-cross-section.md) is $\pi(D_t+D)^2/4$, so the exact [catastrophic planetesimal collision rate](../../../../../../catastrophic-planetesimal-collision-rate.md) in this model is

$$
\boxed{R_{\rm cc}(D_t)=
\frac{\pi Cv_{\rm rel}}{4V}
\int_{X_cD_t}^{D_{\max}}(D_t+D)^2D^{-\alpha}\,dD}.
$$

Equivalently, with $A=\pi Cv_{\rm rel}/(4V)$,

$$
R_{\rm cc}=A\left[
\frac{D^{3-\alpha}}{3-\alpha}
+\frac{2D_tD^{2-\alpha}}{2-\alpha}
+\frac{D_t^2D^{1-\alpha}}{1-\alpha}
\right]_{X_cD_t}^{D_{\max}}.
$$

If $D_{\min}\ll X_cD_t\ll D_t\ll D_{\max}$, the steep distribution makes impactors just above $X_cD_t$ dominate and their collision cross-section is approximately $\pi D_t^2/4$. Hence

$$
\boxed{R_{\rm cc}(D_t)\simeq
\frac{A}{\alpha-1}X_c^{1-\alpha}D_t^{3-\alpha}}.
$$

This approximation also assumes a common $v_{\rm rel}$ and size-independent [catastrophic disruption threshold](../../../../../../catastrophic-disruption-threshold.md) $Q_D^*$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
