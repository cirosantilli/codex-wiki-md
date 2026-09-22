<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The one-group particle balance with a prescribed external volume source $S$ can be written

$$
\frac1v\frac{\partial\phi}{\partial t}
=-\nabla\cdot\mathbf J-\Sigma_a\phi+\nu\Sigma_f\phi+S,
\qquad
\mathbf J=-D\nabla\phi.
$$

Here $\phi$ is scalar [neutron flux](../../../../../neutron-flux.md), $D$ is the [neutron diffusion coefficient](../../../../../neutron-diffusion-coefficient.md), and $\Sigma_a,\Sigma_f$ are [macroscopic cross sections](../../../../../macroscopic-nuclear-reaction-cross-section.md). The terms describe accumulation, current divergence, absorption, [nuclear fission](../../../../../nuclear-fission.md) production and external input.

For a [steady state](../../../../../steady-state.md), set $\partial_t\phi=0$; source-free means $S=0$. In a homogeneous medium $D$ is spatially constant, so substitution gives

$$
D\nabla^2\phi+(\nu\Sigma_f-\Sigma_a)\phi=0.
$$

The supplied notation defines $\eta$ as the effective production per absorption, $\eta=\nu\Sigma_f/\Sigma_a$. Therefore

$$
\boxed{\nabla^2\phi+\frac{(\eta-1)\Sigma_a}{D}\phi=0.}
$$

This identification uses the absorption accounting for the homogeneous model; a fuel-only reproduction factor with other absorbers excluded would not automatically equal this $\eta$. The derivation assumes one prescribed energy group, constant effective coefficients and the [diffusion approximation](../../../../../diffusion-approximation.md); all neutron production included here is represented by the steady [nuclear fission](../../../../../nuclear-fission.md) term.

## ↑ Ancestors (10)

1. [B](../b.md)
2. [2](../../2.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
