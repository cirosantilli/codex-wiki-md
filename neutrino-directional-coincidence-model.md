# Neutrino directional-coincidence model

↑ **Parent:** [IceCube Neutrino Observatory](icecube-neutrino-observatory.md)

How much does a small directional uncertainty help? Consider an original idealized model: a source direction fixed in advance, uniform background directions over the full [sphere](sphere.md), and circular acceptance radius $\psi$. The accepted [solid angle](solid-angle.md) and single-event background [probability](probability.md) are

$$
\Omega(\psi)=\int_0^{2\pi}\!d\phi\int_0^\psi\sin\theta\,d\theta=2\pi(1-\cos\psi),\qquad
q(\psi)=\frac{\Omega}{4\pi}=\frac{1-\cos\psi}{2}.
$$

The derivation integrates the area element on a unit [sphere](sphere.md). For small $\psi$ in [radians](radian.md), $q\simeq\psi^2/4$: halving the radius quarters the accidental acceptance, to leading order. At $psi=0$ acceptance vanishes; at $\psi=\pi$ it covers the full [sphere](sphere.md). The [solid angle](solid-angle.md) has units of [steradians](steradian.md); $q$ is dimensionless.

For $0<\psi\leq\pi$, take a deliberately crude [point spread function](point-spread-function-split.md): stipulate that every signal direction lies uniformly inside that cap. The signal and background [probability density functions](probability-density-function.md) per [steradian](steradian.md) are $S=1/\Omega$ inside the cap and zero outside, and $B=1/(4\pi)$ everywhere. Both integrate to one. For an event inside the cap their [likelihood ratio](likelihood-ratio.md) is

$$
\frac{S}{B}=\frac1q.
$$

This ratio compares two specified directional models; it is not the [probability](probability.md) that the event came from the source. Such a [conditional probability](conditional-probability.md) would additionally require prior source odds and the other selection information. For fixed source fraction $f$ among selected events, a normalized [mixture distribution](mixture-distribution.md) has density $(1-f)B+fS$. For independent events the [likelihood](likelihood-function.md) is the product of those densities; its ratio to background alone is

$$
\Lambda(f)=\prod_i\left[1+f\left(\frac{S_i}{B_i}-1\right)\right].
$$

Outside-cap events contribute factors $1-f$ rather than being silently discarded. At $f=0$, $\Lambda=1$; for a full-sky cap, $S=B$ and every $f$ gives $\Lambda=1$. A directional model that cannot distinguish source from background carries no directional evidence.

<a id="image-chosen-angular-acceptance-directional-likelihood-and-repeated-background-opportunities"></a>
![](neutrino-angular-background-coincidence.png)

**[Figure 8](#image-chosen-angular-acceptance-directional-likelihood-and-repeated-background-opportunities). Chosen angular acceptance, directional likelihood and repeated background opportunities**. Original exact spherical-cap calculation and uniform-cap signal model. Radii and event counts are chosen illustrations, not IceCube angular resolutions or discovery data. The fixed source direction and independent uniform background assumptions are essential.

As an original numerical example, radii $1^\circ$ and $10^\circ$ give $q\simeq7.615\times10^{-5}$ and $7.596\times10^{-3}$, respectively: nearly a hundredfold difference. For a fixed number $N$ of independent background events, the [binomial distribution](binomial-distribution.md) gives

$$
P(\text{at least one inside})=1-(1-q)^N.
$$

With chosen $N=100$, those radii give approximately $0.00759$ and $0.5335$. A small single-event acceptance can become a common coincidence after many opportunities. This [probability](probability.md) concerns a fixed cap, rather than a scan for the most favorable cap anywhere. For $m$ independent searches with common local tail [probability](probability.md) $p$, the corresponding global tail [probability](probability.md) is $1-(1-p)^m$; overlapping sky searches generally violate that independence. Actual source tests must include directional response, nonuniform exposure, [energy](energy-split.md) information and the [look-elsewhere effect](look-elsewhere-effect.md) in their null calibration.

## ↑ Ancestors (6)

1. [IceCube Neutrino Observatory](icecube-neutrino-observatory.md)
2. [Cherenkov detector](cherenkov-detector.md)
3. [Particle detector](particle-detector.md)
4. [Particle detection](particle-detection-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
