<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $w$ be downward [Darcy flux](../../../../../darcy-velocity.md), measured per unit total horizontal area. Neglect the resistance of the displaced phase, [capillary pressure](../../../../../capillary-pressure.md), and horizontal subsurface flow. Taking atmospheric pressure as zero, the upper end of the saturated column has pressure $\rho gh$ and its advancing lower end has pressure zero. Across a column of depth $l$, [Darcy law](../../../../../darcy-law.md) therefore gives

$$
w=\frac{k}{\mu}\left(\frac{\rho gh}{l}+\rho g\right)
=\frac{gk}{\nu}\left(1+\frac hl\right).
$$

The pressure head from the overlying layer supplies $h/l$, and gravity supplies one. Because the new liquid fills a pore volume $\phi\,dl$ per unit area, the [vertical imbibition under a draining liquid layer](../../../../../vertical-imbibition-under-a-draining-liquid-layer.md) obeys $\phi\dot l=w$. [Volume conservation](../../../../../volume-conservation.md) gives $h+\phi l=h_0$, so, until the surface layer is exhausted,

$$
\boxed{\dot l=\frac{gk}{\phi\nu}\left(\frac{h_0}{l}+1-\phi\right),\qquad h=h_0-\phi l,\quad0<l<h_0/\phi}.
$$

The initial condition is understood as a limiting solution of this singular equation. For $0<\phi<1$, separation of variables gives

$$
t=\frac{\phi\nu}{gk}\left[\frac{l}{1-\phi}-\frac{h_0}{(1-\phi)^2}\log\left(1+\frac{(1-\phi)l}{h_0}\right)\right].
$$

At small penetration, expansion of the logarithm yields $t\sim\phi\nu l^2/(2gkh_0)$, hence

$$
\boxed{l(t)\sim\left(\frac{2gkh_0}{\phi\nu}t\right)^{1/2}}.
$$

A sufficient dimensional early-time condition is $t\ll\phi\nu h_0/(gk)$, for which $l\ll h_0$. The printed $t\ll1$ needs a chosen time unit or nondimensionalization. In the limiting case $\phi=1$, $l^2=2gkh_0t/\nu$ holds exactly until $h=0$. The divergent initial [Darcy flux](../../../../../darcy-velocity.md) is an idealization of sudden contact with a dry continuum; it cannot describe penetration below the pore scale.

For the spreading surface layer, measure $z$ upwards from the substrate. A thin, slow [gravity current](../../../../../gravity-current.md) has [hydrostatic pressure](../../../../../hydrostatic-pressure.md) $p=\rho g(h-z)$ and a leading horizontal viscous balance $\nu u_{zz}=gh_x$. A [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) at $z=0$ and a [stress-free boundary condition](../../../../../stress-free-boundary-condition.md) at $z=h$ give

$$
u=\frac g\nu h_x\left(\frac{z^2}{2}-hz\right),\qquad
q=\int_0^h u\,dz=-\frac{g}{3\nu}h^3h_x.
$$

This [lubrication gravity-current flux](../../../../../lubrication-gravity-current-flux.md) drives horizontal spreading down the surface-pressure gradient. Surface [volume conservation](../../../../../volume-conservation.md) is $h_t+q_x=-w$, while conservation in the pores is $\phi l_t=w$. Combining these balances gives the [deep-substrate drainage of a gravity current](../../../../../deep-substrate-drainage-of-a-gravity-current.md) model

$$
\boxed{h_t-\frac{g}{3\nu}(h^3h_x)_x=-\frac{gk}{\nu}\left(1+\frac hl\right)=-\phi l_t}.
$$

Drainage transfers liquid from the surface layer into the substrate. Indeed $(h+\phi l)_t+q_x=0$.

For definiteness take a one-sided current on $0<x<x_N(t)$, supplied at $x=0$. The imposed volume is per unit span, so $V_0$ has dimensions of area. The [boundary conditions](../../../../../boundary-condition.md) and [volume conservation](../../../../../volume-conservation.md) constraint are

$$
\begin{gathered}
h,l\ge0,\qquad h=l=0\ \text{outside the wetted region},\qquad h(x_N,t)=l(x_N,t)=0,\\
q(x_N,t)=0,\qquad q(0,t)=\frac{3V_0t^2}{\tau^3},\qquad
\int_0^{x_N(t)}[h(x,t)+\phi l(x,t)]\,dx=V_0(t/\tau)^3.
\end{gathered}
$$

The source starts from zero injected volume. Initially dry points acquire $l>0$ only when the advancing current reaches them; the formula $h/l$ is not applied outside that region. At the advancing nose these are limiting conditions for a singular drainage equation. For a source feeding two identical sides, each side has half the volume and inlet flux; only the corresponding numerical prefactors change. The integral and inlet-flux conditions are equivalent once the local balance and nose conditions hold.

The physical approximations are [lubrication theory](../../../../../lubrication-theory.md), negligible inertia, slowly varying surface height, small pore-scale [Reynolds number](../../../../../reynolds-number.md), and negligible capillary entry pressure. Treating the substrate as vertically draining columns also requires its lateral flow to be negligible and its depth to exceed the penetration depth. The model is valid while surface liquid remains available above each draining column.

For a [similarity solution](../../../../../similarity-solution.md), let $h$ and $l$ scale as $t^a$, and let the current length scale as $t^b$. Since $h/l$ then has no time dependence, drainage requires $a-1=0$. Balancing $h_t$ with the horizontal spreading term gives $a-1=4a-2b$, so $a=1$ and $b=2$. These exponents also give injected volume $t^{a+b}=t^3$, explaining the particular supply law.

Define scales

$$
C=\left(\frac{\nu V_0^2}{g\tau^6}\right)^{1/5},\qquad
D=\left(\frac{gV_0^3}{\nu\tau^9}\right)^{1/5},
$$

which satisfy $CD=V_0/\tau^3$ and $D^2=(g/\nu)C^3$. The [cubic-input similarity for a draining gravity current](../../../../../cubic-input-similarity-for-a-draining-gravity-current.md) is

$$
\boxed{\xi=\frac{x}{Dt^2},\qquad h(x,t)=CtH(\xi),\qquad l(x,t)=CtL(\xi),\qquad
x_N(t)=\xi_N\left(\frac{gV_0^3}{\nu\tau^9}\right)^{1/5}t^2}.
$$

Substitution into the two conservation equations gives

$$
\boxed{H-2\xi H'-\frac13(H^3H')'=-K\left(1+\frac HL\right),\qquad
\phi(L-2\xi L')=K\left(1+\frac HL\right)},
$$

where

$$
K=\frac{gk/\nu}{C}=k\left(\frac{g^3\tau^3}{\nu^3V_0}\right)^{2/5}.
$$

Thus only $K$ and $\phi$ remain in the dimensionless problem. Its constraints are

$$
\begin{gathered}
H(\xi_N)=L(\xi_N)=0,\qquad H^3H'\to0\ \text{as }\xi\to\xi_N^-,\\
-H(0)^3H'(0)=9,\qquad
\int_0^{\xi_N}[H+\phi L]\,d\xi=1,\qquad H,L>0\ \text{for }0<\xi<\xi_N.
\end{gathered}
$$

Integrating the sum of the two [ordinary differential equations](../../../../../ordinary-differential-equation.md) verifies that the inlet flux and integral normalization agree. The dimensionless endpoint $\xi_N=\xi_N(K,\phi)$ is the undetermined multiplicative constant in the length law; solving for it is not required.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
