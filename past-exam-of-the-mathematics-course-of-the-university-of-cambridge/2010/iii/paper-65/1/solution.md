<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the boundary to be horizontal, put $z=0$ on it, and let $z=h(x,t)$ be the interface. Write $\Delta\rho=\rho-\rho_2>0$. Under the long-thin [hydrostatic approximation](../../../../../hydrostatic-approximation.md), the deep ambient fluid has pressure $p_2=p_* -\rho_2gz$ to leading order, with negligible horizontal pressure gradient. Matching [pressure](../../../../../pressure.md) at the interface gives, inside the dense [porous gravity current](../../../../../porous-gravity-current.md),

$$
p=p_* -\rho gz+\Delta\rho g h(x,t),\qquad p_x=\Delta\rho g h_x.
$$

The [Darcy velocity](../../../../../darcy-velocity.md) is superficial volume flux per total area, not pore speed. The horizontal [Darcy law](../../../../../darcy-law.md) and depth-integrated flux therefore give

$$
u_D=-\frac{k\Delta\rho g}{\mu}h_x,\qquad
q=\int_0^h u_D\,dz=-\frac{k\Delta\rho g}{\mu}hh_x.
$$

The [porosity](../../../../../porosity.md) $\phi$ multiplies storage, so [mass conservation](../../../../../mass-conservation.md) is $\phi h_t+q_x=0$. Consequently

$$
\boxed{h_t=\lambda(hh_x)_x,\qquad\lambda=\frac{k\Delta\rho g}{\phi\mu}.}
$$

The deep-ambient and long-thin assumptions are what permit neglecting the ambient return-flow pressure variation, vertical inertia, and nonhydrostatic pressure corrections.

For a localized finite release, first use the reflecting half-line $x\geq0$, so $h_x(0,t)=0$. Let $S=V/\phi$ be the conserved cross-sectional area of the current; $V$ here is actual pore-fluid volume per unit cross-flow distance. A [similarity solution](../../../../../similarity-solution.md) of the [porous medium equation](../../../../../porous-medium-equation.md) has thickness proportional to $t^{-\alpha}$ and extent proportional to $t^\beta$. Conservation gives $\alpha=\beta$, and balancing $h_t$ against $(hh_x)_x$ gives $\alpha+2\beta=1$. Thus $\alpha=\beta=1/3$. Put

$$
L_*=(\lambda St)^{1/3},\qquad
h=\frac S{L_*}F(\xi),\qquad\xi=\frac x{L_*}.
$$

Substitution gives $-(F+\xi F')/3=(FF')'$. Zero flux at $\xi=0$ allows one integration: $FF'=-\xi F/3$. In the positive-current region, $F'=-\xi/3$, so $F=(\xi_f^2-\xi^2)/6$. The normalization $\int_0^{\xi_f}F\,d\xi=1$ gives $\xi_f^3=9$. The [one-sided constant-volume porous gravity current](../../../../../one-sided-constant-volume-porous-gravity-current.md) is therefore

$$
\boxed{h(x,t)=\frac{[L(t)^2-x^2]_+}{6\lambda t},\qquad
L(t)=\left(\frac{9\lambda Vt}{\phi}\right)^{1/3}.}
$$

Here $[a]_+=\max(a,0)$. Its [Darcy flux](../../../../../darcy-velocity.md) vanishes at the moving front because $h=0$ there, and its physical volume is $\phi\int_0^Lh\,dx=V$. This is the exact concentrated-release [Barenblatt solution](../../../../../barenblatt-solution.md) of the depth equation, physically used after the short initial adjustment to a long-thin current; an arbitrary finite initial patch requires its initial profile as well as its volume, although the same profile describes the usual late spreading regime. If a line release spreads symmetrically in both directions and $V$ denotes the total volume, use the same parabola on $-L<x<L$ with $L^3=9\lambda Vt/(2\phi)$. If instead volume has already been divided by porosity, replace $V/\phi$ by that geometric volume.

Drainage at superficial rate $\phi\Gamma h$ changes [mass conservation](../../../../../mass-conservation.md) to $\phi h_t+q_x=-\phi\Gamma h$, so

$$
\boxed{h_t=\lambda(hh_x)_x-\Gamma h.}
$$

For constant $\Gamma>0$, use the [exponential drainage transform for porous-medium diffusion](../../../../../exponential-drainage-transform-for-porous-medium-diffusion.md)

$$
h=e^{-\Gamma t}H(x,\tau),\qquad
\tau(t)=\frac{1-e^{-\Gamma t}}\Gamma.
$$

Indeed, $h_t+\Gamma h=e^{-\Gamma t}\tau'H_\tau$ and $(hh_x)_x=e^{-2\Gamma t}(HH_x)_x$. Choosing $\tau'=e^{-\Gamma t}$ leaves $H_\tau=\lambda(HH_x)_x$. Substituting the undrained [Barenblatt solution](../../../../../barenblatt-solution.md) gives

$$
\boxed{h(x,t)=e^{-\Gamma t}\frac{[L_d(t)^2-x^2]_+}{6\lambda\tau(t)},\qquad
L_d(t)=\left(\frac{9\lambda V\tau(t)}\phi\right)^{1/3}.}
$$

Use the factor $1/2$ in $L_d^3$ for a total-volume symmetric release, as above. For general initial data the same transform is exact, but $H$ is the corresponding undrained solution rather than automatically a source parabola.

The remaining physical volume is $V(t)=Ve^{-\Gamma t}$. Early times have $\tau\sim t$, recovering undrained spreading. Late times have $\tau\to1/\Gamma$, so **the front approaches a finite runout while the current drains exponentially**:

$$
\boxed{L_d\longrightarrow\left(\frac{9\lambda V}{\phi\Gamma}\right)^{1/3},\qquad V(t)=Ve^{-\Gamma t}.}
$$

The front slows because drainage reduces the hydrostatic driving head. The finite transformed time also explains why drainage does not guarantee that an arbitrary initial profile reaches its undrained universal large-time shape.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
