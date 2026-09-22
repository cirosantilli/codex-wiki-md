<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\chi=H(F)$ use the [Heaviside step function](../../../../../heaviside-step-function.md), and $\delta_s=|\nabla F|\delta(F)$, so that $\mathbf n_s=\nabla F/|\nabla F|$ points from the body into the fluid. The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) gives $F_t+\mathbf u\cdot\nabla F=0$ on the surface. In the exterior, [mass conservation](../../../../../mass-conservation.md) and the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) are

$$
\rho_t+\partial_i(\rho u_i)=0,\qquad
\partial_t(\rho u_i)+\partial_j(\rho u_iu_j+p\delta_{ij})=0.
$$

Products with $\chi$ are understood distributionally, using $\partial_t\chi=F_t\delta(F)$ and $\partial_i\chi=F_i\delta(F)$. With $\rho'=\rho-\rho_0$, the extended continuity equation is

$$
\partial_t(\rho'\chi)+\partial_i(\rho u_i\chi)=\rho_0\mathbf u\cdot\nabla F\,\delta(F).
$$

The corresponding extended momentum equation is

$$
\partial_t(\rho u_i\chi)+\partial_j[(\rho u_iu_j+p\delta_{ij})\chi]
=pF_i\delta(F),
$$

because its advective surface term is $\rho u_i(F_t+\mathbf u\cdot\nabla F)\delta(F)=0$. Differentiate continuity in time and substitute the divergence of momentum. Subtracting $c_0^2\nabla^2(\rho'\chi)$ gives the [Ffowcs Williams-Hawkings equation](../../../../../ffowcs-williams-hawkings-equation.md)

$$
\boxed{(\partial_t^2-c_0^2\nabla^2)(\rho'\chi)
=\partial_t(\rho_0\mathbf u\cdot\nabla F\,\delta(F))
-\partial_i(pF_i\delta(F))+\partial_i\partial_j(T_{ij}\chi),}
$$

where the inviscid [Lighthill stress tensor](../../../../../lighthill-stress-tensor.md) is

$$
T_{ij}=\rho u_iu_j+(p-c_0^2\rho')\delta_{ij}.
$$

If $p$ denotes total [pressure](../../../../../pressure.md), this tensor includes the constant ambient [pressure](../../../../../pressure.md) $p_0$. Its contribution $p_0\nabla^2\chi$ cancels the corresponding surface term exactly. For radiation integrals it is convenient to subtract $p_0$ from both terms, making $T_{ij}=\rho u_iu_j+(p'-c_0^2\rho')\delta_{ij}$ with $p'=p-p_0$. The displayed source identity is unchanged by this consistent [pressure](../../../../../pressure.md)-gauge subtraction.

Assume no incoming sound and no free initial acoustic field. Put $R_y=|\mathbf x-\mathbf y|$, $\tau_y=t-R_y/c_0$, $Q=\rho_0u_n\delta_s$, and $P_i=p'n_{s,i}\delta_s$. Convolution with the [retarded acoustic Green function](../../../../../retarded-acoustic-green-function.md) gives the three source integrals, for an observer outside the body:

$$
\boxed{\begin{aligned}
\rho'_m&=\frac1{4\pi c_0^2}\partial_t\int_{\mathbb R^3}\frac{Q(\mathbf y,\tau_y)}{R_y}\,d^3y,\\
\rho'_f&=-\frac1{4\pi c_0^2}\partial_{x_i}\int_{\mathbb R^3}\frac{P_i(\mathbf y,\tau_y)}{R_y}\,d^3y,\\
\rho'_S&=\frac1{4\pi c_0^2}\partial_{x_i}\partial_{x_j}\int_{\mathbb R^3}\frac{T_{ij}(\mathbf y,\tau_y)H(F(\mathbf y,\tau_y))}{R_y}\,d^3y.
\end{aligned}}
$$

These are the surface thickness, surface loading and volume quadrupole contributions. The retarded surface [Dirac delta distributions](../../../../../dirac-delta-function.md) must remain inside the integrals: integrating them over a moving retarded surface produces the [moving-surface retarded Jacobian](../../../../../moving-surface-retarded-jacobian.md), and is not generally the same as simply substituting one [retarded time](../../../../../retarded-time.md) into an instantaneous [surface integral](../../../../../surface-integral.md).

For an [acoustic compact-source approximation](../../../../../acoustic-compact-source-approximation.md), suppose the dominant sources have size $\ell$, source frequency scale $\omega$, and $\omega\ell/c_0\ll1$. Also require $r=|\mathbf x|\gg\ell$ and the [acoustic far field](../../../../../acoustic-far-field.md) $\omega r/c_0\gg1$. Then $R_y\simeq r-\mathbf n\cdot\mathbf y$, $1/R_y\simeq1/r$, and the leading source integrals use the common time $\tau=t-r/c_0$. Slow source motion relative to $c_0$ is implicit in this leading retardation approximation. Define

$$
m(t)=\rho_0\int_{S(t)}u_n\,dS,\qquad
f_i(t)=-\int_{S(t)}p'n_{s,i}\,dS,\qquad
S_{ij}(t)=\int_{F>0}T_{ij}\,d^3y.
$$

Thus $m$ is net displaced mass per unit time, $\mathbf f$ is the fluid [pressure](../../../../../pressure.md) [force](../../../../../force.md) on the body, and $S_{ij}$ is the integrated excess [Lighthill stress tensor](../../../../../lighthill-stress-tensor.md). The minus sign in $\mathbf f$ fixes the requested loading convention; the [force](../../../../../force.md) on the fluid is opposite. On the radiating $1/r$ terms, $\partial_{x_i}\simeq-(n_i/c_0)\partial_t$, giving

$$
\boxed{\rho'(\mathbf x,t)\simeq\frac{\dot m(\tau)}{4\pi r c_0^2}
-\frac{n_i\dot f_i(\tau)}{4\pi r c_0^3}
+\frac{n_in_j\ddot S_{ij}(\tau)}{4\pi r c_0^4}.}
$$

Spatial derivatives of $1/r$ produce near-field terms of orders $r^{-2}$ and $r^{-3}$, omitted here. Neglecting source delays is a separate approximation from discarding those observer near-field terms. If a leading integrated source vanishes by symmetry, its first nonzero delay correction can be as important as another retained multipole.

For the translating sphere, write its center as $\mathbf X(t)=a_1\cos(\omega t)\mathbf e$, with $\mathbf e$ a unit vector, and its [velocity](../../../../../velocity.md) as $\mathbf V=\dot{\mathbf X}$. Let $\mathcal V=4\pi a^3/3$, $\eta=a\omega/c_0\ll1$ and $d=a_1/a\ll1$. Impermeability gives $u_n=\mathbf V\cdot\mathbf n_s$. Since its volume is constant,

$$
\boxed{m=\rho_0\mathbf V\cdot\int_S\mathbf n_s\,dS=0,\qquad\rho'_{\dot m}=0}
$$

in the leading compact formula. The individual local thickness sources have scale $\rho_0(a_1/r)\eta^2$, but their net monopole cancels.

At first order in [amplitude](../../../../../wave-amplitude.md) and leading order in $\eta$, the exterior incompressible [velocity potential](../../../../../velocity-potential.md) is $\phi=-a^3\mathbf V\cdot\mathbf r_s/(2r_s^3)$, where $\mathbf r_s$ is measured from the mean center. It has $\partial_{r_s}\phi=\mathbf V\cdot\mathbf n_s$ at $r_s=a$. Linear [Bernoulli equation](../../../../../bernoulli-equation.md) gives $p'=-\rho_0\phi_t=(\rho_0a/2)\dot{\mathbf V}\cdot\mathbf n_s$ there. Since $\int n_{s,i}n_{s,j}dS=(4\pi a^2/3)\delta_{ij}$,

$$
\mathbf f=-M_a\dot{\mathbf V},\qquad M_a=\frac12\rho_0\mathcal V=\frac{2\pi}3\rho_0a^3.
$$

This is the [added mass of a sphere](../../../../../added-mass-of-a-sphere.md). The explicit leading loading contribution is

$$
\boxed{\rho'_{\dot f}=\frac{M_a\mathbf n\cdot\ddot{\mathbf V}(\tau)}{4\pi r c_0^3}
=\frac{\rho_0a^3a_1\omega^3}{6r c_0^3}(\mathbf n\cdot\mathbf e)\sin(\omega\tau).}
$$

It scales as $\rho_0(a_1/r)\eta^3$. In homentropic small-[amplitude](../../../../../wave-amplitude.md) flow the volume stress is quadratic to leading order, $T_{ij}=O(\rho_0V^2)$ over volume $O(a^3)$, so the volume [acoustic quadrupole](../../../../../acoustic-quadrupole.md) has scale

$$
\rho'_S=O\left(\rho_0\frac{a_1^2}{ar}\eta^4\right).
$$

It is smaller than the linear dipole by $O(d\eta)=O(V/c_0)$ and can contain a second harmonic.

For completeness, the exact thickness-source integral has a nonzero first delay correction even though $m=0$. Its first spatial moment is

$$
M_j=\rho_0\int_Sy_j\mathbf V\cdot\mathbf n_s\,dS=\rho_0\mathcal V V_j.
$$

Expand its integrand at $\tau_y=\tau+\mathbf n\cdot\mathbf y/c_0$. The leading nonzero [translating-sphere acoustic thickness dipole](../../../../../translating-sphere-acoustic-thickness-dipole.md) is therefore

$$
\boxed{\rho'_{\rm th}=\frac{\rho_0\mathcal V\mathbf n\cdot\ddot{\mathbf V}(\tau)}{4\pi r c_0^3}
=\frac{\rho_0a^3a_1\omega^3}{3r c_0^3}(\mathbf n\cdot\mathbf e)\sin(\omega\tau).}
$$

It too scales as $\rho_0(a_1/r)\eta^3$. Thus zero net-volume monopole does not mean zero thickness radiation. The full leading linear sound, summing thickness and loading, is

$$
\boxed{\rho'_{\rm linear}=\frac{\rho_0a^3a_1\omega^3}{2r c_0^3}(\mathbf n\cdot\mathbf e)\sin(\omega\tau),\qquad p'_{\rm far}=c_0^2\rho'_{\rm linear}.}
$$

The leading compact equation gives the requested zero $\dot m$ and added-mass $\dot f$ terms; this extra delay calculation is necessary to obtain the complete linear field when its nominal monopole has cancelled.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
