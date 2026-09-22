# Dragged-bead fluctuation theorem experiment

↑ **Parent:** [Fluctuation theorem](fluctuation-theorem.md)

The 2002 experiment trapped a $6.3\,\mathrm{\mu m}$ bead in [water](water.md) with a $980\,\mathrm{nm}$ [laser](laser.md), a $100\times$, [numerical aperture](numerical-aperture.md) $1.3$ objective and a piezo-driven microscope stage. A quadrant [photodiode](photodiode.md) tracked bead position at $1\,\mathrm{kHz}$ with approximately $500\,\mathrm{Hz}$ bandwidth and reported $15\,\mathrm{nm}$ resolution. Stage translation drove water past the fixed [optical trap](optical-tweezers.md) at $1.25\,\mathrm{\mu m/s}$. Weak trapping prolonged the transient; stationary recording before translation established the position reference. [Stokes drag law](stokes-s-law.md) calibration was checked against the bead's measured [diffusion coefficient](diffusion-coefficient.md). [Wang and colleagues, 2002, p. 050601-2: apparatus, calibration and trajectory protocol](experimental-demonstration-of-violations-of-the-second-law-of-thermodynamics-for-small-systems-and-short-time-scales-by-g-m-wang-and-others.md)

From calibrated [displacement](displacement.md) and calibrated [harmonic optical trap](harmonic-optical-trap.md) [force](force.md), the experimenters evaluated the dimensionless driven-bead dissipation functional

$$
\Sigma_t^{\rm drive}=\frac1{k_BT}\int_0^t\mathbf v_{\rm opt}\cdot\mathbf F_{\rm opt}(u)\,du.
$$

Among 540 trajectories, negative values became less frequent with duration. Figure 2 compared the negative/positive count ratio with $\langle e^{-\Sigma_t^{\rm drive}}\rangle_{\Sigma_t^{\rm drive}>0}$; its agreement tested the paper's integrated transient relation. The detailed log-ratio plot in Figure 4 used simulated particle [sample trajectories](sample-path.md), not bead measurements. Near-zero sign discrimination and stage-start transients limited the earliest points. [Wang and colleagues, 2002, Eq. (2), Eq. (3), pp. 050601-2–4 and Figs. 1, 2 and 4](experimental-demonstration-of-violations-of-the-second-law-of-thermodynamics-for-small-systems-and-short-time-scales-by-g-m-wang-and-others.md)

For any continuous [probability distribution](probability-distribution.md) satisfying the same-law relation, integration over $s>0$ yields

$$
\frac{\Pr(\Sigma<0)}{\Pr(\Sigma>0)}
=\left\langle e^{-\Sigma}\right\rangle_{\Sigma>0}.
$$

This conditional relation explains the comparison without equating it to the unconditional [integral fluctuation theorem](integral-fluctuation-theorem.md). The experiment supports a specified driven-system relation; it does not establish a universal same-law symmetry for any definition of [heat](heat.md) or [entropy production](entropy-production.md). In particular, a transient work-like functional should not silently acquire the actual-distribution endpoint term in [finite trajectory entropy production](finite-trajectory-entropy-production.md). Negative realizations are compatible with positive mean dissipation and the [Second law of thermodynamics](second-law-of-thermodynamics.md); they do not provide a cyclic machine with reliable [work](work.md) output from a single [thermal reservoir](heat-bath.md).

## ↑ Ancestors (8)

1. [Fluctuation theorem](fluctuation-theorem.md)
2. [Entropy production](entropy-production.md)
3. [Stochastic thermodynamics](stochastic-thermodynamics.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
