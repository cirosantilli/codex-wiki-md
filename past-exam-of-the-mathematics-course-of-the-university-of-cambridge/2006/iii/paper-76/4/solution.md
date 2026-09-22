<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For fixed nominal boundary tractions and dead body forces, use the total potential

$$
\Pi[x]=\int_\Omega W(F)\,dX-\int_\Omega\rho_0g_i x_i\,dX-\int_{\partial\Omega_T}T_i x_i\,dA_0.
$$

The dead-load terms are linear in the [deformation map](../../../../../deformation-map.md). Let $x(\varepsilon)$ be a constraint-preserving perturbation path through equilibrium, with $H=\delta F$ and $K=\delta^2F$. Differentiating $\phi(F)=0$ twice gives $\phi_{,F}:H=0$ and $\phi_{,F}:K=-\phi_{,FF}[H,H]$. Equilibrium has [nominal stress tensor](../../../../../nominal-stress-tensor.md) $P_{Ii}=W_{,F_{iI}}+q\phi_{,F_{iI}}$. Its virtual-work relation, applied to $\delta^2x$, gives the otherwise remaining first-derivative contribution $\Pi'[\delta^2x]=-\int q\phi_{,F}:K\,dX$. Therefore the constrained [second variation](../../../../../second-variation.md) is

$$
\boxed{\mathcal Q[H]=\int_\Omega\left(W_{,F_{iI}F_{jJ}}+q\phi_{,F_{iI}F_{jJ}}\right)H_{iI}H_{jJ}\,dX}.
$$

For a time-dependent linearized perturbation $y$, the incremental reaction stress contains $\delta q\,\phi_{,F}$, but its power vanishes because $\phi_{,F}:\nabla\dot y=0$. Multiply the incremental momentum equation by $\dot y$, integrate by parts, and use zero incremental dead-load traction or the prescribed displacement condition. One obtains

$$
\frac{d}{dt}\left\{\frac12\int_\Omega\rho_0|\dot y|^2dX+\frac12\mathcal Q[\nabla y]\right\}=0.
$$

Positive $\mathcal Q$ is therefore the standard [constrained second-variation stability in elasticity](../../../../../constrained-second-variation-stability-in-elasticity.md) criterion: perturbations cannot grow in this quadratic energy norm. A statement in a specified displacement norm also uses the usual coercivity and boundary conditions removing uncontrolled rigid-motion modes; translations with $\delta F=0$ are not tested by the displayed condition. This is a small-perturbation energy argument, not a claim of global nonlinear stability.

For the cube use [incompressibility](../../../../../incompressible-flow.md) in the form $\phi=\det F-1$. A [neo-Hookean solid](../../../../../neo-hookean-solid.md) has $W_{,F}=\mu F$, and hence the spatial-index-first transpose of nominal stress is $\mu F+qF^{-T}$. On the diagonal family, equality to $TI$ gives

$$
T=\mu\lambda+q\lambda^{-1}=\mu\lambda^{-1/2}+q\lambda^{1/2}.
$$

The first relation immediately gives $\boxed{q=T\lambda-\mu\lambda^2}$. Eliminating $q$ and factoring yields

$$
(1-\lambda^{-3/2})[\mu(\lambda+\lambda^{-1/2})-T]=0.
$$

Thus $\boxed{\lambda=1\quad\text{or}\quad T/\mu=\lambda+\lambda^{-1/2}}$.

Let $t=T/\mu$ and $h(\lambda)=\lambda+\lambda^{-1/2}$. Its derivative $h'=1-\tfrac12\lambda^{-3/2}$ vanishes only at $\lambda_c=2^{-2/3}$, where $h''>0$ and $h_c=3\,2^{-2/3}$. Also $h\to\infty$ at both ends of $(0,\infty)$. Therefore $h(\lambda)=t$ has two distinct positive roots for $t>h_c$, one repeated root at $h_c$, and none below. **There is an exception to the printed assertion that both roots differ from one: at $t=2$, one root is exactly $\lambda=1$.** Indeed, with $x=\sqrt\lambda$, the equation becomes $(x-1)(x^2+x-1)=0$, so the only other positive stretch is $\lambda=(3-\sqrt5)/2$.

Evaluate the stability form directly on the prescribed uniform perturbation

$$
H=\delta\lambda\,\operatorname{diag}(1,-\tfrac12\lambda^{-3/2},-\tfrac12\lambda^{-3/2}).
$$

It satisfies $\operatorname{tr}(F^{-1}H)=0$. The determinant Hessian identity is

$$
(\det F)_{,FF}[H,H]=J\{[\operatorname{tr}(F^{-1}H)]^2-\operatorname{tr}[(F^{-1}H)^2]\}=-\frac32\lambda^{-2}(\delta\lambda)^2.
$$

Meanwhile $W_{,FF}[H,H]=\mu(1+\tfrac12\lambda^{-3})(\delta\lambda)^2$. For the unit reference cube,

$$
\mathcal Q=\left[\mu(1+\tfrac12\lambda^{-3})-\frac{3q}{2\lambda^2}\right](\delta\lambda)^2.
$$

On the trivial branch, $q=T-\mu$ and

$$
\boxed{\mathcal Q=\tfrac32\mu(2-t)(\delta\lambda)^2}.
$$

Thus the undeformed state is stable in this perturbation family for $t<2$, unstable for $t>2$, and quadratically neutral at $t=2$.

On a nontrivial branch, substitute $t=h(\lambda)$ and put $z=\lambda^{-3/2}$:

$$
\boxed{\mathcal Q=\tfrac\mu2(z-1)(z-2)(\delta\lambda)^2}.
$$

The smaller root always has $\lambda<\lambda_c$, hence $z>2$, and is stable. For $h_c<t<2$, the larger root lies between $\lambda_c$ and one, so $1<z<2$ and it is unstable; the trivial branch is the second stable equilibrium. For $t>2$, the larger root lies above one and has $0<z<1$, so it is stable; the trivial branch is now unstable. **Whenever there are three distinct equilibria in this family, precisely two are stable and one unstable against the specified uniform perturbations.** This does not establish stability to every nonuniform or symmetry-breaking perturbation.

The [homogeneous tensile bifurcation of a neo-Hookean cube](../../../../../homogeneous-tensile-bifurcation-of-a-neo-hookean-cube.md) has a nontrivial-branch fold at $t=3\,2^{-2/3}$ and a meeting with the undeformed branch at $\boxed{t=2}$. The latter is the bifurcation from the undeformed state. Stating both values distinguishes this branch intersection from the earlier creation of the two nontrivial solutions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
