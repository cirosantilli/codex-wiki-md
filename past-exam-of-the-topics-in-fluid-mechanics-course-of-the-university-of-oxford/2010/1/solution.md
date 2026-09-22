<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose $x$ vertically upward. Let $G(x,t)$ be the gas-occupied part of a pipe cross-section, of area $\alpha A$. Define the phase mean [mass density](../../../density.md), [mass](../../../mass.md)-weighted [velocity](../../../velocity.md), second moment of [velocity](../../../velocity.md), and phase mean [pressure](../../../pressure-split.md) by

$$
\bar\rho_g=\frac{1}{\alpha A}\int_G\rho_g\,dA,\quad
\bar v=\frac{\int_G\rho_g v_x\,dA}{\alpha A\bar\rho_g},\quad
\overline{v^2}=\frac{\int_G\rho_g v_x^2\,dA}{\alpha A\bar\rho_g},\quad
\bar p_g=\frac{1}{\alpha A}\int_Gp_g\,dA.
$$

The [void fraction](../../../void-fraction.md) $\alpha$ is a volume fraction, not a [mass](../../../mass.md) fraction. The gas [momentum](../../../momentum-split.md) in a slice of length $dx$ is $A\alpha\bar\rho_g\bar v\,dx$; its advected [momentum flux](../../../momentum-flux.md) is $A\alpha\bar\rho_g\overline{v^2}$. The two end [pressures](../../../pressure-split.md) give the net force $-A\partial_x(\alpha\bar p_g)\,dx$. Include every other vertical force on the gas, including interfacial forces, in $M_g\,dx$. [Newton's second law](../../../newton-s-second-law.md) for this fixed slice, followed by division by $A\,dx$, therefore gives

$$
\boxed{\partial_t(\alpha\bar\rho_g\bar v)+\partial_x(\alpha\bar\rho_g\overline{v^2})=M_g/A-\partial_x(\alpha\bar p_g).}
$$

This is a [cross-section averaged phase momentum balance](../../../cross-section-averaged-phase-momentum-balance.md). In particular, [mass](../../../mass.md) weighting makes the [momentum](../../../momentum-split.md) and its flux exact averages; one must not replace $\overline{v^2}$ by $\bar v^2$ without an additional closure. With liquid mean [velocity](../../../velocity.md) $\bar u$, constant liquid [mass density](../../../density.md) $\rho_\ell$, and liquid second moment $\overline{u^2}$, the same calculation gives

$$
\boxed{\partial_t[(1-\alpha)\rho_\ell\bar u]+\partial_x[(1-\alpha)\rho_\ell\overline{u^2}]=M_\ell/A-\partial_x[(1-\alpha)\bar p_\ell].}
$$

With the common [pressure](../../../pressure-split.md) $p=\bar p_g=\bar p_\ell$, the specified [pressure](../../../pressure-split.md) contributions to $M_g,M_\ell$ cancel the phase-fraction [derivatives](../../../derivative.md) from the [product rule](../../../product-rule.md). The remaining [pressure](../../../pressure-split.md) forces per unit mixture volume are $-\alpha p_x$ and $-(1-\alpha)p_x$.

Assume that the bubbles at a given height have the stated radius $a$. Their number per unit mixture volume is $N=3\alpha/(4\pi a^3)$. The [drag force](../../../drag-physics.md) on a rising bubble opposes its relative [velocity](../../../velocity.md), so multiplication of the single-bubble law by $N$ gives the signed magnitude

$$
D_v=\frac{3C_D\rho_\ell\alpha}{4a}\bar v|\bar v|.
$$

[Gravity](../../../gravity.md) acts downward; the [drag force](../../../drag-physics.md) on the liquid is the opposite of that on the gas. With no wall force,

$$
\boxed{M'_g/A=-\alpha\bar\rho_g g-D_v,\qquad M'_\ell/A=-(1-\alpha)\rho_\ell g+D_v.}
$$

A bubble retains its [mass](../../../mass.md) in the absence of transfer between phases. Consequently $a^3\bar\rho_g=a_0^3\rho_0$ and

$$
\boxed{a=a_0(\rho_0/\bar\rho_g)^{1/3}.}
$$

For clarity suppress bars on $p,\rho_g,v$ in the steady calculation. On a macroscopic variation length $\ell$, gas [inertia](../../../inertia.md) per unit volume scales like $\alpha\rho_gv^2/\ell$, whereas the quadratic [drag force](../../../drag-physics.md) scales like $\alpha\rho_\ell v^2/a$. Their ratio is $O[(\rho_g/\rho_\ell)(a/\ell)]$. Thus $\rho_g=O(\rho_0)\ll\rho_\ell$, together with the scale separation $a\ll\ell$ inherent in this averaging model, justifies the leading-order neglect of gas [inertia](../../../inertia.md). Small reference density alone does not justify it in an arbitrarily short or strongly compressed region. Neglect gas weight at the same order, with the [liquid fraction](../../../liquid-fraction.md) not vanishing. For a stationary liquid, summing the two [momentum](../../../momentum-split.md) equations gives

$$
p_x=-g[\alpha\rho_g+(1-\alpha)\rho_\ell]\sim-\rho_\ell g(1-\alpha).
$$

The leading gas balance is $0=-\alpha p_x-D_v$. Substitution of the bubble-radius law yields

$$
\boxed{p_x=-\rho_\ell g(1-\alpha)=-\frac{3C_D\rho_\ell}{4a_0}(\rho_g/\rho_0)^{1/3}v|v|.}
$$

The gas [continuity equation](../../../continuity-equation.md), with constant pipe area and no [mass](../../../mass.md) exchange, is $\partial_t(\alpha\rho_g)+\partial_x(\alpha\rho_gv)=0$. Hence the steady gas [mass flux](../../../mass-flux.md) $J=\alpha\rho_gv$ is constant. For $0<\alpha<1$ the [pressure](../../../pressure-split.md) equation selects $v>0$, and

$$
v^2=\frac{4a_0g}{3C_D}(1-\alpha)(\rho_0/\rho_g)^{1/3},\qquad
J^2=\frac{4a_0g}{3C_D}\rho_0^{1/3}\alpha^2(1-\alpha)\rho_g^{5/3}.
$$

Evaluate the latter constant at a reference point $\rho_g=\rho_0$, $\alpha=\alpha_0$ and divide. The [terminal-drift density law for compressible bubbles](../../../terminal-drift-density-law-for-compressible-bubbles.md) is

$$
\boxed{\frac{\rho_g}{\rho_0}=\left[\frac{\alpha_0^2(1-\alpha_0)}{\alpha^2(1-\alpha)}\right]^{3/5}.}
$$

The exponent $3/5$ comes from combining [mass](../../../mass.md) conservation with the density dependence of bubble radius; no gas equation of state was needed.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2010](../../2010-split.md)
3. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../split.md)
4. [Topics in fluid mechanics course of the University of Oxford](../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
