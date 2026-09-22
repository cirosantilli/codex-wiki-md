<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use constant [porosity](../../../../../porosity.md) $\phi$, isotropic rock [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) $K$, common liquid [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu$ and [gravitational acceleration](../../../../../gravitational-acceleration.md) $g$. Treat the two liquids as separated by a sharp interface, with negligible capillary [pressure](../../../../../pressure.md), molecular mixing, ambient-current resistance and inertia. At distances beyond the initial source scale the current is shallow relative to its horizontal length, so its [pressure](../../../../../pressure.md) is hydrostatic. The initial release is symmetric about $x=0$ and has actual liquid volume $V$ per unit length of source. Consequently its geometric thickness [integral](../../../../../integral.md) is $V/\phi$, not $V$.

Below the interface the excess [pressure](../../../../../pressure.md) relative to the ambient hydrostatic field is $p'=\Delta\rho g(h-z)$, so [Darcy law](../../../../../darcy-law.md) gives horizontal discharge $q_x=-K\Delta\rho g h_x/\mu$. The vertically integrated discharge is $Q_x=-K\Delta\rho g hh_x/\mu$. Take the specified downward leakage $v=\gamma h$ to mean [Darcy flux](../../../../../darcy-velocity.md) per bulk horizontal area. [Mass conservation](../../../../../mass-conservation.md) then gives

$$
\phi h_t+\partial_xQ_x=-\gamma h,
\qquad
\boxed{h_t=\beta(hh_x)_x-\lambda h,\quad
\beta=\frac{K\Delta\rho g}{\mu\phi},\quad\lambda=\frac\gamma\phi.}
$$

If $v$ is instead defined as interstitial seepage speed, the actual leakage discharge is $\phi v$ and the corresponding coefficient is $\lambda=\gamma$. Stating the [velocity](../../../../../velocity.md) convention removes that otherwise ambiguous [porosity](../../../../../porosity.md) factor. For a shale of thickness $d_s$ and permeability $K_s$, a simple hydrostatic leakage model has $\gamma=K_s\Delta\rho g/(\mu d_s)$, if the reservoir below it has the same ambient [pressure](../../../../../pressure.md) reference and no capillary entry threshold.

Let $R(t)$ be the half-width of the support; the full end-to-end length will be $L(t)=2R(t)$. Appropriate conditions are symmetry $h_x(0,t)=0$, $h(\pm R,t)=0$, no flux beyond the support, and the moving-front condition $\dot R=-\beta h_x(R^-,t)$. Initially $\phi h(x,t)\,dx$ converges weakly to $V\delta_0$, expressing the concentrated line release. The equations describe the spreading [porous gravity current](../../../../../porous-gravity-current.md), not the singular immediate release itself.

With $\lambda=0$, conserved volume and balance of $h_t$ against $\beta(hh_x)_x$ give width proportional to $t^{1/3}$ and height proportional to $t^{-1/3}$. Write $h=t^{-1/3}f(\eta)$, $\eta=x/t^{1/3}$. Substitution gives

$$
-\frac13(f+\eta f')=\beta(ff')'.
$$

Integrating from the symmetry axis gives $\beta ff'=-\eta f/3$. Inside the support $f>0$, so $f'=-\eta/(3\beta)$ and $f=A-\eta^2/(6\beta)$. Thus the compact [Barenblatt solution](../../../../../barenblatt-solution.md) is

$$
\boxed{h(x,t)=\frac{[R(t)^2-x^2]_+}{6\beta t}.}
$$

The positive-part notation makes $h=0$ outside the current. Volume fixes its remaining constant:

$$
\frac V\phi=\int_{-R}^Rh\,dx=\frac{2R^3}{9\beta t},\qquad
\boxed{R(t)=\left(\frac{9\beta Vt}{2\phi}\right)^{1/3},\quad L(t)=2\left(\frac{9\beta Vt}{2\phi}\right)^{1/3}.}
$$

If “length” denotes the distance from the source to one front, it is $R$ rather than $L$; both conventions are given explicitly. Differentiating gives $\dot R=R/(3t)=-\beta h_x(R^-,t)$, so the front condition holds. Using $V/2$ on each reflecting half-line gives the same normalization.

For positive leakage define actual retained volume $\mathcal V(t)=\phi\int h\,dx$. Since the edge thickness and boundary flux vanish, integration of the equation yields

$$
\boxed{\frac{d\mathcal V}{dt}=-\lambda\mathcal V,\qquad\mathcal V(t)=Ve^{-\lambda t}.}
$$

Put $h=e^{-\lambda t}H(x,\tau)$, where $\tau=(1-e^{-\lambda t})/\lambda$. Because $\dot\tau=e^{-\lambda t}$, substitution cancels the leakage term and leaves $H_\tau=\beta(HH_x)_x$. This derives the [exponential drainage transform for porous-medium diffusion](../../../../../exponential-drainage-transform-for-porous-medium-diffusion.md). Its conserved geometric volume is still $V/\phi$, so

$$
\boxed{h(x,t)=e^{-\lambda t}\frac{[R(t)^2-x^2]_+}{6\beta\tau(t)},\qquad
R(t)=\left[\frac{9\beta V}{2\phi\lambda}(1-e^{-\lambda t})\right]^{1/3}.}
$$

The full length is again $L(t)=2R(t)$. In particular,

$$
\boxed{R_\infty=\left(\frac{9\beta V}{2\phi\lambda}\right)^{1/3},\qquad L_\infty=2R_\infty.}
$$

At early times $\tau\sim t$, recovering impermeable-bed spreading. At late times, drainage reduces the current thickness and therefore its hydrostatic driving [pressure](../../../../../pressure.md); the effective spreading time saturates at $1/\lambda$. The current approaches a finite horizontal reach while its retained volume and thickness vanish exponentially. This does not mean a positive-volume pool remains at a finite final depth. For small positive $\lambda$ the length scale diverges as $\lambda^{-1/3}$, consistently with unbounded spreading when leakage is absent.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
