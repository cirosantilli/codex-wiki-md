<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\eta=H e^{\sigma t}J_0(\alpha r)$ using the [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md). The wall [boundary conditions](../../../../boundary-condition.md) at $z=\pm h$ select

$$
\phi_1=C_1\cosh[\alpha(z+h)]J_0(\alpha r)e^{\sigma t},\qquad
\phi_2=C_2\cosh[\alpha(h-z)]J_0(\alpha r)e^{\sigma t}.
$$

Because $J_0'(s)=-J_1(s)$, the sidewall [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md) requires

$$
\boxed{J_1(\alpha_na)=0,\qquad \alpha_n=\frac{j_{1,n}}a,\quad n=1,2,\ldots,}
$$

where $j_{1,n}$ are the positive zeros of $J_1$. These radial [eigenfunctions](../../../../eigenfunction.md) automatically preserve layer volume because

$$
\int_0^a rJ_0(\alpha_nr)\,dr=\frac{aJ_1(\alpha_na)}{\alpha_n}=0.
$$

The constant radial mode $\alpha=0$ cannot change the interface height in a closed tank: the [Laplace equation](../../../../laplace-equation.md) and the impermeable lids then give zero vertical [velocity](../../../../velocity.md), and a uniform displacement would change each layer's volume.

The [kinematic boundary condition](../../../../kinematic-boundary-condition.md) fixes

$$
C_1=\frac{\sigma H}{\alpha\sinh(\alpha h)},\qquad
C_2=-\frac{\sigma H}{\alpha\sinh(\alpha h)}.
$$

Thus the interface values are $\phi_1(0)=\sigma\eta\coth(\alpha h)/\alpha$ and $\phi_2(0)=-\sigma\eta\coth(\alpha h)/\alpha$. Substitution in the [normal stress](../../../../normal-stress.md) condition gives the [finite-depth Rayleigh-Taylor dispersion relation](../../../../finite-depth-rayleigh-taylor-dispersion-relation.md):

$$
\frac{(\rho_1+\rho_2)\sigma_n^2}{\alpha_n}\coth(\alpha_nh)
=(\rho_2-\rho_1)g,
$$

so

$$
\boxed{\sigma_{n,\pm}=\pm\sqrt{\mathcal A g\alpha_n\tanh(\alpha_nh)},\qquad
\mathcal A=\frac{\rho_2-\rho_1}{\rho_2+\rho_1}>0.}
$$

Here $\mathcal A$ is the [Atwood number](../../../../atwood-number.md). Every allowed mode has a positive [growth rate](../../../../growth-rate.md) and is subject to [Rayleigh-Taylor instability](../../../../rayleigh-taylor-instability.md). Since $d[\alpha\tanh(\alpha h)]/d\alpha=\tanh(\alpha h)+\alpha h\operatorname{sech}^2(\alpha h)>0$, shorter radial scales grow faster. The limits are

$$
\sigma_{n,+}\sim\sqrt{\mathcal A gh}\,\alpha_n\quad(\alpha_nh\ll1),\qquad
\sigma_{n,+}\sim\sqrt{\mathcal A g\alpha_n}\quad(\alpha_nh\gg1).
$$

There is no fastest finite [wavenumber](../../../../wavenumber.md) in the ideal sharp-interface model without [surface tension](../../../../surface-tension-split.md), [viscosity](../../../../dynamic-viscosity-split.md) or [diffusion](../../../../diffusion.md). The zero-initial-[velocity](../../../../velocity.md) condition uses both exponential branches: an initial mode $H J_0(\alpha_nr)$ evolves as $H\cosh(\sigma_{n,+}t)J_0(\alpha_nr)$. If the [mass density](../../../../density.md) ordering were reversed the same calculation would give oscillatory stable modes; equal [mass densities](../../../../density.md) give neutral modes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
