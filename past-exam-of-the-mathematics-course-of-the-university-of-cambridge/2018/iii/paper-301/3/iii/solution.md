<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [Lorentz-invariant phase-space measure](../../../../../../lorentz-invariant-phase-space-measure.md) from the original PDF, including the $1/(2E_{p'})$ and $1/(2E_{q'})$ factors missing from the local TeX. In the [center of mass](../../../../../../center-of-mass.md) frame put $E=\sqrt s/2$ and $k=\sqrt{s-4m^2}/2$, assuming $s>4m^2$. The spatial [Dirac delta distribution](../../../../../../dirac-delta-function.md) sets $\mathbf q'=-\mathbf p'$, leaving

$$
d\Phi_2=\frac1{16\pi^2}\frac{k'^2\,dk'\,d\Omega}{E_{k'}^2}\,
\delta(\sqrt s-2E_{k'}).
$$

Since $d(2E_{k'})/dk'=2k'/E_{k'}$, the radial integral gives

$$
d\Phi_2=\frac{k}{16\pi^2\sqrt s}\,d\Omega
=\frac{\sqrt{1-4m^2/s}}{32\pi^2}\,d\Omega.
$$

The [invariant flux factor](../../../../../../invariant-flux-factor.md) is $2\sqrt{\kappa(s,m^2,m^2)}=2\sqrt{s(s-4m^2)}$, using the [Källén function](../../../../../../kallen-function.md). Dividing the phase space by this flux yields $d\sigma/d\Omega=|\mathcal M|^2/(64\pi^2s)$, with the final-state labels retained as in the printed formula.

Let $x=\cos\theta$. Of the [Mandelstam variables](../../../../../../mandelstam-variables.md), $t$ is

$$
t=-2k^2(1-x)=-\frac{s-4m^2}{2}(1-x),\qquad
\frac{dt}{dx}=\frac{s-4m^2}{2}.
$$

The azimuthal integral contributes $2\pi$, and the angular endpoints are therefore

$$
\boxed{t_{\min}=4m^2-s,\qquad t_{\max}=0.}
$$

Changing variables gives the requested expression from the formula supplied in the paper:

$$
\boxed{\sigma=\frac1{16\pi}\int_{4m^2-s}^{0}\frac{|\mathcal M|^2}{s(s-4m^2)}\,dt,
\qquad X=\frac1{16\pi},\quad Y=4.}
$$

There is a normalization qualification: the displayed starting formula integrates over labeled final momenta and contains no $1/2!$. For the physical cross-section of two indistinguishable outgoing quanta of this [real scalar field](../../../../../../real-scalar-field.md), the [identical-particle factor in a final-state phase-space integral](../../../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md) divides the full integral by two. With that convention $X=1/(32\pi)$; equivalently, integrate only one representative of each exchanged pair. The boxed value $1/(16\pi)$ follows the given formula exactly.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
