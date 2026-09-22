<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $z$ upward from the unperturbed interface in the apparatus frame, with liquid at $z>0$ and pulling [velocity](../../../../../velocity.md) $-V\mathbf e_z$. The primary [ice](../../../../../ice.md) contains no salt. We use the dilute, equal-density approximation and neglect fluid motion relative to the mould. The initial salt inventory per unit horizontal area, with a common density factor suppressed, is $N=hC_0$. Its conservation is essential: the far liquid has zero [concentration](../../../../../concentration.md), so an imposed nonzero far-field composition would describe a different experiment.

The steady [advection-diffusion equation](../../../../../advection-diffusion-equation.md) is $-VC'=DC''$. Decay into the pure [water](../../../../../water.md) and interfacial [salt rejection](../../../../../salt-rejection.md) give

$$
C(z)=C_Ie^{-Vz/D},\qquad DC'(0)+VC_I=0.
$$

Since $\int_0^\infty C(z)\,dz=DC_I/V=N$, the [finite-inventory directional salt rejection](../../../../../finite-inventory-directional-salt-rejection.md) solution is

$$
\boxed{C(z)=\frac{VhC_0}{D}e^{-Vz/D}\quad(z>0),\qquad C=0\quad\text{in the primary ice}.}
$$

The decay length is $D/V$. Local [liquidus](../../../../../liquidus.md) equilibrium gives

$$
\boxed{T_I=-m\frac{VhC_0}{D}.}
$$

Thus the thermal apparatus selects the interface position at this isotherm. The stated speed inequality is precisely $C_I<C_E$, so the interface is warmer than the [eutectic temperature](../../../../../eutectic-temperature.md), $T_I>T_E=-mC_E$. These are steady values after the initial finite saline layer has rearranged; the final exponential distribution is not confined to the original depth $h$.

For $VhC_0/D>C_E$, a steady pure-[ice](../../../../../ice.md) front would require an interfacial composition beyond the [eutectic composition](../../../../../eutectic-composition.md). That branch is unavailable. During the transient, rejected brine concentrates until it reaches $C_E$; secondary salt-bearing crystals can then form and the residual brine freezes as an [eutectic system](../../../../../eutectic-system.md). Salt is incorporated into the product rather than remaining indefinitely in a super-eutectic exponential layer. The detailed pattern can include brine pockets and a nonplanar [freezing](../../../../../freezing.md) region; it depends on the thermal history and the morphological stability. The speed inequality alone does not decide that latter stability.

For the stability calculation use an interface displacement $\eta=\widehat\eta e^{ikx+st}$ and a liquid perturbation $c=\widehat c e^{ikx+st-qz}$. Here $k>0$ is the [wavenumber](../../../../../wavenumber.md), $s$ is the temporal rate and $\Re q>0$ gives spatial decay. The frozen thermal field is $T_I+Gz$. Define $\Gamma=\gamma_{sl}T_m/(\rho L)>0$, where $\gamma_{sl}$ is [solid-liquid surface energy](../../../../../solid-liquid-surface-energy.md), $T_m$ is absolute pure-solvent [melting](../../../../../melting.md) [temperature](../../../../../temperature.md), $\rho$ is [mass density](../../../../../density.md) and $L$ is specific [latent heat](../../../../../latent-heat.md). For a solid protrusion into liquid the [curvature](../../../../../curvature.md) is $\mathcal K=-\eta_{xx}=k^2\eta$, and the [Gibbs-Thomson effect](../../../../../gibbs-thomson-relation.md) gives local equilibrium $T=-mC-\Gamma\mathcal K$. We assume isotropic surface energy and [instantaneous interface kinetics](../../../../../instantaneous-interface-kinetics.md), so no [kinetic undercooling](../../../../../kinetic-undercooling.md) term is present.

Linearizing the equilibrium condition at the displaced interface gives

$$
G\eta=-m[c(0)+\eta C'(0)]-\Gamma k^2\eta,
\qquad
\widehat c=\left[\frac{VC_I}{D}-\frac{G+\Gamma k^2}{m}\right]\widehat\eta.
$$

The perturbation [advection-diffusion equation](../../../../../advection-diffusion-equation.md) gives

$$
s=Dq^2-Vq-Dk^2.
$$

The local solute balance at a moving graph, to first order, is

$$
D\partial_n C+(V+\eta_t)C=0.
$$

Its perturbation is $(V-Dq)\widehat c+sC_I\widehat\eta=0$, because the terms $D\eta C''(0)$ and $V\eta C'(0)$ cancel. Consequently the full [frozen-temperature solutal interface dispersion](../../../../../frozen-temperature-solutal-interface-dispersion.md) is

$$
\boxed{s=(Dq-V)\left[\frac VD-\frac{G+\Gamma k^2}{mC_I}\right],\qquad s=Dq^2-Vq-Dk^2.}
$$

No quasistatic approximation to solute [diffusion](../../../../../diffusion.md) was made here. For a growing mode the unique admissible liquid root is

$$
q=\frac{V+\sqrt{V^2+4D(s+Dk^2)}}{2D}.
$$

Writing $b=(G+\Gamma k^2)/(mC_I)$ and eliminating $s$ gives $(q-V/D)(q-V/D+b)=k^2$. The root continuously connected to the growing interface branch is therefore

$$
q=\frac VD+\frac{\sqrt{b^2+4k^2}-b}{2},\qquad
\boxed{s(k)=\frac D2\left(\frac VD-b\right)\left(\sqrt{b^2+4k^2}-b\right).}
$$

In particular, **unstable wavelengths exist exactly when $mVC_I/D>G$**, and their band is

$$
0<k^2<\frac{mVC_I/D-G}{\Gamma}.
$$

This is the [constitutional supercooling](../../../../../constitutional-supercooling.md) criterion: immediately above the plane, the local [liquidus](../../../../../liquidus.md) rises at rate $-mC'(0)=mVC_I/D$, so it overtakes the imposed thermal gradient when that rate exceeds $G$. The [Gibbs-Thomson effect](../../../../../gibbs-thomson-relation.md) cuts off short waves. At long wavelength $s\sim D(V/D-b)k^2/b$ for positive $G$. The exactly uniform inventory-changing displacement is not an instability of a fixed-inventory experiment. On stable branches the full [diffusion](../../../../../diffusion.md) problem also admits relaxation transients; the root selection above is sufficient to identify every exponentially growing interface mode.

If one additionally neglects the perturbation time [derivative](../../../../../derivative.md) in the liquid [diffusion](../../../../../diffusion.md) equation, the alternative reduced rate is

$$
s_{\rm qs}(k)=\frac12\left[\sqrt{V^2+4D^2k^2}-V\right]\left[\frac VD-\frac{G+\Gamma k^2}{mC_I}\right].
$$

It has the same onset and cutoff, but need not have the same rate away from the slow-growth regime. The [frozen-temperature approximation](../../../../../frozen-temperature-approximation.md) by itself does not justify this extra reduction.

After onset, protrusions reach more weakly saline liquid and advance faster, while grooves accumulate rejected brine. The planar interface develops cells and, as growth becomes sufficiently strong, [crystal dendrites](../../../../../dendrite-crystal.md) with concentrated liquid between them. Nonlinear competition changes the selected spacing; linear rates alone cannot fix the final geometry. The interdendritic liquid forms a [mushy layer](../../../../../mushy-layer.md), concentrates toward the [eutectic composition](../../../../../eutectic-composition.md), and ultimately freezes into a salt-bearing eutectic product when it reaches $T_E$. This replaces the pure planar salt-rejection picture with trapping and [freezing](../../../../../freezing.md) of brine between crystals.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
