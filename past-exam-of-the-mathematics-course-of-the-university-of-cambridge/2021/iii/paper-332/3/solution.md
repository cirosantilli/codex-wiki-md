<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take the rock at $z=0$, the till–ice interface at $z=h$, and the ice surface at $z=h+H$. The common leading [hydrostatic pressure](../../../../../hydrostatic-pressure.md) has horizontal gradient

$$
p_x=\rho gH_x.
$$

The thin-film momentum equations are

$$
\lambda\mu u_{t,zz}=p_x,
\qquad
\mu u_{i,zz}=p_x.
$$

Impose no slip at the rock, continuity of velocity and shear stress at $z=h$, and zero shear at the ice surface. Expanding for $h/H\ll1$ gives the till flux and ice flux

$$
q_t=-\frac{\rho g}{2\lambda\mu}Hh^2H_x,
$$



$$
q_i=-\frac{\rho g}{3\mu}
\left(1+\frac{3h}{\lambda H}\right)H^3H_x.
$$

The basal shear stress is

$$
\tau_0=-\rho gHH_x+o(\rho gHH_x).
$$

Applying [mass conservation](../../../../../mass-conservation.md) separately to the ice and till, with erosion source $E\tau_0$, gives

$$
\boxed{
H_t=\frac{\rho g}{3\mu}
\partial_x\left[\left(1+\frac{3h}{\lambda H}\right)H^3H_x\right]},
$$

and

$$
\boxed{
h_t=\frac{\rho g}{2\lambda\mu}
\partial_x(Hh^2H_x)-\rho gEH H_x}.
$$

In a steady state $q_i=q_0$. Balancing the two terms in the till equation over length $L$ gives

$$
\frac{\rho g}{\lambda\mu}
\frac{H^2h^2}{L}\sim\rho gEH^2,
$$

and hence

$$
\boxed{h\sim(\lambda\mu EL)^{1/2}},
$$

independently of $q_0$. Without substantial lubrication, the usual shallow-ice balance gives $H^4\sim\mu q_0L/(\rho g)$. Therefore

$$
\left(\frac{h}{\lambda H}\right)^4
\sim\frac{\mu E^2L\rho g}{\lambda^2q_0}
=\mathcal E.
$$

The sheet is essentially unlubricated when $\boxed{\mathcal E\ll1}$.

For $\mathcal E\gg1$, the sliding term dominates the ice flux:

$$
q_0=-\frac{\rho g}{\lambda\mu}H^2hH_x.
$$

Integrating the steady till equation from $x=0$, where $H=H_0$ and $h=0$, gives

$$
Hh^2H_x=\lambda\mu E(H^2-H_0^2).
$$

Eliminating $H_x$ between these equations yields

$$
\boxed{h=\frac{\rho gE}{q_0}H(H_0^2-H^2)}.
$$

With $F=H/H_0$ and $\xi=x/L$, a second integration gives

$$
\boxed{3F^4-2F^6=1-\xi},
$$

where the physical branch decreases from $F(0)=1$ to $F(1)=0$. The length condition determines

$$
\boxed{
H_0=\left(\frac{12\lambda\mu q_0^2L}
{\rho^2g^2E}\right)^{1/6}}.
$$

Using this relation in the till thickness gives

$$
\boxed{
h(x)=\sqrt{12\lambda\mu EL}\,F(\xi)[1-F(\xi)^2]}.
$$

**Thus $H$ decreases monotonically from $H_0$ to zero. The till starts at zero, rises to one interior maximum at $F=1/\sqrt3$, and returns to zero at the margin.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
