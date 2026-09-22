<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the notation $I_\nu(\mu,\tau)$ throughout, with optical depth increasing inward and $0<\mu\leq1$ for an outward ray. This removes the change in argument order used in the printed surface-intensity notation. Multiplying the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) by its integrating factor gives

$$
\frac{d}{d\tau}\left(I_\nu e^{-\tau/\mu}\right)=-\frac{S_\nu(\tau)}\mu e^{-\tau/\mu}.
$$

Integrating from the surface to a deeper boundary $b$ yields

$$
I_\nu(\mu,0)=I_\nu(\mu,b)e^{-b/\mu}+\frac1\mu\int_0^b S_\nu(t)e^{-t/\mu}\,dt.
$$

For a semi-infinite atmosphere with no exponentially growing homogeneous term, the boundary term vanishes as $b\to\infty$. The [formal solution of the radiative transfer equation](../../../../../../formal-solution-of-the-radiative-transfer-equation.md) is therefore

$$
I_\nu(\mu,0)=\int_0^\infty S_\nu(t)e^{-t/\mu}\frac{dt}{\mu}.
$$

The usual deep-atmosphere boundary condition is necessary; a first-order differential equation alone does not fix the emerging [specific intensity](../../../../../../specific-intensity.md).

For a linear [source function](../../../../../../radiative-transfer-source-function.md), the zeroth and first exponential moments give **$I_\nu(\mu,0)=a_0+a_1\mu$**. Equivalently $I_\nu(\mu,0)=S_\nu(\tau=\mu)$, the [Eddington-Barbier relation](../../../../../../eddington-barbier-relation.md). If the source rises inward, rays near the limb sample cooler, shallower layers, producing [limb darkening](../../../../../../limb-darkening.md).

For the finite polynomial, put $u=t/\mu$ and integrate each term. Repeated integration by parts gives $\int_0^\infty u^je^{-u}\,du=j!$, so the [polynomial source function moments for emergent intensity](../../../../../../polynomial-source-function-moments-for-emergent-intensity.md) give

$$
\boxed{I_\nu(\mu,0)=\sum_{j=0}^n j!a_j\mu^j,\qquad A_j=j!a_j.}
$$

The limiting grazing-ray [specific intensity](../../../../../../specific-intensity.md) is $a_0$. If the displayed polynomial is only a local Taylor approximation to a more general source, this formula applies to that approximation and a source-function remainder also contributes; a finite local expansion is not automatically an exact description at every optical depth.

For a constant source in an overlying layer of optical thickness $\tau$, the radial ray has the exact transfer relation

$$
I_\nu(1,0)=I_\nu(1,\tau)e^{-\tau}+S_\nu(1-e^{-\tau}).
$$

Expanding the exponentials gives the [constant source transfer through a thin layer](../../../../../../constant-source-transfer-through-a-thin-layer.md):

$$
\boxed{I_\nu(1,0)=I_\nu(1,\tau)+[S_\nu-I_\nu(1,\tau)]\tau+O(\tau^2).}
$$

This finite-layer result does not require the [specific intensity](../../../../../../specific-intensity.md) below the layer to equal its source function. The sign of $S_\nu-I_\nu(1,\tau)$ already distinguishes emission from absorption.

An [absorption line](../../../../../../absorption-line.md) forms when a bound-bound transition increases [opacity](../../../../../../opacity.md) at selected frequencies. In a photosphere whose [temperature](../../../../../../temperature.md) decreases outward, optical depth of order one at the line frequency occurs higher than at a nearby continuum frequency. In an absorption-dominated region in [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md), the source is the [Planck function](../../../../../../planck-function.md); the cooler line-forming layer then emits less [specific intensity](../../../../../../specific-intensity.md) than the deeper continuum-forming layer. The result is a dark spectral feature. Scattering and departures from LTE modify the source, so this temperature-gradient picture is a useful mechanism rather than a universal identity for every line.

Two distinct situations can produce [emission lines](../../../../../../emission-line.md). First, a heated [chromosphere](../../../../../../chromosphere.md) has an outward [temperature](../../../../../../temperature.md) rise, so an optically thick line can sample gas hotter than the continuum photosphere beneath it. Secondly, a hot optically thin circumstellar envelope or [stellar wind](../../../../../../stellar-wind.md) emits line photons through collisional excitation or recombination, with no comparably bright background along all rays; its added line flux can exceed the underlying continuum. Winds of hot luminous stars can also give a mixture of emission and absorption across a Doppler-broadened line profile. These examples explain the change in [specific intensity](../../../../../../specific-intensity.md) through either an enhanced source function or additional emitting material. 

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
