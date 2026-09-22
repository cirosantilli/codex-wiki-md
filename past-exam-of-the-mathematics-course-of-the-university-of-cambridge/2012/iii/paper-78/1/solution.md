<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let the fluid approach a uniform, quiescent state $(\rho_0,p_0,c_0)$ at infinity. Use the outward unit [normal vector](../../../../../normal-vector.md) $N=\nabla f/|\nabla f|$, pointing from the object into the fluid. Write $H=H(f)$ for the [Heaviside step function](../../../../../heaviside-step-function.md), $q=\rho-\rho_0$, and $\delta_S=\delta(f)|\nabla f|$. With the [viscous stress tensor](../../../../../viscous-stress-tensor.md) $\tau_{ij}$, define

$$
P_{ij}=(p-p_0)\delta_{ij}-\tau_{ij},\qquad T_{ij}=\rho u_i u_j+P_{ij}-c_0^2q\delta_{ij},\qquad L_i=P_{ij}N_j.
$$

Thus $T_{ij}$ is the [Lighthill stress tensor](../../../../../lighthill-stress-tensor.md), and $L_i$ is the surface loading exerted on the fluid. The total [force](../../../../../force.md) on the object has the opposite sign. Extend $q$ by zero inside the object. Since the boundary is fixed and impermeable, $u\cdot N=0$, and the distributional [mass conservation](../../../../../mass-conservation.md) and [momentum conservation](../../../../../momentum-conservation.md) equations are

$$
\partial_t(Hq)+\partial_i(H\rho u_i)=0,
$$



$$
\partial_t(H\rho u_i)+c_0^2\partial_i(Hq)+\partial_j(HT_{ij})=L_i\delta_S.
$$

For example, the surface contribution to the momentum equation is $(\rho u_i u_j+P_{ij})N_j\delta_S=L_i\delta_S$. Differentiating the first equation in time and subtracting the divergence of the second gives the fixed-body [Ffowcs Williams-Hawkings equation](../../../../../ffowcs-williams-hawkings-equation.md):

$$
\boxed{(\partial_t^2-c_0^2\Delta)(Hq)=\partial_i\partial_j(HT_{ij})-\partial_i(L_i\delta_S).}
$$

There is no [acoustic thickness noise](../../../../../acoustic-thickness-noise.md): a fixed impermeable boundary injects no mass. Apply the [retarded acoustic Green function](../../../../../retarded-acoustic-green-function.md) $\delta(t-R/c_0)/(4\pi c_0^2R)$, where $R=|x-y|$. The supplied surface-delta identity converts the loading term to a surface integral. For an exterior observer, the required integral equation is

$$
\boxed{q(x,t)=\frac{1}{4\pi c_0^2}\partial_{x_i}\partial_{x_j}\int_{f(y)>0}\frac{T_{ij}(y,t-R/c_0)}{R}\,d^3y-\frac{1}{4\pi c_0^2}\partial_{x_i}\int_{f(y)=0}\frac{L_i(y,t-R/c_0)}{R}\,dS_y.}
$$

This [acoustic analogy](../../../../../acoustic-analogy.md) is an exact rearrangement of the fluid equations; source approximations enter later. In the distant linear acoustic region, $p'=c_0^2q$.

The [acoustic far field](../../../../../acoustic-far-field.md) requires observer distance $r$ much larger than the source extent $\ell$ and $k_0r\gg1$, so derivatives of the retarded phase dominate derivatives of $1/R$. The [acoustic compact-source approximation](../../../../../acoustic-compact-source-approximation.md) requires $k_0\ell\ll1$, so the source's differential propagation delays can be neglected. These conditions concern different lengths and neither implies the other. Put $n=x/r$, $t_r=t-r/c_0$, and define the loading and stress moments

$$
F_i(t)=\int_S L_i(y,t)\,dS_y,\qquad Q_{ij}(t)=\int_{f>0}T_{ij}(y,t)\,d^3y.
$$

The leading compact [acoustic far field](../../../../../acoustic-far-field.md) is

