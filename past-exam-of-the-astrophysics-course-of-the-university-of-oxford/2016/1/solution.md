<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Inverse Compton scattering](../../../inverse-compton-scattering.md) transfers [energy](../../../energy-split.md) from fast [electrons](../../../electron.md) to lower-[energy](../../../energy-split.md) [photons](../../../photon.md). In the [Thomson scattering](../../../thomson-scattering.md) limit the scattering is approximately elastic in the [electron](../../../electron.md)'s instantaneous rest frame, but the transformations into and out of that frame can greatly increase the [photon](../../../photon.md) [energy](../../../energy-split.md) in the original frame.

In a [blazar](../../../blazar.md), relativistic jet [electrons](../../../electron.md) can scatter their own [synchrotron radiation](../../../synchrotron-radiation.md), producing [synchrotron self-Compton radiation](../../../synchrotron-self-compton-radiation.md), or scatter [photons](../../../photon.md) from an [accretion disk](../../../accretion-disk.md) and its surrounding reprocessing material. The two spectral humps constrain [electron](../../../electron.md) [Lorentz factors](../../../lorentz-factor.md), the [electron](../../../electron.md) distribution and, with assumptions about geometry and relativistic beaming, the [magnetic field](../../../magnetic-field-split.md). For the same [electron](../../../electron.md) population in the Thomson regime, the ratio of inverse-Compton to synchrotron power scales as $u_{\rm ph}/u_B$ in the plasma rest frame. It does not determine the field without information about the [photon energy density](../../../photon-energy-density.md) and beaming.

In a [galaxy cluster](../../../galaxy-cluster.md), hot thermal [electrons](../../../electron.md) scatter [cosmic microwave background](../../../cosmic-microwave-background-split.md) [photons](../../../photon.md) and slightly raise their mean [energy](../../../energy-split.md), producing the [thermal Sunyaev-Zeldovich effect](../../../thermal-sunyaev-zeldovich-effect.md). The spectral distortion measures the line-of-sight integral of [electron](../../../electron.md) [pressure](../../../pressure-split.md), approximately $y=\sigma_T\int n_ek_BT_e\,d\ell/(m_ec^2)$ for nonrelativistic thermal [electrons](../../../electron.md). Combined with X-ray emission, which weights density approximately quadratically, it constrains the gas density, [temperature](../../../temperature-split.md) and [mass](../../../mass.md) distribution. These are distinct source populations and seed [photon](../../../photon.md) fields from the blazar example.

For the power derivation, use an isotropic incident radiation field of **total [photon energy density](../../../photon-energy-density.md)** $u_{\rm ph}$ in the laboratory frame. Its [stress-energy tensor](../../../stress-energy-tensor-split.md) has $T^{00}=u_{\rm ph}$ and $T^{zz}=u_{\rm ph}/3$, with zero mean flux. Boosting to an [electron](../../../electron.md) moving at $\beta c$ along $z$ gives

$$
T'^{0z}=-\gamma^2\beta(T^{00}+T^{zz})=-\frac43\gamma^2\beta u_{\rm ph}.
$$

The radiation [energy flux](../../../energy-flux.md) in this rest frame is $S'_z=cT'^{0z}$. Elastic [Thomson scattering](../../../thomson-scattering.md) exerts the drag $F'_z=\sigma_TS'_z/c$. The parallel three-force has the same value in the laboratory frame, so the [electron](../../../electron.md)'s positive [energy](../../../energy-split.md) loss rate is

$$
\boxed{P_{\rm IC}=-F_z\beta c=\frac43\sigma_Tc\,u_{\rm ph}\beta^2\gamma^2.}
$$

This [isotropic inverse-Compton drag](../../../isotropic-inverse-compton-drag.md) assumes [photon](../../../photon.md) [energies](../../../energy-split.md) small compared with $m_ec^2$ in the [electron](../../../electron.md) rest frame, negligible recoil and an isotropic seed field in the specified frame. An anisotropic [photon](../../../photon.md) field requires its directional moments; the recoil-dependent [differential scattering cross-section](../../../differential-scattering-cross-section.md) of [Compton scattering](../../../compton-scattering.md) becomes necessary at larger rest-frame [energies](../../../energy-split.md).

There are two conventions to qualify in the printed expression. First, the density multiplying $4/3$ must be $u_{\rm ph}$, not literally only the magnetic part of a propagating electromagnetic field. That field has equal electric and magnetic [energy](../../../energy-split.md) densities, so $u_{\rm ph}=2u_{\rm mag}$ and the corresponding formula is $P_{\rm IC}=(8/3)\sigma_Tcu_{\rm mag}\beta^2\gamma^2$. Second, this is net [electron](../../../electron.md) [energy](../../../energy-split.md) loss, rather than all incident plus scattered [photon](../../../photon.md) [energy](../../../energy-split.md). At $\beta=0$ an [electron](../../../electron.md) still scatters power $\sigma_Tcu_{\rm ph}$, but transfers no kinetic [energy](../../../energy-split.md) to the [photons](../../../photon.md), so the inverse-Compton gain is zero.

For an individual incident [photon](../../../photon.md) of [energy](../../../energy-split.md) $\varepsilon$, the [electron](../../../electron.md)-frame [energy](../../../energy-split.md) is $\varepsilon'=\gamma\varepsilon(1-\beta\cos\theta)$. For a head-on [photon](../../../photon.md) followed by forward emission in the laboratory,

$$
\varepsilon_{\rm out}\simeq\gamma^2(1+\beta)^2\varepsilon\simeq4\gamma^2\varepsilon.
$$

Averaging an isotropic seed field gives $\langle\varepsilon_{\rm out}\rangle\simeq(4/3)\gamma^2\varepsilon$ for ultrarelativistic [electrons](../../../electron.md). The original plot has an inverse-Compton maximum of order $10^8\,\mathrm{eV}$, a synchrotron maximum around $10^{-1}\,\mathrm{eV}$ and a disk component around $1\,\mathrm{eV}$. Thus

$$
\boxed{\gamma\sim\sqrt{\frac{3\varepsilon_{\rm out}}{4\varepsilon_{\rm seed}}}\sim9\times10^3\ \hbox{to}\ 3\times10^4.}
$$

The head-on maximum gives the same order of magnitude, about $5\times10^3$ to $1.6\times10^4$. These are approximate readings of a broad spectrum, not precise fitted parameters. Disk and synchrotron seed [photons](../../../photon.md) need not be scattered by the same part of the [electron](../../../electron.md) distribution, and bulk jet Doppler factors also enter the observed peak relation. The indicated rest-frame seed [energies](../../../energy-split.md) remain well below the [electron](../../../electron.md) rest [energy](../../../energy-split.md) in this estimate.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2016](../../2016-split.md)
3. [Past exam of the astrophysics course of the University of Oxford](../../split.md)
4. [Astrophysics course of the University of Oxford](../../../astrophysics-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
