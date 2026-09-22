<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\Gamma=-\dot\tau>0$. The [tight-coupling approximation](../../../../../../tight-coupling-approximation.md) requires $\Gamma\gg k,\mathcal H$: frequent [Thomson scattering](../../../../../../thomson-scattering.md) makes the [photon-baryon velocity slip](../../../../../../photon-baryon-velocity-slip.md) small and suppresses higher multipoles. Work with constant $R$ on the short scales of the question.

Set $s=v_\gamma-v_b$ and $A=k\Theta_0-2k\Theta_2/5$. The dipole and baryon equations imply

$$
\dot s=-A+\dot\tau(1+R^{-1})s,
\qquad
(1+R)\dot\Theta_1-A=-R\dot s.
$$

To leading order, $s=RA/[(1+R)\dot\tau]$. Differentiating this and keeping the first correction in $k/\Gamma$ yields

$$
\boxed{(1+R)\dot\Theta_1+\frac{2k}{5}\Theta_2-k\Theta_0
\simeq-\frac{R^2}{1+R}\frac{k}{\dot\tau}\dot\Theta_0}.
$$

Terms involving derivatives of $\Theta_2$ contribute at the next order here.

The leading $\ell=2$ polarization balance is

$$
0\simeq\dot\tau\left[\frac25E_2+\frac{3}{5\sqrt6}\Theta_2\right],
\qquad E_2=-\frac{\sqrt6}{4}\Theta_2.
$$

The $\ell=2$ temperature equation then becomes

$$
-\frac{2k}{3}\Theta_1
\simeq\dot\tau\left[\frac9{10}\Theta_2+\frac{\sqrt6}{10}E_2\right]
=\frac34\dot\tau\Theta_2,
$$

so the [photon quadrupole in tight coupling with polarization](../../../../../../photon-quadrupole-in-tight-coupling-with-polarization.md) is

$$
\boxed{\Theta_2\simeq-\frac89\frac{k}{\dot\tau}\Theta_1}.
$$

Finally substitute $\Theta_1=-3\dot\Theta_0/k$ into the corrected dipole equation. This gives the [photon-baryon diffusion damping equation](../../../../../../photon-baryon-diffusion-damping-equation.md)

$$
\boxed{\ddot\Theta_0+
\frac{k^2|\dot\tau^{-1}|}{3(1+R)}
\left(\frac{R^2}{1+R}+\frac{16}{15}\right)\dot\Theta_0+
\frac{k^2}{3(1+R)}\Theta_0\simeq0}.
$$

The oscillation frequency agrees with the [photon-baryon sound speed](../../../../../../photon-baryon-sound-speed.md). The positive damping coefficient comes from velocity slip and shear viscosity. Its growth as $k^2$ suppresses small-scale oscillations, producing the [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) tail and reducing the high-multipole [Cosmic microwave background acoustic peaks](../../../../../../cosmic-microwave-background-acoustic-peak.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
