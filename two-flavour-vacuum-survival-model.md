# Two-flavour vacuum survival model

↑ **Parent:** [Super-Kamiokande atmospheric-neutrino experiment](super-kamiokande-atmospheric-neutrino-experiment.md)

For a deliberately simplified [neutrino oscillation](neutrino-oscillation.md) calculation, take two [neutrino flavors](neutrino-flavor.md) related to two [mass eigenstates](mass-eigenstate.md) by a real [rotation matrix](rotation-matrix.md) with angle $\theta$. A [quantum superposition](quantum-superposition.md) acquires different phases during propagation; projecting back onto the initial [neutrino flavor](neutrino-flavor.md) gives the [probability](probability.md)

$$
P_{\mu\mu}=1-\sin^2(2\theta)\sin^2\!\left(1.27\frac{\Delta m^2}{\mathrm{eV}^2}\frac{L}{\mathrm{km}}\frac{\mathrm{GeV}}{E}\right),\qquad \Delta m^2=m_2^2-m_1^2.
$$

Here $L$ is path [length](length.md) and $E$ is [neutrino](neutrino.md) [energy](energy-split.md); the numerical coefficient incorporates unit conversion.

The paper states the corresponding conversion formula.[PDF p. 2, Eq. (1)](evidence-for-oscillation-of-atmospheric-neutrinos-by-y-fukuda-and-others.md)

The path dependence has a geometrical origin. In an original spherical-[Earth](earth.md) model, let $R$ be the radius and $h$ a fixed production height, neglecting detector depth. Let $\Theta$ be the [zenith distance](zenith-distance.md) of the direction in the sky from which the [neutrino](neutrino.md) arrives, so $c=\cos\Theta=+1$ means downward propagation. The backward ray from detector to production obeys $R^2+L^2+2RLc=(R+h)^2$. Its positive solution is

$$
L(c)=-Rc+\sqrt{(R+h)^2-R^2(1-c^2)}.
$$

Thus $L(+1)=h$ and $L(-1)=2R+h$. The calculation explains why opposite directions test very different baselines, rather than attributing every observed direction to the same travel distance. Actual production heights and the angle between the outgoing [charged lepton](charged-lepton.md) and incoming [neutrino](neutrino.md) smear that relationship.

For an original chosen example, set $\theta=\pi/4$ and $\Delta m^2=2.5\times10^{-3}\,\mathrm{eV}^2$. At $E=1\,\mathrm{GeV}$, $L=20\,\mathrm{km}$ gives $P_{\mu\mu}\simeq0.9960$, while $L=500\,\mathrm{km}$ gives $P_{\mu\mu}\simeq0.000279$. The first minimum is at $L/E\simeq494.7\,\mathrm{km/GeV}$. These are stipulated inputs, not a fit to the 1998 data. A broad distribution of true $L/E$, together with [energy](energy-split.md) and directional uncertainty, smooths the sharp minima.

A direct amplitude check makes the mechanism explicit. Define

$$
U=\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix},\qquad
S=U\begin{pmatrix}1&0\\0&e^{-2i\varphi}\end{pmatrix}U^T,
\qquad \varphi=1.27\frac{\Delta m^2}{\mathrm{eV}^2}\frac{L}{\mathrm{km}}\frac{\mathrm{GeV}}{E}.
$$

Then $S_{11}=\cos^2\theta+\sin^2\theta e^{-2i\varphi}$. Taking its squared [absolute value](absolute-value.md) yields the displayed survival formula because $1-\cos(2\varphi)=2\sin^2\varphi$. [Unitarity](unitary-operator.md) gives $|S_{11}|^2+|S_{21}|^2=1$: disappearance from one channel becomes conversion to the other within this closed model.

This illustration does not describe all [solar neutrino](solar-neutrino.md) propagation. Coherent forward scattering in matter changes the effective propagation operator, and three active [neutrino flavors](neutrino-flavor.md) require a larger mixing description. Even in the simplified model, [neutrino oscillation](neutrino-oscillation.md) measures a squared-[mass](mass.md) difference; it does not determine the absolute [neutrino mass](neutrino-mass.md).

## ↑ Ancestors (8)

1. [Super-Kamiokande atmospheric-neutrino experiment](super-kamiokande-atmospheric-neutrino-experiment.md)
2. [Super-Kamiokande](super-kamiokande.md)
3. [Kajita-McDonald neutrino flavor-conversion experiments](kajita-mcdonald-neutrino-flavor-conversion-experiments.md)
4. [Cherenkov detector](cherenkov-detector.md)
5. [Particle detector](particle-detector.md)
6. [Particle detection](particle-detection-split.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Neutrino oscillation](neutrino-oscillation.md)
