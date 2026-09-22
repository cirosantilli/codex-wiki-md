<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

For a bulk liquid and vapor at common fixed [temperature](../../../../temperature-split.md) and [pressure](../../../../pressure-split.md), transfer $dN_l$ molecules from vapor to liquid while holding their sum fixed. The [Gibbs free energy](../../../../gibbs-free-energy.md) change is $dG=(\mu_l-\mu_v)dN_l$. [Thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md) with both phases present requires stationarity under either sign of transfer, hence $\boxed{\mu_l=\mu_v}$. This is the bulk coexistence condition; an interface's curvature adds a surface-energy cost.

In the capillarity approximation, take an incompressible drop with constant liquid [number density](../../../../number-density.md) $n_l$, bulk [chemical potential](../../../../chemical-potential-split.md) $\mu_l$ at the specified reservoir conditions, and size-independent [surface tension](../../../../surface-tension-split.md) $\Gamma$. The liquid bulk is extensive, so its Gibbs [thermodynamic free energy](../../../../thermodynamic-free-energy.md) is $N_l\mu_l$. Creating interface area reversibly at fixed [temperature](../../../../temperature-split.md) adds $\Gamma A$. Equivalently, along growth at fixed bulk parameters the stated differential integrates as $dG_d=\mu_l\,dN_l+\Gamma\,dA$, with the no-drop reference set to zero. For a sphere,

$$
\boxed{G_d=\frac43\pi R^3n_l\mu_l+4\pi R^2\Gamma.}
$$

This approximation uses bulk properties for the interior and neglects the molecular interface thickness, curvature dependence of [surface tension](../../../../surface-tension-split.md) and higher compressibility corrections. It does not apply quantitatively to drops only a few molecules across.

The vapor contains $N-N_l$ molecules. Treat its [chemical potential](../../../../chemical-potential-split.md) as approximately unchanged by forming the drop, as for a large surrounding reservoir or negligible vapor depletion. Then

$$
\boxed{G_{\rm tot}(R)=N\mu_v+\frac43\pi n_l(\mu_l-\mu_v)R^3+4\pi\Gamma R^2.}
$$

The [radius](../../../../radius.md) is limited by the available molecules in a finite sample; the constant-reservoir expression is a local nucleation model, not a description of arbitrarily complete vapor depletion. The excess over the vapor reference has derivative

$$
\Delta G'(R)=4\pi R[2\Gamma+n_l(\mu_l-\mu_v)R].
$$

If $\mu_l>\mu_v$, it increases for every $R>0$, leaving only the stable boundary minimum $R=0$. If $\mu_l<\mu_v$, $R=0$ is a metastable local minimum and the additional stationary [radius](../../../../radius.md) is

$$
\boxed{R_c=\frac{2\Gamma}{n_l(\mu_v-\mu_l)}.}
$$

At that [radius](../../../../radius.md) $\Delta G''=-8\pi\Gamma<0$, so it is an unstable maximum. The [classical nucleation theory](../../../../classical-nucleation-theory.md) barrier is $16\pi\Gamma^3/[3n_l^2(\mu_v-\mu_l)^2]$.

<a id="section-c/c11/image-surface-cost-and-bulk-gain-produce-a-critical-droplet-in-supersaturated-vapor"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004-droplet-nucleation-barrier.png)

**[Figure 3](#section-c/c11/image-surface-cost-and-bulk-gain-produce-a-critical-droplet-in-supersaturated-vapor). Surface cost and bulk gain produce a critical droplet in supersaturated vapor**. Original dimensionless capillarity curves. The supersaturated case has a barrier at the critical radius; the other curve rises monotonically. These are reservoir-model free energies, before finite-sample depletion changes the chemical potentials.

A fluctuation below $R_c$ tends to shrink because reducing its surface cost lowers [thermodynamic free energy](../../../../thermodynamic-free-energy.md). **A supercritical drop tends to grow**, because its bulk free-energy gain outweighs the added surface cost. Growth continues while material supply and supersaturation allow it, eventually changing the vapor state or leading to macroscopic liquid. Curved-interface [pressure](../../../../pressure-split.md) and chemical [thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md) can also be described through the [Young–Laplace equation](../../../../young-laplace-equation.md) and the [Kelvin equation](../../../../kelvin-equation.md).

## ↑ Ancestors (13)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
