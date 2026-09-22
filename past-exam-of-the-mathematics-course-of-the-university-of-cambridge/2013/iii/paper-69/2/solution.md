<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The required boundary model is a fracture that drains after the storm, with $h(0,t)=0$, and a current of finite extent whose flux vanishes at its advancing nose. Introduce [mass density](../../../../../density.md) $\rho$, gravity $g$, constant [porosity](../../../../../porosity.md) $\phi$ and [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu$. Hydrostatic [Darcy law](../../../../../darcy-law.md) gives the depth-integrated discharge $q=-k\rho g h h_x/\mu$. Fluid-volume conservation then gives the [Boussinesq equation for an unconfined aquifer](../../../../../boussinesq-equation-for-an-unconfined-aquifer.md)

$$
h_t=\kappa(hh_x)_x,\qquad\kappa=\frac{k\rho g}{\mu\phi}.
$$

The fluid volume per fracture length is $V=\phi\int_0^\infty h\,dx$; omitting the constant $\phi$ does not change its fractional decay rate.

The [conserved first moment of a draining porous current](../../../../../conserved-first-moment-of-a-draining-porous-current.md) follows directly:

$$
\frac{d}{dt}\int_0^\infty xh\,dx
=\kappa[xhh_x]_0^\infty-\kappa\int_0^\infty hh_x\,dx
=-\frac\kappa2[h^2]_0^\infty=0.
$$

The finite outlet discharge does not contribute to $[xhh_x]$ at $x=0$. This establishes $D=\int xh\,dx$ constant. An unspecified nonzero fracture head would instead give $\dot D=\kappa h(0,t)^2/2$; the drained boundary is essential.

For the [dipole similarity solution of a draining porous current](../../../../../dipole-similarity-solution-of-a-draining-porous-current.md), set $h=a t^\alpha f(\eta)$ and $\eta=x/(d t^\beta)$. The conserved first moment requires $\alpha+2\beta=0$, while matching the time powers in the evolution equation gives $\alpha-1=2\alpha-2\beta$. Hence

$$
\boxed{\alpha=-\frac12,\qquad\beta=\frac14}.
$$

Choose the nose at $\eta=1$ and the normalization $\kappa a/d^2=1$. The profile equation becomes

$$
-\frac12f-\frac14\eta f'=(ff')'.
$$

For $f=b\eta^2+c\eta^{1/2}$, the two sides have coefficients $-b,-5c/8$ and $6b^2,15bc/4$, respectively. The nonzero positive profile therefore has $b=-1/6$; its zero at $\eta=1$ gives $c=1/6$. Its normalization is determined by

$$
D=ad^2\int_0^1\eta f(\eta)\,d\eta=\frac{ad^2}{40},\qquad a=\frac{d^2}{\kappa}.
$$

Thus a complete choice of the constants is

$$
\boxed{d=(40\kappa D)^{1/4},\quad a=(40D/\kappa)^{1/2},\quad
b=-\frac16,\quad c=\frac16,\quad
h=\frac{a}{6\sqrt t}\left(\sqrt\eta-\eta^2\right)\ \ (0<\eta<1)}.
$$

Set $h=0$ beyond the nose. The square-root behavior at the outlet allows finite drainage: $ff'\to1/72$ as $\eta\downarrow0$, while $ff'\to0$ at the nose.

Since $\int_0^1f\,d\eta=1/18$, the volume is

$$
\boxed{V(t)=\frac{\phi ad}{18}t^{-1/4},\qquad\frac1V\frac{dV}{dt}=-\frac1{4t}}.
$$

The [drainage volume decay in a dipole porous current](../../../../../drainage-volume-decay-in-a-dipole-porous-current.md) shows that the printed positive rate cannot describe drainage and its factor is also inconsistent with the conserved-moment scaling. This solution supplies a direct counterexample to that rate and the corrected one. If the initial volume $V_0$ is prescribed at the start of a similarity phase, replace $t$ by $t+t_0$ with $t_0=(\phi ad/(18V_0))^4$. A general post-storm initial shape need not be exactly self-similar; this is the dipole similarity profile and its long-time scaling, not an asserted exact profile for every initial condition. The initial volume alone does not specify $D$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
