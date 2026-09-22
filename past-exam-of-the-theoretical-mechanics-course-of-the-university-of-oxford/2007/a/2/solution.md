<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let the thin transverse length be $Re^{-1/2}$ times the longitudinal scale and write $Y=Re^{1/2}y$, $V=Re^{1/2}v$. Continuity then remains $u_x+V_Y=0$. Transverse momentum gives $p_Y=0$ to leading order; the quiescent exterior has constant [pressure](../../../../pressure-split.md), hence $p_x=0$. Axial viscous diffusion in $x$ is smaller by $Re^{-1}$, leaving

$$
\boxed{uu_x+Vu_Y=u_{YY},\qquad u_x+V_Y=0.}
$$

[Symmetry](../../../../symmetry-physics.md) about the jet centreline requires $V=0$ and $u_Y=0$ at $Y=0$. At large positive $Y$, require $u\to0$ and $u_Y\to0$. The transverse [velocity](../../../../velocity.md) can approach a finite nonzero scaled [entrainment](../../../../fluid-entrainment.md) [velocity](../../../../velocity.md); imposing $V\to0$ as well would rule out the jet. The physical transverse [velocity](../../../../velocity.md) remains smaller by $Re^{-1/2}$ and matches an entraining outer flow.

Using continuity, the momentum equation is $\partial_x(u^2)+\partial_Y(uV-u_Y)=0$. Integrating across the jet, the boundary terms vanish because $u,u_Y\to0$ while $V$ is finite. Thus

$$
\boxed{M=\int_{-\infty}^\infty u^2\,dY=\text{constant}.}
$$

Apart from the dimensional [density](../../../../density.md) and [velocity](../../../../velocity.md)/length factors, this is the conserved axial [momentum flux](../../../../momentum-flux.md) supplied by the nozzle. [Entrainment](../../../../fluid-entrainment.md) increases [volume flux](../../../../volumetric-flow-rate.md) without adding axial momentum from the resting exterior.

For $u=x^\alpha f'(\eta)$ with $\eta=Y/x^\beta$, use the [stream function](../../../../stream-function.md) $\psi=x^{\alpha+\beta}f(\eta)$ so that $u=\psi_Y$ and $V=-\psi_x$. Momentum conservation requires $2\alpha+\beta=0$. Inertia and diffusion scale as $x^{2\alpha-1}$ and $x^{\alpha-2\beta}$, so $\alpha+2\beta=1$. Therefore $\boxed{\alpha=-1/3,\quad\beta=2/3}$. In particular

$$
V=x^{-2/3}(2\eta f'-f)/3.
$$

Substitution reduces momentum to $3f^{(3)}+ff''+(f')^2=0$, with $f(0)=f''(0)=0$ and $f'(\infty)=0$. Integrating first gives $3f''+ff'=0$, the integration constant vanishing at the centreline. A second integration gives $3f'+f^2/2=C$. Parameterize its positive constant as $C=18A^2$ and solve the resulting [Riccati equation](../../../../riccati-equation.md) with $f(0)=0$:

$$
\boxed{f=6A\tanh(A\eta),\qquad u=6A^2x^{-1/3}\operatorname{sech}^2(AYx^{-2/3}).}
$$

The momentum [integral](../../../../integral-split.md) fixes its scale, since $\int_{-\infty}^\infty\operatorname{sech}^4z\,dz=4/3$:

$$
\boxed{M=48A^3,\qquad A=(M/48)^{1/3}.}
$$

The upper-half [entrainment](../../../../fluid-entrainment.md) is $V\to-2Ax^{-2/3}$; the negative side has the opposite sign, drawing ambient fluid inward. This is the [Bickley jet](../../../../bickley-jet.md), valid in the slender far-downstream laminar regime, rather than in the immediate nozzle region.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
