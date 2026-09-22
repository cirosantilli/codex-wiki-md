<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In a [regular solution](../../../../regular-solution.md), ideal combinatorial [entropy](../../../../entropy-split.md) competes with a nonzero unlike-contact [energy](../../../../energy-split.md). For equal molecular [volumes](../../../../volume.md) and [mole fraction](../../../../mole-fraction.md) $\phi$ of species A, write mixing [free energy](../../../../thermodynamic-free-energy.md) per site as

$$
\frac{f(\phi)}{k_BT}
=\phi\ln\phi+(1-\phi)\ln(1-\phi)+\chi\phi(1-\phi),
$$

where

$$
\chi=\frac{z}{k_BT}\left[\epsilon_{AB}-\frac{\epsilon_{AA}+\epsilon_{BB}}2\right].
$$

Here $z$ is the [coordination number](../../../../coordination-number.md) and $\epsilon_{ij}$ a pair-contact [energy](../../../../energy-split.md) counted consistently in the lattice model. A positive $\chi$ penalizes unlike contacts; a negative value favors them. The logarithmic terms lower [free energy](../../../../thermodynamic-free-energy.md) on mixing. The sign of the [enthalpy of mixing](../../../../enthalpy-of-mixing.md) alone therefore does not determine miscibility.

At fixed [temperature](../../../../temperature-split.md) and composition, a homogeneous phase is globally stable only if no division into two compositions lowers its [free energy](../../../../thermodynamic-free-energy.md). The [common-tangent construction](../../../../common-tangent-construction.md) selects coexisting compositions $\phi_a,\phi_b$, equivalent to equality of both species' [chemical potentials](../../../../chemical-potential-split.md). Local stability to infinitesimal fluctuations instead requires

$$
\frac{f''}{k_BT}=\frac1\phi+\frac1{1-\phi}-2\chi>0.
$$

Zero [curvature](../../../../curvature.md) gives the [spinodal](../../../../spinodal.md), while the coexistence boundary is the [binodal](../../../../binodal.md). Between them a homogeneous state can be metastable and require [nucleation](../../../../nucleation.md); inside the [spinodal](../../../../spinodal.md) its small composition fluctuations grow. The symmetric [regular solution](../../../../regular-solution.md) has

$$
\boxed{\phi_c=\tfrac12,\qquad\chi_c=2.}
$$

Below this contact penalty, the [free energy](../../../../thermodynamic-free-energy.md) is convex at every composition. Above it a miscibility gap is possible around the central composition. If $\chi=A/T$ with $A>0$, heating promotes mixing, but specific interactions or temperature-dependent noncombinatorial terms can produce other trends.

For two [polymers](../../../../polymer-split.md), let $N_A,N_B$ count equal-volume segments per chain, and now let $\phi$ be the segment [volume fraction](../../../../volume-fraction.md) of A. Connecting segments into chains reduces their independent translational [entropy](../../../../entropy-split.md). The [binary Flory-Huggins polymer blend](../../../../binary-flory-huggins-polymer-blend.md) has

$$
\frac{f}{k_BT}=\frac{\phi}{N_A}\ln\phi
+\frac{1-\phi}{N_B}\ln(1-\phi)+\chi\phi(1-\phi).
$$

The energetic contact term remains extensive in the number of segments, while the favorable [entropy](../../../../entropy-split.md) per segment is reduced by $1/N_A$ and $1/N_B$. This is the key [long-chain limit of polymer-blend miscibility](../../../../long-chain-limit-of-polymer-blend-miscibility.md): a small positive incompatibility can overcome the mixing [entropy](../../../../entropy-split.md). The lattice treatment is a controlled model for this argument, rather than a claim that every real blend has composition-independent $\chi$.[1942, pp. 51–55: chain-connected lattice configurations and combinatorial mixing entropy; later sections add the energetic contribution](../../../../thermodynamics-of-high-polymer-solutions-by-paul-j-flory.md)

The local stability condition and critical interaction parameter become

$$
\frac1{N_A\phi}+\frac1{N_B(1-\phi)}-2\chi>0,\qquad
\boxed{\chi_c=\frac12\left(N_A^{-1/2}+N_B^{-1/2}\right)^2.}
$$

