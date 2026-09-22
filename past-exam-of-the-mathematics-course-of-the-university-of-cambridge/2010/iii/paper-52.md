# Paper 52

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper52.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper52.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use geometric units $G=c=1$, [metric signature](../../../topology.md#metric-signature) $(-+++)$, and a [four-velocity](../../../special-relativity.md#four-velocity) normalized by the physical metric. Write $\phi=1+\Phi$, where $|\Phi|\ll1$. For a pressureless [perfect fluid](../../../general-relativity.md#perfect-fluid), the [dust stress-energy tensor](../../../general-relativity.md#dust-stress-energy-tensor) is $T_{ij}=\rho U_iU_j$ and $g^{ij}U_iU_j=-1$. Since $\eta^{ij}=\phi^2g^{ij}$, its background trace is

$$
\eta^{ij}T_{ij}=-\rho\phi^2.
$$

Consequently the field equation is $(-\partial_t^2+\Delta)\phi=4\pi\rho\phi^3$. Neglecting time derivatives and higher weak-field orders gives the [Newtonian limit of Nordstrom gravity](../../../general-relativity.md#newtonian-limit-of-nordstrom-gravity):

$$
\boxed{\Delta\Phi=4\pi\rho,\qquad\Phi=\phi-1.}
$$

The constant shift between $\phi$ and $\Phi$ does not affect the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) or the force. Here $\rho$ is the physical rest density; if fluid indices are instead defined using the background metric, the intermediate powers of $\phi$ change but the same leading-order equation results.

For the motion, the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) of the [conformally flat metric](../../../general-relativity.md#conformally-flat-metric) is

$$
\Gamma^i{}_{jk}=\delta^i_j\partial_k\log\phi+\delta^i_k\partial_j\log\phi-\eta_{jk}\eta^{i\ell}\partial_\ell\log\phi.
$$

In particular $\Gamma^\alpha{}_{00}=\partial_\alpha\log\phi$. Replacing the [affine parameter](../../../riemannian-geometry.md#affine-parameter) in the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) by coordinate time gives, with $w^i=(1,\boldsymbol v)$ and $\boldsymbol v=d\boldsymbol x/dt$,

$$
\frac{d^2x^\alpha}{dt^2}=-\Gamma^\alpha{}_{ij}w^iw^j+\Gamma^0{}_{ij}w^iw^jv^\alpha
=-(1-|\boldsymbol v|^2)\left(\partial_\alpha\log\phi+v^\alpha\partial_t\log\phi\right).
$$

At small speeds and for a nearly static field, this becomes

$$
\boxed{\frac{d^2\boldsymbol x}{dt^2}=-\boldsymbol\nabla\Phi.}
$$

Thus the [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) and freely falling trajectories agree to the stated weak-field, slow-motion order. The comparison is an approximation, not an exact equivalence of relativistic trajectories.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

**Yes, at the weak-field accuracy of the experiment.** The [Pound-Rebka experiment](../../../general-relativity.md#pound-rebka-experiment) measures [gravitational redshift](../../../general-relativity.md#gravitational-redshift), which [Nordstrom theory of gravitation](../../../general-relativity.md#nordstrom-s-theory-of-gravitation) predicts even though it does not predict bending of light.

In a static field, a stationary clock has $d\tau=\phi\,dt$. A [photon](../../../quantum-mechanics.md#photon) has constant [Killing energy](../../../general-relativity.md#killing-energy) $E=-p_t$, and an observer at rest has $U=\phi^{-1}\partial_t$. Its measured frequency is proportional to $-p_iU^i=E/\phi$. Emission at $e$ and reception at $r$ therefore give

$$
\boxed{\frac{\nu_r}{\nu_e}=\frac{\phi_e}{\phi_r}
=1+\Phi_e-\Phi_r+O(\Phi^2).}
$$

An upward ray has $\Phi_r-\Phi_e\simeq gH/c^2$ when ordinary units are restored, so $\Delta\nu/\nu\simeq-gH/c^2$. This is the shift tested using the [Mössbauer effect](../../../physics.md#mossbauer-effect). The [gravitational redshift](../../../general-relativity.md#gravitational-redshift) follows from the physical clock rates; a claim that straight light paths imply no frequency shift would confuse two different observables.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**No: the theory predicts zero gravitational deflection of light.** The reason is [conformal preservation of null geodesic paths](../../../general-relativity.md#conformal-preservation-of-null-geodesic-paths). Along a [null geodesic](../../../special-relativity.md#null-geodesic) with tangent $k^i$, the [geodesic equation for a conformally flat metric](../../../general-relativity.md#geodesic-equation-for-a-conformally-flat-metric) reduces to

$$
\frac{dk^i}{d\lambda}+2\frac{d\log\phi}{d\lambda}k^i=0,
$$

because $\eta_{ij}k^ik^j=0$. The acceleration is parallel to the tangent and changes only its parametrization. Equivalently, with $\ell^i=\phi^2k^i$, $d\ell^i/d\lambda=0$, so the unparametrized ray is a straight [null geodesic](../../../special-relativity.md#null-geodesic) of [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime). A positive [conformal factor](../../../general-relativity.md#conformal-factor) also preserves local angles, so this straight-path result cannot be hidden by changing the local angle measurement. It contradicts the nonzero solar deflection observed in [gravitational lensing](../../../general-relativity.md#gravitational-lensing), while remaining compatible with the [gravitational redshift](../../../general-relativity.md#gravitational-redshift) in part (b).

## 2

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [linearized coordinate gauge transformation](../../../general-relativity.md#linearized-coordinate-gauge-transformation) changes the identification of points of the perturbed [spacetime](../../../special-relativity.md#spacetime) with its [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) background. With $x'^i=x^i+\epsilon\xi^i$, the same physical metric has perturbation

$$
h'_{ij}=h_{ij}-\partial_i\xi_j-\partial_j\xi_i.
$$

These changes are coordinate freedom, not extra physical [gravitational wave polarizations](../../../general-relativity.md#gravitational-wave-polarization). Raising indices with $\eta$, define $h=\eta^{ij}h_{ij}$ and the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation) $\bar h_{ij}=h_{ij}-\eta_{ij}h/2$. Then

$$
\bar h'_{ij}=\bar h_{ij}-\partial_i\xi_j-\partial_j\xi_i+\eta_{ij}\partial_k\xi^k.
$$

The first-order [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is $\Gamma^{(1)k}{}_{ij}=\tfrac12\eta^{k\ell}(\partial_ih_{j\ell}+\partial_jh_{i\ell}-\partial_\ell h_{ij})$. Contracting the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) in the stated convention gives

$$
R^{(1)}_{ij}=\tfrac12\left(\partial_i\partial_kh^k{}_j+\partial_j\partial_kh^k{}_i-\Box h_{ij}-\partial_i\partial_jh\right),
\qquad R^{(1)}=\partial_i\partial_jh^{ij}-\Box h.
$$

Put $A_j=\partial^i\bar h_{ij}$. The corresponding [Einstein tensor](../../../general-relativity.md#einstein-tensor) is

$$
G^{(1)}_{ij}=-\tfrac12\Box\bar h_{ij}
+\tfrac12\left(\partial_iA_j+\partial_jA_i-\eta_{ij}\partial^kA_k\right).
$$

Under the [linearized coordinate gauge transformation](../../../general-relativity.md#linearized-coordinate-gauge-transformation), $A'_j=A_j-\Box\xi_j$. Choosing a solution of $\Box\xi_j=A_j$ imposes [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity), $A'_j=0$. Thus the vacuum [Einstein field equations](../../../general-relativity.md#einstein-field-equations) reduce to

$$
\boxed{\partial^i\bar h_{ij}=0,\qquad\Box\bar h_{ij}=0.}
$$

There remains [residual gauge symmetry of linearized gravity](../../../general-relativity.md#residual-gauge-symmetry-of-linearized-gravity) with $\Box\xi_j=0$.

For the transverse profiles, write both symmetric off-diagonal entries as $h_{xy}=h_{yx}=h_\times(t-z)$ and the diagonal entries as $h_{xx}=-h_{yy}=h_+(t-z)$. The [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation) has zero trace and therefore equals $h$. Its divergence vanishes: its only nonzero index directions are $x,y$, while its coefficients depend only on $t-z$. Also $(-\partial_t^2+\partial_z^2)F(t-z)=0$ for every twice differentiable profile $F$. These are consequently [plane gravitational waves in linearized gravity](../../../general-relativity.md#plane-gravitational-wave-in-linearized-gravity) in [transverse-traceless gauge](../../../general-relativity.md#transverse-traceless-gauge), with the two independent [gravitational wave polarizations](../../../general-relativity.md#gravitational-wave-polarization) $h_+$ and $h_\times$.

To calculate the detector response, use a [parallel-propagated orthonormal frame](../../../general-relativity.md#parallel-propagated-orthonormal-frame) along the centre of a short nonrotating stick. To first order its clock reads $t$, and the tidal curvature is

$$
R_{A0B0}=-\frac\epsilon2\ddot h_{AB}+O(\epsilon^2),\qquad A,B\in\{x,y\}.
$$

For a [sliding-bead gravitational wave detector](../../../general-relativity.md#sliding-bead-gravitational-wave-detector), the stick constrains transverse motion but supplies no axial restoring force. Projecting [geodesic deviation](../../../general-relativity.md#geodesic-deviation) along an $x$-directed stick gives

$$
\ddot L=\frac\epsilon2\ddot h_+(t-z_0)L_0+O(\epsilon^2).
$$

Here $L$ is the proper separation and $L_0=L(t_0)$, with $\dot L(t_0)=0$. Integrating with those actual initial conditions yields

$$
\boxed{L(t)=L_0\left[1+\frac\epsilon2\left(h_+(t-z_0)-h_+(t_0-z_0)
-(t-t_0)\dot h_+(t_0-z_0)\right)\right]+O(\epsilon^2).}
$$

For beads at rest before an incident wave, both initial profile terms vanish and the familiar result is $\boxed{L(t)=L_0[1+\epsilon h_+(t-z_0)/2]+O(\epsilon^2)}$. The cross polarization produces a transverse tidal force, balanced by the guide, and no axial first-order displacement in this orientation. In [transverse-traceless gauge](../../../general-relativity.md#transverse-traceless-gauge) the same plus response can be read from the proper line element, $d\ell=\sqrt{1+\epsilon h_+}\,dx$; coordinate distances alone are not measured distances. When a cross polarization is present, keeping the guide physically nonrotating may require transverse coordinate adjustments, which do not change the axial answer at this order.

For a $z$-directed stick, $R_{z0z0}=0$ and the wave is transverse. Therefore **beads initially at rest retain their proper separation to first order**: $L(t)=L_0+O(\epsilon^2)$. The tidal calculation is the usual linear detector limit, with bead spacing small compared with the wavelength; it does not treat a macroscopic rigid body as exactly rigid over arbitrary relativistic distances.

## 3

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Assume $M>0$ and use geometric units. The stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) $K=\partial_t$ gives the conserved [Killing energy](../../../general-relativity.md#killing-energy) $E=-g(K,U)=f\dot t$. For radial motion, normalization of the [four-velocity](../../../special-relativity.md#four-velocity) gives $-f\dot t^2+f^{-1}\dot r^2=-1$. Combining these identities yields

$$
\boxed{f\dot t=E,\qquad \dot r^2+f=E^2.}
$$

At rest at infinity, $f\to1$ and $\dot r\to0$, so $E=1$. Choose the inward branch $\dot r=-\sqrt{2M/r}$. Its [proper time](../../../special-relativity.md#proper-time) from the [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon) to the [curvature singularity](../../../general-relativity.md#curvature-singularity) is

$$
\boxed{\Delta\tau=\int_0^{2M}\sqrt{\frac r{2M}}\,dr=\frac{4M}{3}.}
$$

In ordinary units this is $4GM/(3c^3)$. The endpoint $r=0$ is not a regular centre of the [spacetime](../../../special-relativity.md#spacetime). This is the [Schwarzschild horizon-to-singularity proper time for fall from infinity](../../../general-relativity.md#schwarzschild-horizon-to-singularity-proper-time-for-fall-from-infinity), rather than a universal time for all infall energies.

For this [geodesic congruence](../../../geodesic-congruence.md), set $w(r)=\sqrt{2M/r}$. Its [four-velocity](../../../special-relativity.md#four-velocity) and metric dual are

$$
U=f^{-1}\partial_t-w\partial_r,
\qquad U_a\,dx^a=-dt-f^{-1}w\,dr.
$$

The right side is an exact one-form because $w/f$ depends only on $r$. Thus $U_a=-\partial_a\tau$, with [free-fall proper time in Schwarzschild spacetime](../../../general-relativity.md#free-fall-proper-time-in-schwarzschild-spacetime) determined by

$$
\boxed{d\tau=dt+\frac{w}{f}\,dr,\qquad
\tau=t+2\sqrt{2Mr}+2M\log\left|\frac{\sqrt r-\sqrt{2M}}{\sqrt r+\sqrt{2M}}\right|+\text{constant}.}
$$

Indeed $U^a\partial_a\tau=-U^aU_a=1$, so this scalar advances by the actual [proper time](../../../special-relativity.md#proper-time) on every member of the infalling [geodesic congruence](../../../geodesic-congruence.md), with a synchronized choice of additive offsets.

Substitution of $dt=d\tau-wf^{-1}dr$ in the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) gives

$$
-f\,dt^2+f^{-1}dr^2=-f\,d\tau^2+2w\,d\tau\,dr+dr^2.
$$

Using $f=1-w^2$, the [Painlevé–Gullstrand coordinates](../../../general-relativity.md#painleve-gullstrand-coordinates) therefore have

$$
\boxed{ds^2=-d\tau^2+(dr+w\,d\tau)^2+r^2d\Sigma^2.}
$$

All coefficients are finite at $r=2M$; the determinant of the $\tau,r$ block is $-f-w^2=-1$. Hence the horizon is a [coordinate singularity](../../../general-relativity.md#coordinate-singularity) of [Schwarzschild time](../../../general-relativity.md#schwarzschild-time), not a degeneracy of the metric. The new spatial slices have $d\ell^2=dr^2+r^2d\Sigma^2$, the flat Euclidean metric, and $g^{ab}\partial_a\tau\partial_b\tau=-1$ makes their normals the freely falling [four-velocities](../../../special-relativity.md#four-velocity). By contrast, the curvature scalar $R_{abcd}R^{abcd}=48M^2/r^6$ diverges at $r=0$; this genuine singularity is not removed.

For [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates), use $v=t+r_*$ with $dr_*/dr=f^{-1}$, for example $r_*=r+2M\log|r/(2M)-1|$. Then

$$
ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Sigma^2.
$$

Both constructions cross the future horizon. Their time functions have different meanings: $v=\text{constant}$ is an ingoing [null hypersurface](../../../general-relativity.md#null-hypersurface), whereas $\tau=\text{constant}$ is a flat spacelike hypersurface orthogonal to the infallers. Thus the former is adapted to ingoing [null geodesics](../../../special-relativity.md#null-geodesic), and the latter to a timelike free-fall clock congruence.

For the [Kruskal diagram](../../../general-relativity.md#kruskal-diagram), choose [Kruskal–Szekeres coordinates](../../../general-relativity.md#kruskal-szekeres-coordinates) with $U_K=-e^{-(t-r_*)/(4M)}$, $V_K=e^{(t+r_*)/(4M)}$ in the right exterior and extend them across its horizon. They obey

$$
U_KV_K=\left(1-\frac r{2M}\right)e^{r/(2M)},\qquad
ds^2=-\frac{32M^3}{r}e^{-r/(2M)}dU_K\,dV_K+r^2d\Sigma^2.
$$

The four regions of [Kruskal spacetime](../../../general-relativity.md#kruskal-spacetime) are I, the right exterior $(U_K<0,V_K>0)$; II, the future [black hole](../../../general-relativity.md#black-hole) $(U_K>0,V_K>0)$; III, the other exterior $(U_K>0,V_K<0)$; and IV, the past [white hole](../../../general-relativity.md#white-hole) $(U_K<0,V_K<0)$. The null axes are horizons, their intersection is the bifurcation two-sphere, and the spacelike boundaries $U_KV_K=1$ are the future and past curvature singularities. A point in this radial diagram represents a symmetry two-sphere.

<a id="3/image-kruskal-extension-with-both-exteriors-black-hole-and-white-hole-the-ingoing-painleve-gullstrand-domain-is-shaded-blue"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-52-kruskal.png)

**[Figure 1](#3/image-kruskal-extension-with-both-exteriors-black-hole-and-white-hole-the-ingoing-painleve-gullstrand-domain-is-shaded-blue). Kruskal extension with both exteriors, black hole and white hole; the ingoing Painlevé-Gullstrand domain is shaded blue**.

The [domain of the ingoing Painleve-Gullstrand chart](../../../general-relativity.md#domain-of-the-ingoing-painleve-gullstrand-chart) is **region I together with region II and their common future horizon**. More precisely, it is $V_K>0$, $U_KV_K<1$, or $r>0$ with finite $\tau$. To verify the boundary rather than infer it from the locally regular metric, put $\rho=\sqrt{r/(2M)}$ and write

$$
\tau=v+S(r),\qquad S(r)=4M\rho-2M\rho^2-4M\log(1+\rho).
$$

This follows by subtracting $r_*$ from the preceding radial primitive, and $S$ is finite at $r=2M$. Thus $V_K=\exp[(\tau-S(r))/(4M)]>0$ throughout the chart. Conversely every point with $V_K>0$ and $r>0$ gives a finite $\tau$. The past horizon $V_K=0$, the bifurcation sphere, region III and region IV are absent. Reversing the sign of the radial term produces the outgoing chart through the [white hole](../../../general-relativity.md#white-hole) instead.

## 4

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The radial part of the [Minkowski metric](../../../special-relativity.md#minkowski-metric) becomes $-du\,dv$, and $r=(v-u)/2$. With $u=\tan p$, $v=\tan q$ and the positive [conformal factor](../../../general-relativity.md#conformal-factor) $\Omega=2\cos p\cos q$, multiplication by $\Omega^2$ gives

$$
\Omega^2(-du\,dv)=-4\,dp\,dq=-dT^2+dR^2,
\qquad
\Omega^2r^2=(\cos p\cos q)^2(\tan q-\tan p)^2=\sin^2(q-p).
$$

Consequently the [Minkowski conformal compactification](../../../general-relativity.md#minkowski-conformal-compactification) is

$$
\boxed{ds^2=\Omega^{-2}\left(-dT^2+dR^2+\sin^2R\,d\Sigma^2\right),\qquad
\Omega=\cos T+\cos R.}
$$

The spatial metric $dR^2+\sin^2R\,d\Sigma^2$ is the round unit three-sphere. The extended unphysical metric is therefore that of the [Einstein static universe](../../../general-relativity.md#einstein-static-universe), $\mathbb R\times S^3$ with unit spatial radius. Physical [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) occupies only the diamond-shaped causal patch of this cylinder, or a triangle after restricting to nonnegative spherical radius; it is not the whole cylinder.

The complete coordinate ranges and joint restrictions are

$$
\begin{gathered}
t\in\mathbb R,\quad r\in[0,\infty),\quad\theta\in[0,\pi],\quad\phi\in[0,2\pi),\\
u,v\in\mathbb R,\quad u\le v,\\
-\frac\pi2<p\le q<\frac\pi2,\\
-\pi<T<\pi,\quad 0\le R<\pi,\quad |T|+R<\pi.
\end{gathered}
$$

The polar angles have the usual coordinate degeneracies at their poles and at $r=0$. In the extended [Einstein static universe](../../../general-relativity.md#einstein-static-universe) one may let $T\in\mathbb R$ and $0\le R\le\pi$, but these are not the ranges of the original physical patch. In its interior $\Omega>0$. The line $R=0$ is the regular centre $r=0$, not a component of infinity.

The [conformal completion](../../../general-relativity.md#conformal-completion) has [future timelike infinity](../../../general-relativity.md#future-timelike-infinity) $i^+=(\pi,0)$, [past timelike infinity](../../../general-relativity.md#past-timelike-infinity) $i^-=(-\pi,0)$, and [spacelike infinity](../../../general-relativity.md#spacelike-infinity) $i^0=(0,\pi)$. The open sloping boundaries are

$$
\mathcal I^+:T+R=\pi,\quad0<R<\pi,
\qquad
\mathcal I^-:T-R=-\pi,\quad0<R<\pi,
$$

namely [future null infinity](../../../general-relativity.md#future-null-infinity) and [past null infinity](../../../general-relativity.md#past-null-infinity). Each ordinary interior point of the radial diagram represents a two-sphere, and each point on either open null boundary represents a two-sphere of null directions.

<a id="4/image-minkowski-penrose-triangle-with-timelike-spacelike-and-null-infinities-the-regular-centre-and-representative-causal-and-spacelike-geodesics"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-52-penrose.png)

**[Figure 2](#4/image-minkowski-penrose-triangle-with-timelike-spacelike-and-null-infinities-the-regular-centre-and-representative-causal-and-spacelike-geodesics). Minkowski Penrose triangle with timelike, spacelike and null infinities, the regular centre and representative causal and spacelike geodesics**.

A [timelike geodesic](../../../general-relativity.md#timelike-geodesic) is an inertial worldline $\boldsymbol x=\boldsymbol b+\boldsymbol\beta t$ with $|\boldsymbol\beta|<1$. As $t\to+\infty$, both $t-r$ and $t+r$ tend to $+\infty$, giving $p,q\to\pi/2$ and endpoint $i^+$. At past infinity both tend to $-\infty$, giving $i^-$. These endpoints are reached at infinite physical [proper time](../../../special-relativity.md#proper-time), although at finite conformal coordinate time $T$. A [null geodesic](../../../special-relativity.md#null-geodesic) has $r\sim|t|$. In its outgoing future, $u$ approaches a finite retarded time while $v\to+\infty$, giving an endpoint on $\mathcal I^+$; in its incoming past, $v$ has a finite limit and $u\to-\infty$, giving an endpoint on $\mathcal I^-$. A [spacelike geodesic](../../../riemannian-geometry.md#spacelike-geodesic) is a straight line with spatial tangent larger than its temporal tangent, so $u\to-\infty$, $v\to+\infty$ at either end and both endpoints are $i^0$ in the compactified radial description. All these physical geodesics are complete. Only the unparametrized [null geodesics](../../../special-relativity.md#null-geodesic) are necessarily preserved as geodesics of the unphysical metric; timelike and spacelike images need not be its geodesics.

For horizons, distinguish a property of the [spacetime](../../../special-relativity.md#spacetime) from a property of an observer or of an initial-data hypersurface. Complete inertial observers have **no particle horizon**: in the flat cosmological slicing $a(t)=1$, the past light-travel distance $\int_{-\infty}^{t_0}dt$ is infinite. There is no finite-age initial singularity truncating communication between comoving observers. This statement does not say that an event receives signals from spacelike-separated events at the same time.

There is also no black-hole [event horizon](../../../general-relativity.md#event-horizon), because every event can send a future-directed null ray to [future null infinity](../../../general-relativity.md#future-null-infinity). Nevertheless **accelerated timelike observers can have both future and past observer event horizons**. For an entire observer worldline $\gamma$, define them by $H^+_\gamma=\partial I^-(\gamma)$ and $H^-_\gamma=\partial I^+(\gamma)$, using its complete future and past respectively. An inertial observer's chronological past and future of the whole worldline are both all of [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime). By contrast, for the uniformly accelerated worldline in a Cartesian spatial direction,

$$
t=a^{-1}\sinh(a\tau),\qquad x=a^{-1}\cosh(a\tau),\qquad y=z=0,
$$

its null coordinates obey $t-x=-a^{-1}e^{-a\tau}<0$ and $t+x=a^{-1}e^{a\tau}>0$. An event with $t-x<0$ can signal to a sufficiently late point of this worldline, whereas an event with $t-x\ge0$ cannot; finite transverse displacements do not change that conclusion as $t+x\to\infty$. Similarly the worldline can signal to precisely the events with $t+x>0$. Thus its two [observer event horizons](../../../general-relativity.md#observer-event-horizon) are

$$
\boxed{H^+_\gamma:\ t-x=0,\qquad H^-_\gamma:\ t+x=0.}
$$

They are the [Rindler horizons](../../../special-relativity.md#rindler-horizon), and their accessible common region is $x>|t|$. They do not indicate a [curvature singularity](../../../general-relativity.md#curvature-singularity) or a failure of global predictability.

Finally [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) is a [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime): every inextendible [causal curve](../../../general-relativity.md#causal-curve) crosses each complete spacelike plane $t=t_0$ exactly once. Indeed $t$ is strictly monotone along future-directed [causal curves](../../../general-relativity.md#causal-curve), and the speed bound $|d\boldsymbol x/dt|\le1$ prevents an inextendible curve from ending at finite $t$ by escaping to spatial infinity. Its time range is therefore all of $\mathbb R$. These planes are [Cauchy hypersurfaces](../../../general-relativity.md#cauchy-surface) with full [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence), so **there are no Cauchy horizons associated with complete Cauchy data**.

A [Cauchy horizon](../../../general-relativity.md#cauchy-horizon) is, however, defined relative to a specified initial surface. Under a literal existence reading of “admits”, non-Cauchy initial surfaces can have such horizons even in flat [spacetime](../../../special-relativity.md#spacetime). For example the edgeless spacelike hyperboloid $\Sigma_a:\ t=\sqrt{a^2+r^2}$ has $D(\Sigma_a)=\{t>r\}$. To see this, inside the future light cone $t-r$ and $t+r$ are positive and nondecreasing on future-directed [causal curves](../../../general-relativity.md#causal-curve). Their product $t^2-r^2$ increases past $a^2$ on every future-inextendible curve from below the hyperboloid; every past-inextendible curve from above it crosses down through $a^2$ before leaving the cone. Outside the cone there is an inextendible null curve avoiding the hyperboloid. The future light cone itself is its past [Cauchy horizon](../../../general-relativity.md#cauchy-horizon). The time-reversed hyperboloid gives a future [Cauchy horizon](../../../general-relativity.md#cauchy-horizon). This is the [dependence of a Cauchy horizon on the initial hypersurface](../../../general-relativity.md#dependence-of-a-cauchy-horizon-on-the-initial-hypersurface), not an intrinsic loss of predictability of full [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime). Thus a categorical claim that no choice of partial initial surface can ever have a Cauchy horizon would be too strong.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
