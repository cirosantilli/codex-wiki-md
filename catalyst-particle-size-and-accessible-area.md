# Catalyst particle size and accessible area

↑ **Parent:** [Heterogeneous catalysis](heterogeneous-catalysis.md)

Consider an original geometric model of $N$ separate nonporous [solid](solid.md) [spheres](sphere.md), each with [radius](radius.md) $r$. Hold their total [volume](volume-thermodynamics.md) $V_s$ fixed. The [sphere](sphere.md) formulas give

$$
V_s=N\frac{4\pi r^3}{3},\qquad S=N4\pi r^2=\frac{3V_s}{r}.
$$

At fixed [mass density](density.md), fixed $V_s$ also means fixed total [mass](mass.md). Halving $r$ requires eight times as many particles and doubles their total external [surface area](surface-area.md) $S$; this follows by eliminating $N$, without any assumption about [chemical kinetics](chemical-kinetics-split.md).

For example, take one [sphere](sphere.md) of [radius](radius.md) $1.00\,\mathrm{mm}$, so $V_s=4\pi/3\,\mathrm{mm^3}$. Eight [spheres](sphere.md) of [radius](radius.md) $0.50\,\mathrm{mm}$ have the same $V_s$. Their total [surface areas](surface-area.md) are respectively $4\pi\,\mathrm{mm^2}$ and $8\pi\,\mathrm{mm^2}$, approximately $12.57$ and $25.13\,\mathrm{mm^2}$. Sixty-four particles of [radius](radius.md) $0.25\,\mathrm{mm}$ would instead give $16\pi\,\mathrm{mm^2}$, four times the original area.

<a id="image-catalyst-particle-size-and-area"></a>
![](catalyst-particle-size-and-area.png)

**[Figure 10](#image-catalyst-particle-size-and-area). Smaller separate catalyst particles expose more surface area at fixed total solid volume**. Original exact [sphere](sphere.md) model. The circles are particle silhouettes: one of [radius](radius.md) $r_0$ and eight of [radius](radius.md) $r_0/2$ represent equal three-dimensional [solid](solid.md) [volumes](volume.md), with twice the external [surface area](surface-area.md) in the second case. The right-hand curve is $S/S_0=r_0/r$, with the quarter-radius example marked too. It is a geometric prediction, not a measured [reaction rate](reaction-rate.md), a peroxide experiment, or a time series.

To obtain a kinetic prediction, add assumptions explicitly. Let $f$ be the accessible fraction of external [surface area](surface-area.md), $\sigma$ the [amount of substance](amount-of-substance.md) of [catalytic surface sites](catalytic-surface-site.md) per unit accessible area, and $\nu$ the mean number of completed conversions per site per unit time under the chosen conditions. Then the model's [reaction product](product-chemistry.md) formation rate is

$$
\frac{dn_{\mathrm B}}{dt}=\nu\sigma fS=\frac{3\nu\sigma fV_s}{r}.
$$

Here $\nu$ has units $\mathrm{s^{-1}}$ and $\sigma$ has units $\mathrm{mol\,m^{-2}}$, giving $\mathrm{mol\,s^{-1}}$ overall. Halving $r$ doubles this predicted rate only if $f$, $\sigma$ and $\nu$ remain unchanged. Particle contact can hide area; pores can add area; [diffusion](diffusion.md), altered surface structure and [catalyst deactivation](catalyst-deactivation.md) can change the other factors. Consequently, twice the calculated external area is not a universal promise of twice the measured [reaction rate](reaction-rate.md). The geometric argument changes contact, not the net [Gibbs free energy](gibbs-free-energy.md) or the [equilibrium constant](equilibrium-constant.md) of the same overall [chemical reaction](chemical-reaction-split.md).

## ↑ Ancestors (6)

1. [Heterogeneous catalysis](heterogeneous-catalysis.md)
2. [Catalysis](catalysis.md)
3. [Chemical kinetics](chemical-kinetics-split.md)
4. [Chemical reaction](chemical-reaction-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)