For equal chain [lengths](../../../../length.md), $\chi_c=2/N$. Similar segment chemistry and matched cohesive interactions can reduce the unlike-contact penalty; favorable specific interactions, such as complementary [hydrogen bonding](../../../../hydrogen-bonding.md), can make mixing favorable even for long chains. Lower [molar mass](../../../../molar-mass.md) increases mixing [entropy](../../../../entropy-split.md). [temperature](../../../../temperature-split.md) can help when it lowers the effective $\chi$, but heating is not universally sufficient. A suitable common [solvent](../../../../solvent.md) can facilitate processing or ternary mixing, and a block-copolymer compatibilizer can stabilize fine domains; neither guarantees that the final solvent-free binary material is one [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) molecular phase.

An oil–water [emulsion](../../../../emulsion.md) illustrates [emulsion stability versus molecular miscibility](../../../../emulsion-stability-versus-molecular-miscibility.md). A [surfactant](../../../../surfactant.md) adsorbs with its water-affine head toward water and its oil-affine tail toward oil, lowering [interfacial tension](../../../../interfacial-tension.md) and the [work](../../../../work.md) $\gamma\,dA$ needed to make additional interface. Breaking a fixed oil [volume](../../../../volume.md) $V_o$ into spherical droplets of radius $R$ gives total [area](../../../../surface-area.md) $3V_o/R$, so creating small droplets still requires substantial [area](../../../../surface-area.md) and usually mechanical [work](../../../../work.md).

Adsorbed [surfactants](../../../../surfactant.md) can oppose [droplet coalescence](../../../../droplet-coalescence.md) through charged double-layer repulsion, hydrated-head interactions or [steric repulsion](../../../../steric-repulsion.md) from sufficiently extended groups. Adequate coverage, [adsorption](../../../../adsorption.md) time, ionic conditions and [film drainage](../../../../film-drainage.md) affect the lifetime. A lower [interfacial tension](../../../../interfacial-tension.md) does not itself remove the bulk miscibility gap, and a protected [emulsion](../../../../emulsion.md) is commonly kinetically stabilized. A thermodynamically stable [microemulsion](../../../../microemulsion.md) is a distinct situation requiring an appropriate composition and free-energy balance. The two liquids must not be called molecularly miscible simply because droplets disperse visibly.

For the capillary, balance upward contact-line [force](../../../../force-split.md) against hydrostatic column weight, neglecting meniscus [volume](../../../../volume.md) and gas [density](../../../../density.md). For inner radius $r$,

$$
2\pi r\gamma\cos\theta=\rho g\pi r^2h,
\qquad h=\frac{2\gamma\cos\theta}{\rho gr}.
$$

The [contact angle](../../../../contact-angle.md) is measured through the liquid. [complete wetting](../../../../complete-wetting.md) means $\theta_2=0$, so the [contact-angle change of capillary rise](../../../../contact-angle-change-of-capillary-rise.md) gives

$$
\boxed{h_2=\frac{0.050}{\cos35^\circ}=0.06104\,\mathrm m\simeq6.10\,\mathrm{cm}.}
$$

This follows from the stipulated [wetting](../../../../wetting.md) change, holding radius, bulk liquid [surface tension](../../../../surface-tension-split.md) and [density](../../../../density.md) fixed. One should not replace that premise with a general claim that grease always improves glass [wetting](../../../../wetting.md); if contamination also changes the liquid [surface tension](../../../../surface-tension-split.md), the original height and new angle alone would not determine the new height.

For two wide vertical plates separated by gap $d$, use unit width. There are two upward contact-line contributions and liquid cross-sectional [area](../../../../surface-area.md) $d$, giving the [capillary rise between parallel plates](../../../../capillary-rise-between-parallel-plates.md):

$$
2\gamma\cos\theta=\rho gdh_{\rm plates},
\qquad\boxed{h_{\rm plates}=\frac{2\gamma\cos\theta}{\rho gd}.}
$$

Only one principal meniscus [curvature](../../../../curvature.md) contributes between wide plates, whereas a circular tube has two. For the same [fluid](../../../../fluid.md) and angle,

$$
\boxed{\frac{h_{\rm plates}}{h_{\rm tube}}=\frac rd.}
$$

If the plate gap equals the tube diameter, $d=2r$, the rise is half as large: the initial and completely [wetting](../../../../wetting.md) heights would be $2.50$ cm and $3.05$ cm. If instead $d=r$, the heights are equal. In either geometry, changing only the angle from $35^\circ$ to zero multiplies the height by $1/\cos35^\circ$. Since the question specifies no plate spacing, the general gap-dependent relation is the unambiguous result; the half-height answer requires the equal-gap-to-diameter convention.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
