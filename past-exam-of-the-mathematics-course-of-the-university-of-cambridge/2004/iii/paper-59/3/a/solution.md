<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the comoving [cold dark matter](../../../../../../cold-dark-matter.md) choice $\mathbf v_C=0$ in [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md). Its continuity equation gives $\delta_C'=-h'/2$. Substituting $h'=-2\delta_C'$ and $h''=-2\delta_C''$ into the [metric tensor](../../../../../../metric-tensor.md) equation yields

$$
\boxed{\delta_C''+\mathcal H\delta_C'
-\frac32\mathcal H^2(\Omega_C\delta_C+2\Omega_R\delta_R)=0.}
$$

For radiation, put $\vartheta_R=i\mathbf k\cdot\mathbf v_R$. The continuity and Euler equations become $\delta_R'=-(4/3)\vartheta_R-(2/3)h'$ and $\vartheta_R'=k^2\delta_R/4$. Differentiating the first and eliminating the other two variables gives

$$
\boxed{\delta_R''+\frac{k^2}{3}\delta_R-\frac43\delta_C''=0.}
$$

The radiation [sound speed](../../../../../../speed-of-sound.md) is $1/\sqrt3$.

During [radiation domination](../../../../../../radiation-domination.md), $a\propto\tau$, $\mathcal H=1/\tau$ and $\Omega_R\simeq1$. Outside the horizon, $k\tau\ll1$, the [gradient](../../../../../../gradient.md) term is negligible. The regular initially adiabatic mode has $\delta_R=(4/3)\delta_C$ to leading order. Consequently

$$
\delta_C''+\frac1\tau\delta_C'-\frac4{\tau^2}\delta_C=0,
$$

with powers $\tau^2$ and $\tau^{-2}$. Keeping the regular growing branch gives

$$
\boxed{\delta_C\simeq A(k)\tau^2,\qquad
\delta_R\simeq\frac43A(k)\tau^2\quad(k\tau\ll1).}
$$

The superhorizon [density contrasts](../../../../../../density-contrast.md) here are in the specified comoving [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md); [density contrast](../../../../../../density-contrast.md) is not a gauge-independent superhorizon observable.

Deep inside the horizon, still before equality, radiation pressure produces bounded acoustic oscillations at frequency $\omega=k/\sqrt3$. The leading form is

$$
\delta_R\simeq B_1(k)\cos(\omega\tau)+B_2(k)\sin(\omega\tau),
\qquad
\delta_C\simeq C_1(k)+C_2(k)\log(k\tau).
$$

To see the logarithmic growth, average the rapidly oscillating radiation forcing in the [Cold dark matter](../../../../../../cold-dark-matter.md) equation and neglect the small matter self-gravity term; the remaining equation is $(\tau\delta_C')'\simeq0$. Radiation does not have a secular growing acoustic amplitude in this approximation. Its source $(4/3)\delta_C''$ supplies only a smaller slowly varying response, asymptotically $-4C_2/(k^2\tau^2)$, while the radiation oscillations induce suppressed oscillatory corrections to [Cold dark matter](../../../../../../cold-dark-matter.md).

The matching can be made explicit in the leading $\Omega_R=1$ system. Put $x=k\tau/\sqrt3$ and define

$$
F(x)=\int_0^x\frac{1-\cos z}{z}\,dz+\frac{\sin x}{x}
-\frac{1-\cos x}{x^2}-\frac12.
$$

Eliminating radiation gives $x^2F^{(4)}+5xF^{(3)}+x^2F''+xF'=0$. Direct differentiation verifies that the regular adiabatic solution is

$$
\delta_C=K F(x),\qquad
\delta_R=\frac K3\left[-2\cos x+\frac{4\sin x}{x}-\frac{4(1-\cos x)}{x^2}\right],
\qquad K=\frac{24A(k)}{k^2}.
$$

Indeed $F(x)\sim x^2/8$ at zero, and the radiation bracket is $x^2/2+O(x^4)$, recovering the early amplitudes. At infinity, $F(x)=\log x+\gamma_E-1/2+O(x^{-2})$ and $\delta_R=-(2K/3)\cos x+O(x^{-1})$. This [adiabatic radiation-era cold-dark-matter transfer solution](../../../../../../adiabatic-radiation-era-cold-dark-matter-transfer-solution.md) fixes the logarithmic coefficient and leading acoustic phase rather than leaving matching arbitrary.

The constants and acoustic phase are fixed by matching through horizon entry, not by imposing the early adiabatic relation at every later time. Since entry occurs at $\tau_h\sim k^{-1}$, their amplitude scale is set by $A(k)/k^2$. This is the [Mészáros effect](../../../../../../meszaros-effect.md): logarithmic subhorizon [Cold dark matter](../../../../../../cold-dark-matter.md) growth accompanies radiation oscillations until matter becomes dynamically important. Factors such as $2\pi$ in defining a wavelength do not change the two asymptotic regimes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
