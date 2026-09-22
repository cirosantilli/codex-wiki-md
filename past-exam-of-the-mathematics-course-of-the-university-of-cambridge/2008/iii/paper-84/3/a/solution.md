<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $Q$ as the fluid volume flux per unit source length into one side of the aquifer. For a symmetric release with total rate $Q$, use $Q/2$ on each side. Introduce a constant [porosity](../../../../../../porosity.md) $\phi$ to distinguish [Darcy velocity](../../../../../../darcy-velocity.md) from the advecting [interstitial velocity](../../../../../../pore-velocity.md); if the given flux is already normalized to pore volume, this factor is absorbed in its definition. With a pressure gradient $G=-p_x>0$, [Darcy law](../../../../../../darcy-law.md) gives

$$
q_D(z)=\frac{k_0G}{\mu}z(h-z),
\qquad Q=\int_0^h q_D(z)\,dz=\frac{k_0Gh^3}{6\mu}.
$$

Thus, with $\xi=z/h$, the pore velocity and its depth average are

$$
u(z)=6U\xi(1-\xi),\qquad U=\frac{Q}{\phi h}.
$$

The tracer concentration initially obeys the two-dimensional [advection-diffusion equation](../../../../../../advection-diffusion-equation.md)

$$
c_t+u(z)c_x=D(c_{xx}+c_{zz}),\qquad c_z=0\quad\text{at }z=0,h.
$$

Reflecting transverse boundaries and constant effective molecular [diffusion](../../../../../../diffusion.md) are assumed. No independent radioactive decay rate is supplied; it can be added separately if it is significant over the experiment.

For times long compared with $h^2/D$, transverse diffusion exchanges tracer between fast and slow streamlines. Write $c=C(x,t)+\chi(z)C_x+\cdots$, where $C=\overline c$ and $\overline\chi=0$. At the leading transverse-correction order,

$$
D\chi_{zz}=u-U,\qquad\chi_z(0)=\chi_z(h)=0.
$$

Integration yields

$$
\chi=\frac{Uh^2}{D}\left(\xi^3-\frac{\xi^4}{2}-\frac{\xi^2}{2}+\frac1{60}\right).
$$

Its mean and boundary derivatives are zero. Averaging the concentration equation gives $C_t+UC_x=[D-\overline{(u-U)\chi}]C_{xx}$. Integration by parts in the cell equation shows that the enhancement is positive:

$$
-\overline{(u-U)\chi}=D\overline{\chi_z^2}
=\frac{U^2h^2}{D}\int_0^1(3\xi^2-2\xi^3-\xi)^2\,d\xi
=\frac{U^2h^2}{210D}.
$$

Consequently [Taylor dispersion in a parabolic porous-layer velocity profile](../../../../../../taylor-dispersion-in-a-parabolic-porous-layer-velocity-profile.md) gives

$$
\boxed{C_t+UC_x=D_{\rm eff}C_{xx},
\qquad D_{\rm eff}=D+\frac{U^2h^2}{210D}
=D+\frac{Q^2}{210\phi^2D}.}
$$

Injection fixes the inlet concentration or solute-flux boundary condition. This depth-averaged equation requires transverse equilibration and longitudinal concentration variations slow enough for the cell expansion. The supplied PDF hint has both a different polynomial and a false numerical value: its integral evaluates exactly to $-83/2520$, not $0.3525$. The cell problem above supplies the coefficient independently.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
