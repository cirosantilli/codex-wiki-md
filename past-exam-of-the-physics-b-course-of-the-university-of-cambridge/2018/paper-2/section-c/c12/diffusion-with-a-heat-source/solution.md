<h1 id="section-c/c12/diffusion-with-a-heat-source/solution">Solution</h1>

↑ **Parent:** [Diffusion with a heat source](../diffusion-with-a-heat-source.md)

**Origin of [diffusion](../../../../../../diffusion.md).** In a material near local [thermal equilibrium](../../../../../../thermal-equilibrium-split.md), microscopic carriers transfer [energy](../../../../../../energy-split.md) from hotter regions to colder regions. On distances long compared with their [mean free path](../../../../../../mean-free-path.md) and times long compared with relaxation times, the local constitutive law is [Fourier's law](../../../../../../fourier-s-law.md),

$$
\mathbf J_Q=-\kappa\nabla T.
$$

Combining this temperature-gradient-driven flux with local [conservation of energy](../../../../../../conservation-of-energy.md) produces a [diffusion equation](../../../../../../diffusion-equation-split.md). This description assumes diffusive [thermal conduction](../../../../../../thermal-conduction.md); it is not generally valid for [ballistic transport](../../../../../../ballistic-transport.md), and flow would add advective transport.

**[Energy](../../../../../../energy-split.md) balance with heating.** Choose any fixed [volume](../../../../../../volume-thermodynamics.md) $V$, let $c$ be its uniform [volumetric heat capacity](../../../../../../volumetric-heat-capacity.md) and $H$ its [heat](../../../../../../heat-split.md) generation rate per unit [volume](../../../../../../volume-thermodynamics.md). The rate of increase of [internal energy](../../../../../../internal-energy-split.md) equals [heat](../../../../../../heat-split.md) generation minus outward [heat flux](../../../../../../heat-flux-density.md):

$$
\int_V c\frac{\partial T}{\partial t}\,dV
=-\oint_{\partial V}\mathbf J_Q\cdot\widehat{\mathbf n}\,dA+\int_VH\,dV
=\int_V\left[\nabla\cdot(\kappa\nabla T)+H\right]dV.
$$

Since $V$ is arbitrary, for constant [thermal conductivity](../../../../../../thermal-conductivity.md)

$$
\boxed{\frac{\partial T}{\partial t}=\frac{\kappa}{c}\nabla^2T+\frac{H}{c}.}
$$

The ratio $\kappa/c$ is the [thermal diffusivity](../../../../../../thermal-diffusivity.md) in $\mathrm{m^2\,s^{-1}}$. Here $c$ is in $\mathrm{J\,m^{-3}K^{-1}}$, $\kappa$ in $\mathrm{W\,m^{-1}K^{-1}}$ and $H$ in $\mathrm{W\,m^{-3}}$, so both right-hand terms have units $\mathrm{K\,s^{-1}}$. If [thermal conductivity](../../../../../../thermal-conductivity.md) varies with position or [temperature](../../../../../../temperature-split.md), the [divergence](../../../../../../divergence.md) $\nabla\cdot(\kappa\nabla T)$ must be retained rather than replacing it by $\kappa\nabla^2T$.

## ↑ Ancestors (15)

1. [Diffusion with a heat source](../diffusion-with-a-heat-source.md)
2. [C12](../../c12.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