$$
\boxed{p'(x,t)\simeq\frac{1}{4\pi r}\left[\frac{n_i}{c_0}\dot F_i(t_r)+\frac{n_i n_j}{c_0^2}\ddot Q_{ij}(t_r)\right].}
$$

The surface term is an [acoustic dipole](../../../../../acoustic-dipole.md); the volume term is an [acoustic quadrupole](../../../../../acoustic-quadrupole.md). The plus sign of the loading term follows from the minus sign of its spatial divergence and the derivative of retarded time.

For the power comparison, assume low [Mach number](../../../../../mach-number.md) $M=U/c_0$, high [Reynolds number](../../../../../reynolds-number.md), eddy size $\ell$, characteristic time $\tau=\ell/U$, and stress magnitude $\rho_0U^2$. Keep the prescribed turbulent region and its leading volume stress comparable when inserting the object; neglect changes of source statistics and exceptional cancellations of the leading moments. Compactness follows from $\ell/(c_0\tau)=M\ll1$. Since $Q\sim\rho_0U^2\ell^3$ and the outgoing [acoustic intensity](../../../../../acoustic-energy-flux.md) is $\langle p'^2\rangle/(\rho_0c_0)$, the volume power is

$$
\boxed{\mathcal P_Q\sim\frac{\rho_0U^8\ell^2}{c_0^5}=\rho_0c_0^3\ell^2M^8.}
$$

If the object's size is comparable to $\ell$ and its fluctuating resultant loading is $F\sim\rho_0U^2\ell^2$, then

$$
\boxed{\mathcal P_D\sim\frac{\rho_0U^6\ell^2}{c_0^3}=\rho_0c_0^3\ell^2M^6,\qquad \mathcal P_D/\mathcal P_Q\sim M^{-2}.}
$$

Angular factors and dimensionless loading coefficients have been omitted. The [acoustic dipole](../../../../../acoustic-dipole.md) and [acoustic quadrupole](../../../../../acoustic-quadrupole.md) interference vanishes in the leading power integrated over a full sphere, by odd angular parity; individual directions can show interference.

A size threshold also requires a loading model. For a small nonseparating object of size $a\ll\ell$ in an approximately inviscid, smoothly varying incident eddy, a spatially uniform pressure has zero resultant on its closed surface. The first surviving loading is the pressure-gradient or [added mass](../../../../../added-mass.md) force, $F\sim\rho_0a^3U/\tau=\rho_0U^2a^3/\ell$. Under these explicitly stated assumptions,

$$
\mathcal P_D\sim\frac{\rho_0U^6a^6}{c_0^3\ell^4},\qquad \frac{\mathcal P_D}{\mathcal P_Q}\sim\frac{(a/\ell)^6}{M^2}.
$$

**The two mechanisms become comparable at $a\sim\ell M^{1/3}$; for smaller objects the cases with and without the object have the same leading order of power.** This is the [small-body loading-noise threshold](../../../../../small-body-loading-noise-threshold.md). It is not a geometry-independent size law: a separated drag force $F\sim\rho_0U^2a^2$ fluctuating on the original eddy time instead gives $\mathcal P_D/\mathcal P_Q\sim(a/\ell)^4/M^2$ and $a\sim\ell\sqrt M$. If both force and time are set by body-scale eddies, $\tau=a/U$, their loading power is $\rho_0U^6a^2/c_0^3$ and comparison with the original volume source gives $a\sim M\ell$. Each estimate states which source time and force it uses.

The physical distinction is [momentum conservation](../../../../../momentum-conservation.md). Unforced turbulence in a fluid supplies internal stresses, whose net-force contribution cancels and leaves [acoustic quadrupole](../../../../../acoustic-quadrupole.md) radiation. The supported object exchanges momentum with the fluid and the external support, permitting a time-dependent resultant [force](../../../../../force.md) and [acoustic dipole](../../../../../acoustic-dipole.md) radiation. One fewer retarded derivative makes the loading radiation more efficient at low [Mach number](../../../../../mach-number.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
