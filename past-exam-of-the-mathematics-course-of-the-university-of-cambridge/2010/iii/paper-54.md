# Paper 54

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper54.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper54.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Use signature $(-,+,+,+)$ and the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention $[\nabla_a,\nabla_b]X^c=R^c{}_{dab}X^d$. Lower the index of the [Killing vector field](../../../general-relativity.md#killing-vector-field) and set $T_{abc}=\nabla_a\nabla_bV_c$. Differentiating the [Killing equation](../../../general-relativity.md#killing-equation) gives $T_{abc}=-T_{acb}$, while the [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) gives

$$
T_{abc}-T_{bac}=-R^d{}_{cab}V_d.
$$

Define $S_{abc}=R_{cbad}V^d$. The first-pair antisymmetry of the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) gives $S_{abc}=-S_{acb}$. The pair symmetry and the [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity) give

$$
S_{abc}-S_{bac}=(R_{cbad}-R_{cabd})V^d=-R_{dcab}V^d.
$$

Thus $D=T-S$ is symmetric in its first two indices and antisymmetric in its last two. These two symmetries force it to vanish:

$$
D_{abc}=D_{bac}=-D_{bca}=-D_{cba}=D_{cab}=D_{acb}=-D_{abc}.
$$

Consequently $T_{abc}=R_{cbad}V^d$. Raising $c$ using [metric compatibility](../../../fiber-bundle.md#metric-compatibility) proves the required [second covariant derivative of a Killing vector](../../../general-relativity.md#second-covariant-derivative-of-a-killing-vector):

$$
\boxed{\nabla_a\nabla_bV^c=R^c{}_{bad}V^d.}
$$

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) has symmetric [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol), so antisymmetrization removes its connection terms. Hence the [Papapetrou electromagnetic field](../../../general-relativity.md#papapetrou-electromagnetic-field) is

$$
F_{ab}=\nabla_aV_b-\nabla_bV_a=2\nabla_aV_b,
$$

where the last equality uses the [Killing equation](../../../general-relativity.md#killing-equation). As a [differential two-form](../../../differential-form.md#2-form), $F=dV^\flat$, so the identity $d^2=0$ for the [exterior derivative](../../../differential-form.md#exterior-derivative) proves $\nabla_{[a}F_{bc]}=0$. Contracting the preceding [second covariant derivative of a Killing vector](../../../general-relativity.md#second-covariant-derivative-of-a-killing-vector) gives

$$
\nabla^a\nabla_aV_b=-R_{bd}V^d,
\qquad \nabla^aF_{ab}=-2R_{bd}V^d.
$$

A [vacuum spacetime](../../../general-relativity.md#vacuum-spacetime) here has $R_{ab}=0$, with no [cosmological constant](../../../cosmology.md#cosmological-constant). Therefore **both source-free Maxwell equations hold**:

$$
\boxed{\nabla_{[a}F_{bc]}=0,\qquad \nabla^aF_{ab}=0.}
$$

This is a test [electromagnetic field](../../../electromagnetism.md#electromagnetic-field) on the given [vacuum spacetime](../../../general-relativity.md#vacuum-spacetime); its own [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) is not included in that background's [Einstein field equations](../../../general-relativity.md#einstein-field-equations).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

In Cartesian coordinates $x=r\sin\theta\cos\phi$, $y=r\sin\theta\sin\phi$, $z=r\cos\theta$, the rotational [Killing vector field](../../../general-relativity.md#killing-vector-field) and its dual [differential one-form](../../../differential-form.md#one-form) are

$$
V=-y\partial_x+x\partial_y,\qquad V^\flat=-y\,dx+x\,dy.
$$

Therefore the [Papapetrou electromagnetic field](../../../general-relativity.md#papapetrou-electromagnetic-field) is

$$
F=dV^\flat=2\,dx\wedge dy.
$$

Choose the [electromagnetic field](../../../electromagnetism.md#electromagnetic-field) convention $F_{it}=E_i$ and $F_{ij}=\epsilon_{ijk}B^k$. There are no time components, and $F_{xy}=2$, so **this is a uniform magnetic field along the rotation axis, with no electric field**:

$$
\boxed{\mathbf E=0,\qquad \mathbf B=2\,\mathbf e_z.}
$$

Multiplying the [Killing vector field](../../../general-relativity.md#killing-vector-field) by $B_0/2$ produces any desired uniform [magnetic field](../../../electromagnetism.md#magnetic-field) strength $B_0$.

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

Write $f=1-2M/r$ in the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime). For the stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) $V=\partial_t$, its dual is $V^\flat=-f\,dt$ and the [Papapetrou electromagnetic field](../../../general-relativity.md#papapetrou-electromagnetic-field) is

$$
F=-f'\,dr\wedge dt=\frac{2M}{r^2}\,dt\wedge dr.
$$

Outside the [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon), use the static [orthonormal coframe](../../../general-relativity.md#orthonormal-coframe-in-spacetime) $e^{\hat0}=\sqrt f\,dt$, $e^{\hat r}=dr/\sqrt f$, $e^{\hat\theta}=r\,d\theta$, $e^{\hat\phi}=r\sin\theta\,d\phi$. Then $F=(2M/r^2)e^{\hat0}\wedge e^{\hat r}$. With the [electric field](../../../electromagnetism.md#electric-field) convention $E_{\hat i}=F_{\hat i\hat0}$ from the preceding part,

$$
\boxed{E_{\hat r}=-\frac{2M}{r^2},\qquad \mathbf B=0.}
$$

Thus the stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) gives a **Coulomb electric field**, directed inward in this convention. If the charge is normalized by $E_{\hat r}=Q/r^2$, its charge is $Q=-2M$. A convention with $F\mapsto-F$ reverses that charge; the invariant content is a radial monopole [electric field](../../../electromagnetism.md#electric-field) of magnitude $2M/r^2$.

For the axial [Killing vector field](../../../general-relativity.md#killing-vector-field) $V=\partial_\phi$, $V^\flat=r^2\sin^2\theta\,d\phi$, giving

$$
F=2r\sin^2\theta\,dr\wedge d\phi+2r^2\sin\theta\cos\theta\,d\theta\wedge d\phi.
$$

In the same static [orthonormal coframe](../../../general-relativity.md#orthonormal-coframe-in-spacetime), this is a purely [magnetic field](../../../electromagnetism.md#magnetic-field) with

$$
\boxed{B_{\hat r}=2\cos\theta,\qquad B_{\hat\theta}=-2\sqrt f\sin\theta,\qquad B_{\hat\phi}=0.}
$$

At large $r$ these are the spherical components of $2\mathbf e_z$. This is therefore the **regular magnetic test field asymptotic to a uniform axial field**, distorted by the [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime). Its net magnetic monopole flux is zero because the integral of $\cos\theta$ over a sphere vanishes. Both [electromagnetic fields](../../../electromagnetism.md#electromagnetic-field) are regular at the future [event horizon](../../../general-relativity.md#event-horizon): in [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates), the electric field is $(2M/r^2)dv\wedge dr$, and the magnetic two-form already contains only regular spatial coordinates. Static observers themselves cease to exist on the [event horizon](../../../general-relativity.md#event-horizon).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Put $r_+=\ell\sqrt M$ and $f=(r^2-r_+^2)/\ell^2$. The apparent failure of the nonrotating [BTZ black hole](../../../general-relativity.md#btz-black-hole) coordinates at $r=r_+$ is a [coordinate singularity](../../../general-relativity.md#coordinate-singularity). Define the [tortoise coordinate](../../../general-relativity.md#tortoise-coordinate) and ingoing time by

$$
r_* =\frac{\ell^2}{2r_+}\log\left|\frac{r-r_+}{r+r_+}\right|,
\qquad v=t+r_*.
$$

The [Ingoing BTZ coordinates](../../../general-relativity.md#ingoing-btz-coordinates) give

$$
ds^2=-f\,dv^2+2\,dv\,dr+r^2d\phi^2.
$$

All coefficients are analytic at $r_+>0$, and the determinant is $-r^2$, so the [metric tensor](../../../general-relativity.md#metric-tensor) extends nondegenerately through that radius. The [Killing vector field](../../../general-relativity.md#killing-vector-field) $K=\partial_v$ agrees with $\partial_t$ in the exterior. On $r=r_+$, $K^2=-f=0$ and $K_a=(dr)_a$. It is therefore both normal and tangent to this [null hypersurface](../../../general-relativity.md#null-hypersurface), proving that it is a [Killing horizon](../../../general-relativity.md#killing-horizon).

One may include both horizon branches and their [bifurcation surface](../../../general-relativity.md#bifurcation-surface) explicitly. Set $\kappa=r_+/\ell^2$, $u=t-r_*$ and, initially in the exterior, $U=-e^{-\kappa u}$, $V=e^{\kappa v}$. Then

$$
UV=-\frac{r-r_+}{r+r_+},\qquad
r=r_+\frac{1-UV}{1+UV},
\qquad
ds^2=-\frac{4\ell^2\,dU\,dV}{(1+UV)^2}+r_+^2\left(\frac{1-UV}{1+UV}\right)^2d\phi^2.
$$

This [analytic extension of a spacetime](../../../general-relativity.md#analytic-extension-of-a-spacetime) is regular near $UV=0$, and $K=\kappa(V\partial_V-U\partial_U)$ extends analytically. The surfaces $U=0$ and $V=0$ form the **extended Killing horizon at $r=r_+$**; $K$ vanishes only at their regular bifurcation circle.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Use the exterior-normalized [Killing vector field](../../../general-relativity.md#killing-vector-field) $K=\partial_t=\partial_v$ from the previous part. In [Ingoing BTZ coordinates](../../../general-relativity.md#ingoing-btz-coordinates), its only nonzero acceleration component on $r=r_+$ is

$$
K^b\nabla_bK^v=\Gamma^v{}_{vv}=\frac12f'(r_+),
\qquad K^b\nabla_bK^r=\frac12ff'\big|_{r_+}=0.
$$

The defining equation for [surface gravity](../../../general-relativity.md#surface-gravity), $\nabla_KK=\kappa K$, therefore gives the positive future-branch value

$$
\boxed{\kappa=\frac{f'(r_+)}2=\frac{r_+}{\ell^2}=\frac{\sqrt M}{\ell}.}
$$

This value uses exactly the prescribed [Killing vector field](../../../general-relativity.md#killing-vector-field) normalization. A constant rescaling of the [Killing vector field](../../../general-relativity.md#killing-vector-field) rescales its [surface gravity](../../../general-relativity.md#surface-gravity).

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Write $M=-a^2$ with $a>0$. On a constant-time slice, the proper distance from the axis to radius $r$ and the circumference at that radius are

$$
s(r)=\int_0^r\frac{dR}{\sqrt{a^2+R^2/\ell^2}}=\frac r a+O(r^3),
\qquad C(r)=2\pi r.
$$

Hence $C/s\to2\pi a$. A smooth axis in a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) requires the Euclidean limit $C/s\to2\pi$, so regularity forces $a=1$, or $M=-1$. For $a\ne1$ the [conical singularity of negative-mass BTZ geometry](../../../general-relativity.md#conical-singularity-of-negative-mass-btz-geometry) has deficit angle $2\pi(1-a)$; for $a>1$ this is an angular excess. Even integer $a>1$ is singular with the stipulated angular period $2\pi$: a multiple covering does not make the tip a smooth point.

At $M=-1$, set $r=\ell\sinh\chi$. The [metric tensor](../../../general-relativity.md#metric-tensor) becomes

$$
ds^2=-\cosh^2\chi\,dt^2+\ell^2(d\chi^2+\sinh^2\chi\,d\phi^2),
$$

which is regular at $\chi=0$ and describes [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime) with nonperiodic time. For every $M<0$, $f=a^2+r^2/\ell^2$ stays positive. An outward [radial null geodesic](../../../special-relativity.md#radial-null-geodesic) obeys $dt/dr=1/f$, and reaches the timelike conformal boundary in finite coordinate time, since $\int_0^\infty dr/f=\pi\ell/(2a)$. Thus no [event horizon](../../../general-relativity.md#event-horizon) hides the conical axis. **The geometry is nakedly singular except at $M=-1$.** Its local curvature away from the axis is that of [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime); the argument is a global angular-identification test, not curvature blowup.

## 2

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a curve with fixed $v,\theta,\phi$, its tangent is proportional to $\partial_r$. The [Vaidya metric](../../../general-relativity.md#vaidya-metric) has $g_{rr}=0$, so the curve is a [null curve](../../../special-relativity.md#null-curve). Moreover, the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) with two lower $r$ indices vanish:

$$
\Gamma^a{}_{rr}=\frac12g^{ab}(2\partial_rg_{br}-\partial_bg_{rr})=0,
$$

because $g_{vr}=1$ is constant and every other $g_{br}$ is zero. Thus the [covariant derivative](../../../general-relativity.md#covariant-derivative) along this tangent gives $\nabla_{\partial_r}\partial_r=0$. The [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) is satisfied with $r$ as an [affine parameter](../../../riemannian-geometry.md#affine-parameter); choosing future orientation gives the tangent $k=-\partial_r$ and an affine parameter increasing as $-r$. **These are the ingoing radial null geodesics.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the future-directed [null vector](../../../special-relativity.md#null-vector) $k=-\partial_r$, whose dual is $k_a=-(dv)_a$. The [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) has the [null dust](../../../general-relativity.md#null-dust) form

$$
T_{ab}=\varepsilon k_ak_b,\qquad \varepsilon=\frac{\dot m(v)}{4\pi r^2}.
$$

For every future-directed [timelike vector](../../../general-relativity.md#timelike-vector) $t$, $k\cdot t<0$. The energy current appearing in the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) is

$$
J^a=-T^a{}_bt^b=\varepsilon(-k\cdot t)k^a.
$$

If $\varepsilon\geq0$, this is a future-directed [null vector](../../../special-relativity.md#null-vector), or zero; also $T_{ab}t^at^b=\varepsilon(k\cdot t)^2\geq0$. If $\varepsilon<0$, the current is past-directed and that energy density is negative. Therefore, given the already stipulated positivity and smoothness of $m$, the necessary and sufficient additional condition is

$$
\boxed{\dot m(v)\geq0\quad\text{for every }v.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

An [event horizon](../../../general-relativity.md#event-horizon) is a [null hypersurface](../../../general-relativity.md#null-hypersurface). For its spherical defining function $H(v,r)=r-r_H(v)$, the inverse radial [metric tensor](../../../general-relativity.md#metric-tensor) has $g^{vv}=0$, $g^{vr}=1$ and $g^{rr}=f=1-2m(v)/r$. The normal's [null condition](../../../special-relativity.md#null-condition) is

$$
0=g^{ab}\partial_aH\partial_bH=f(v,r_H)-2\dot r_H.
$$

It follows that the [event horizon](../../../general-relativity.md#event-horizon) follows the outgoing [radial null geodesics of the Vaidya metric](../../../general-relativity.md#radial-null-geodesics-of-the-vaidya-metric):

$$
\boxed{2r_H\dot r_H=r_H-2m(v).}
$$

This [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) also describes other outgoing [null hypersurfaces](../../../general-relativity.md#null-hypersurface); the global [event horizon](../../../general-relativity.md#event-horizon) is selected by its future boundary condition, not by this local equation alone.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

In the final [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime), an outgoing ray with $r>2M_1$ escapes to [future null infinity](../../../general-relativity.md#future-null-infinity), whereas one with $r<2M_1$ cannot do so and ends at the [Schwarzschild singularity](../../../general-relativity.md#schwarzschild-singularity). Their boundary is the outgoing [null geodesic](../../../special-relativity.md#null-geodesic) $r=2M_1$. Since the final region continues indefinitely, the boundary of the [causal past](../../../general-relativity.md#causal-past) of [future null infinity](../../../general-relativity.md#future-null-infinity) there is exactly that [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon). Equivalently, integrating the outgoing equation backward from this final boundary selects the complete [event horizon](../../../general-relativity.md#event-horizon). Thus

$$
\boxed{r_H(v)=2M_1\qquad(v>v_0).}
$$

The original [Penrose diagram](../../../general-relativity.md#penrose-diagram) below shows the right-hand exterior and black-hole interior appropriate to ingoing coordinates. The green band is the ingoing accretion interval; the dashed blue curve is the spherical [apparent horizon](../../../general-relativity.md#apparent-horizon) $r=2m(v)$. Outgoing [null geodesics](../../../special-relativity.md#null-geodesic) escaping to [future null infinity](../../../general-relativity.md#future-null-infinity) lie to the right of the red [event horizon](../../../general-relativity.md#event-horizon); those to its left terminate on the future spacelike singularity. In the final stationary region the two horizons coincide. The red [event horizon](../../../general-relativity.md#event-horizon) already lies outside $r=2M_0$ before the ingoing matter arrives, because its position is fixed by the future escape criterion.

<a id="2/d/image-penrose-diagram-of-accretion-onto-a-pre-existing-schwarzschild-black-hole"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54-vaidya-penrose.png)

**[Figure 1](#2/d/image-penrose-diagram-of-accretion-onto-a-pre-existing-schwarzschild-black-hole). Penrose diagram of accretion onto a pre-existing Schwarzschild black hole**.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Let $\Delta M=M_1-M_0$ and retain only terms first order in $\mu/M_0$ and $\rho/M_0$. The outgoing [event horizon](../../../general-relativity.md#event-horizon) equation expands to

$$
4M_0\dot\rho=\rho-2\mu,
\qquad \dot\rho-\kappa_0\rho=-\frac{\mu}{2M_0},
\qquad \kappa_0=\frac1{4M_0}.
$$

Here $\kappa_0$ is the initial [Schwarzschild surface gravity](../../../general-relativity.md#schwarzschild-surface-gravity). The [integrating factor](../../../differential-equation.md#integrating-factor) $e^{-\kappa_0v}$ gives $d(e^{-\kappa_0v}\rho)/dv=-e^{-\kappa_0v}\mu/(2M_0)$. Future stationarity imposes $\rho=2\Delta M$ for $v>v_0$ and removes the growing homogeneous solution. Integrating from $v$ to infinity yields the [teleological response of a Vaidya event horizon](../../../general-relativity.md#teleological-response-of-a-vaidya-event-horizon):

$$
\boxed{\rho(v)=\frac1{2M_0}\int_v^\infty e^{-\kappa_0(s-v)}\mu(s)\,ds.}
$$

The integral is finite because $\mu$ is bounded. Integrating by parts also gives

$$
\rho(v)=2\mu(v)+2\int_v^\infty e^{-\kappa_0(s-v)}\dot\mu(s)\,ds.
$$

For $v>v_0$, this reduces to $2\Delta M$. For $v<0$, the first form becomes

$$
\rho(v)=C e^{\kappa_0v},\qquad C=\frac1{2M_0}\int_0^\infty e^{-\kappa_0s}\mu(s)\,ds.
$$

Consequently **$r_H\to2M_0$ as $v\to-\infty$**. The positive constant $C$ shows that this [event horizon](../../../general-relativity.md#event-horizon) is already expanding in the initially vacuum region. For monotone accretion, $\rho-2\mu\geq0$, so it lies outside the instantaneous [apparent horizon](../../../general-relativity.md#apparent-horizon) to first order. All displayed radius corrections are understood up to $O((\Delta M)^2/M_0)$.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

The [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) is already first order, so its energy flux can be evaluated on the unperturbed [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon) $r=2M_0$, with the infinity-normalized [Killing vector field](../../../general-relativity.md#killing-vector-field) $\xi=\partial_v$. On this background $g^{rv}=1$, and hence

$$
T^r{}_b\xi^b=T^r{}_v=T_{vv}=\frac{\dot\mu}{4\pi(2M_0)^2}.
$$

The conserved [stress-energy current from a Killing vector](../../../general-relativity.md#stress-energy-current-from-a-killing-vector) is $J^a=-T^a{}_b\xi^b$. Its radial component is negative, so the positive inward energy flux is $-J^r$. Using the directed null-surface measure $r_H^2\,dv\,d\Omega$ gives

$$
\Delta E=\int_{-\infty}^{\infty}\int_{S^2}T^r{}_v(2M_0)^2\,d\Omega\,dv
=\int_{-\infty}^{\infty}\dot\mu(v)\,dv
=\boxed{\Delta M}.
$$

The initial and final [event horizon](../../../general-relativity.md#event-horizon) areas are $A_0=16\pi M_0^2$ and $A_1=16\pi(M_0+\Delta M)^2$. Thus $\Delta A=32\pi M_0\Delta M+O((\Delta M)^2)$. With [Schwarzschild surface gravity](../../../general-relativity.md#schwarzschild-surface-gravity) $\kappa_0=1/(4M_0)$, the [Physical-process first law of black-hole mechanics](../../../general-relativity.md#physical-process-first-law-of-black-hole-mechanics) follows:

$$
\boxed{\Delta E=\Delta M=\frac{\kappa_0}{8\pi}\Delta A+O((\Delta M)^2/M_0).}
$$

The flux is [Killing energy](../../../general-relativity.md#killing-energy), including gravitational redshift, rather than the energy measured by a sequence of static observers arbitrarily close to the [event horizon](../../../general-relativity.md#event-horizon).

## 3

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Locally write the [null hypersurface](../../../general-relativity.md#null-hypersurface) as $S=0$ with $dS\ne0$, and extend its normal as $n_a=\nabla_aS$. On the hypersurface, $n^an_a=0$, so $n^a\nabla_aS=n^2=0$: the raised normal is itself tangent. The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and symmetry of the scalar Hessian give

$$
n^b\nabla_bn_a=n^b\nabla_an_b=\frac12\nabla_a(n^2).
$$

Although $n^2$ vanishes on the hypersurface, it need not vanish off it. Its tangential derivatives vanish, so $\nabla_a(n^2)$ must be proportional to the normal $n_a$. Hence $\nabla_nn=\kappa n$ on the hypersurface for some smooth local coefficient $\kappa$. The normal's [integral curves of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) remain in the hypersurface and satisfy the nonaffine [geodesic equation](../../../riemannian-geometry.md#geodesic-equation). Rescale to $k=hn$, where $n(\log h)=-\kappa$ along each generator. Direct substitution gives $\nabla_kk=0$. Thus **the normal generates null geodesics within the hypersurface**, with an [affine parameter](../../../riemannian-geometry.md#affine-parameter) after this rescaling. This proves the [null hypersurface normal generates null geodesics](../../../general-relativity.md#null-hypersurface-normal-generates-null-geodesics) property without incorrectly setting a transverse derivative of $n^2$ to zero.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose the affine tangent $k^a$ to a [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence), and an auxiliary [null vector](../../../special-relativity.md#null-vector) $\ell^a$ with $k\cdot\ell=-1$. The [screen-space projector](../../../geodesic-congruence.md#screen-space-projector)

$$
q_{ab}=g_{ab}+k_a\ell_b+\ell_ak_b
$$

annihilates $k$ and $\ell$ and restricts to a positive-definite two-dimensional metric in four spacetime dimensions. Neighboring transverse rays have relative displacement governed by the [optical tensor](../../../geodesic-congruence.md#optical-tensor)

$$
B_{ab}=q_a{}^cq_b{}^d\nabla_dk_c.
$$

Its irreducible decomposition defines the three requested optical quantities:

$$
\boxed{\theta=q^{ab}B_{ab},\qquad
\sigma_{ab}=B_{(ab)}-\frac12\theta q_{ab},\qquad
\omega_{ab}=B_{[ab]}.}
$$

The [null expansion](../../../geodesic-congruence.md#null-expansion) $\theta$ is the fractional rate of change of transverse area, $d\log A/d\lambda$. The [null shear](../../../geodesic-congruence.md#null-shear) $\sigma$ changes a beam's shape at fixed area to first order; it is symmetric and trace-free. The [null twist](../../../geodesic-congruence.md#null-twist) $\omega$ is antisymmetric and measures local rotation of the transverse rays; it vanishes for a hypersurface-orthogonal [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence). In $D$ dimensions replace $1/2$ by $1/(D-2)$. These definitions use the trace convention for [null expansion](../../../geodesic-congruence.md#null-expansion), rather than the alternative screen-averaged convention.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Take an affinely parametrized [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence), $\nabla_kk=0$. Choose the auxiliary [null vector](../../../special-relativity.md#null-vector) and a transverse orthonormal screen basis to undergo [parallel transport](../../../fiber-bundle.md#parallel-transport) along each ray. For the unprojected tensor $C_{ab}=\nabla_bk_a$, the product rule and the [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) yield

$$
\begin{aligned}
k^c\nabla_cC_{ab}
&=\nabla_b(k^c\nabla_ck_a)-(\nabla_bk^c)(\nabla_ck_a)
+k^c[\nabla_c,\nabla_b]k_a\\
&=-(\nabla_bk^c)(\nabla_ck_a)-R_{acbd}k^ck^d.
\end{aligned}
$$

Here the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention is the one in Question 1; its last-index antisymmetry converts the covector commutator to the displayed curvature term. Because $C_{ab}k^a=C_{ab}k^b=0$, inserting the [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) in the product term adds only terms killed by these contractions. Parallel propagation makes differentiation commute with the screen projection. Therefore, in screen indices $A,B$,

$$
\frac{dB_{AB}}{d\lambda}=-B_{AC}B^C{}_B-R_{AcBd}k^ck^d.
$$

This is the optical matrix evolution equation. Its trace has curvature contraction $q^{ab}R_{acbd}k^ck^d=R_{cd}k^ck^d$: the additional terms in $q^{ab}-g^{ab}$ vanish by curvature antisymmetry. Write $B=(\theta/2)q+\sigma+\omega$ using the [null expansion](../../../geodesic-congruence.md#null-expansion), [null shear](../../../geodesic-congruence.md#null-shear), and [null twist](../../../geodesic-congruence.md#null-twist). Symmetric--antisymmetric cross terms have zero trace, $\sigma$ is trace-free, and

$$
\operatorname{tr}(B^2)=\frac12\theta^2+\sigma_{ab}\sigma^{ab}-\omega_{ab}\omega^{ab}.
$$

The minus sign in the last trace comes from $\omega_{ab}=-\omega_{ba}$ and the positive screen metric. Taking the trace therefore derives the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation):

$$
\boxed{\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}+\omega_{ab}\omega^{ab}-R_{ab}k^ak^b.}
$$

For a nonaffine tangent obeying $\nabla_kk=\kappa k$, the same product-rule derivation adds $+\kappa\theta$ on the right; the projected derivative of $\kappa$ multiplies $k_a$ and vanishes. In $D$ dimensions the quadratic [null expansion](../../../geodesic-congruence.md#null-expansion) term is $-\theta^2/(D-2)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Away from a bifurcation set, the normal to a [Killing horizon](../../../general-relativity.md#killing-horizon) is its nonzero [Killing vector field](../../../general-relativity.md#killing-vector-field) $K$. Any affine tangent to the same generators has the form $k=hK$. In the [optical tensor](../../../geodesic-congruence.md#optical-tensor), derivatives of $h$ contribute a factor of $K_a$ and disappear under the [screen-space projector](../../../geodesic-congruence.md#screen-space-projector). Consequently

$$
B_{(ab)}=h\,q_a{}^cq_b{}^d\nabla_{(d}K_{c)}=0
$$

by the [Killing equation](../../../general-relativity.md#killing-equation). The trace and trace-free symmetric part are therefore zero: $\theta=0$ and $\sigma_{ab}=0$.

For the antisymmetric part, locally the horizon normal is proportional to a gradient. The restriction of its dual one-form to every tangent direction on the horizon is zero. Taking its [exterior derivative](../../../differential-form.md#exterior-derivative) and evaluating on two screen tangents therefore gives zero as well; equivalently this is the hypersurface-orthogonality consequence of the [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem). Since both screen indices are tangential, $B_{[ab]}=0$. Thus the [optical scalars on a Killing horizon](../../../general-relativity.md#optical-scalars-on-a-killing-horizon) satisfy

$$
\boxed{\theta=0,\qquad\sigma_{ab}=0,\qquad\omega_{ab}=0.}
$$

No affine normalization of the [Killing vector field](../../../general-relativity.md#killing-vector-field) itself was assumed. At a regular [bifurcation surface](../../../general-relativity.md#bifurcation-surface), $K$ vanishes but the smooth null generators do not; the conclusions for their optical quantities follow by continuity along each horizon branch.

## 4

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work initially in units $G=c=\hbar=k_B=1$ and consider gravitational collapse settling to a nonextremal [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime). Classically, outgoing rays sufficiently close to the forming [event horizon](../../../general-relativity.md#event-horizon) suffer an arbitrarily large redshift. Quantum mechanically, the meaning of [positive frequency](../../../quantum-field-theory.md#positive-frequency-solution) at [past null infinity](../../../general-relativity.md#past-null-infinity) differs from that at [future null infinity](../../../general-relativity.md#future-null-infinity); a [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation) between these two mode descriptions can therefore mix [creation operators](../../../quantum-mechanics.md#creation-operator) and [annihilation operators](../../../quantum-mechanics.md#annihilation-operator). Hawking's argument computes that mixing and obtains a thermal occupation, even when the incoming state has no particles.

To see why the frequency mixing is universal, use final [Schwarzschild time](../../../general-relativity.md#schwarzschild-time) $t$, the [Schwarzschild tortoise coordinate](../../../general-relativity.md#schwarzschild-tortoise-coordinate) $r_*$, and retarded time $u=t-r_*$. Near the final [event horizon](../../../general-relativity.md#event-horizon), $r_*\sim(2\kappa)^{-1}\log(r-2M)$, with [Schwarzschild surface gravity](../../../general-relativity.md#schwarzschild-surface-gravity) $\kappa=1/(4M)$. On a fixed advanced-time section, $u=v-2r_*$, so $r-2M$ is proportional to $e^{-\kappa u}$. Tracing a ray back through the regular collapsing region maps this small separation smoothly to its separation from the last escaping incoming ray. If $U$ is an affine incoming [null coordinate](../../../general-relativity.md#null-coordinate) and $U_H$ labels that limiting ray, the [Hawking exponential ray map](../../../general-relativity.md#hawking-exponential-ray-map) is

$$
U_H-U=Ae^{-\kappa u}(1+o(1)),\qquad A>0.
$$

The logarithm at a simple horizon root fixes the exponent. Smooth propagation through the earlier collapse changes $A$ and phases but not the leading exponential redshift.

For a massless bosonic test [scalar field](../../../quantum-field-theory.md#scalar-field), an outgoing mode of frequency $\omega>0$ at [future null infinity](../../../general-relativity.md#future-null-infinity) behaves as $e^{-i\omega u}$. Trace it backward in the high-frequency [geometric optics](../../../optics.md#geometrical-optics) approximation. Its relevant incoming dependence is, up to normalization and a phase,

$$
p_\omega(U)\sim\Theta(U_H-U)\left(\frac{U_H-U}{A}\right)^{ia},\qquad a=\frac\omega\kappa.
$$

Here $\Theta$ is the [Heaviside step function](../../../analysis.md#heaviside-step-function). Incoming rays with $U>U_H$ do not escape. This truncated logarithmic phase is not purely [positive frequency](../../../quantum-field-theory.md#positive-frequency-solution) with respect to $U$. Decomposing it into incoming [positive-frequency solutions](../../../quantum-field-theory.md#positive-frequency-solution) $e^{-i\omega' U}$ and negative modes $e^{+i\omega' U}$ gives the [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation). With $x=U_H-U$, the two relevant [Fourier transform](../../../analysis.md#fourier-transform) integrals are

$$
I_-(\omega')=\int_0^\infty x^{ia}e^{-(\epsilon+i\omega')x}\,dx,
\qquad
I_+(\omega')=\int_0^\infty x^{ia}e^{-(\epsilon-i\omega')x}\,dx,
\qquad\epsilon>0.
$$

The former is the positive-frequency coefficient and the latter is the negative-frequency coefficient; the [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) introduces the same frequency normalization into their modulus ratio. By the defining integral of the [gamma function](../../../complex-analysis.md#gamma-function) and analytic continuation in its Laplace parameter,

$$
I_\mp=\Gamma(1+ia)(\epsilon\pm i\omega')^{-1-ia}.
$$

For a complex number $z$ in the right half-plane, $|z^{-1-ia}|=|z|^{-1}e^{a\arg z}$. As $\epsilon\downarrow0$, the two arguments tend to $+\pi/2$ and $-\pi/2$. This gives the [thermal ratio of Hawking Bogoliubov coefficients](../../../general-relativity.md#thermal-ratio-of-hawking-bogoliubov-coefficients):

$$
\boxed{\frac{|\beta_{\omega\omega'}|^2}{|\alpha_{\omega\omega'}|^2}=e^{-2\pi\omega/\kappa}.}
$$

The regulator fixes the branches and is essential to the sign of the thermal exponent.

Expand the outgoing annihilator as $b=\int d\omega'(\alpha_{\omega\omega'}^*a_{\omega'}-\beta_{\omega\omega'}^*a_{\omega'}^\dagger)$, including a complete set of incoming channels. The [canonical identities for a bosonic Bogoliubov transformation](../../../quantum-field-theory.md#canonical-identities-for-a-bosonic-bogoliubov-transformation) express $[b,b^\dagger]=1$. For normalized outgoing [wave packets](../../../wave-equation.md#wave-packet), they give $\int(|\alpha|^2-|\beta|^2)\,d\omega'=1$. In the incoming [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum), the outgoing mean of the [particle number operator](../../../quantum-mechanics.md#number-operator) is $N_\omega=\int|\beta|^2\,d\omega'$. Combining the two identities with the thermal ratio, in the late-time narrow-frequency packet limit, yields

$$
N_\omega=\frac1{e^{2\pi\omega/\kappa}-1},\qquad
\boxed{T_H=\frac\kappa{2\pi}=\frac1{8\pi M}.}
$$

[Wave packets](../../../wave-equation.md#wave-packet) avoid interpreting the divergent normalization of infinitely long continuum modes as a finite particle count. The temperature is the [Hawking temperature](../../../general-relativity.md#hawking-temperature), and the occupation is the zero-chemical-potential [Bose-Einstein distribution](../../../statistical-physics.md#bose-einstein-distribution). Restoring constants, the [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime) temperature is $T_H=\hbar c^3/(8\pi G M k_B)$ for physical mass $M$.

The preceding thermal occupation describes the horizon-originating channel before exterior scattering. The exterior angular and curvature potential partly reflects it. For a [scalar field](../../../quantum-field-theory.md#scalar-field), the number flux at [future null infinity](../../../general-relativity.md#future-null-infinity) is consequently

$$
\frac{dN}{dt\,d\omega}=\frac1{2\pi}\sum_{\ell=0}^\infty(2\ell+1)\frac{\Gamma_\ell(\omega)}{e^{\omega/T_H}-1},
$$

where the [greybody factor](../../../general-relativity.md#greybody-factor) $\Gamma_\ell$ is the transmission probability of a partial wave. Multiplication by $\omega$ gives its energy flux. Thus the asymptotic spectrum has the thermal denominator but is not an exact blackbody spectrum. For fermionic fields the [canonical anticommutation relations](../../../quantum-mechanics.md#canonical-anticommutation-relations) replace the minus sign in the occupation denominator by a plus sign, at the same [Hawking temperature](../../../general-relativity.md#hawking-temperature).

The relevant state is the [collapse vacuum for Hawking radiation](../../../general-relativity.md#collapse-vacuum-for-hawking-radiation): no incoming thermal bath at [past null infinity](../../../general-relativity.md#past-null-infinity), and regular short-distance behavior in freely falling coordinates at the forming [event horizon](../../../general-relativity.md#event-horizon). It predicts an outgoing flux, unlike equilibrium with a thermal bath on an eternal [black hole](../../../general-relativity.md#black-hole). The derivation uses [quantum field theory in curved spacetime](../../../quantum-field-theory.md#quantum-field-theory-in-curved-spacetime) on a prescribed classical geometry; it does not require outgoing particles to follow forbidden classical paths out of the interior. Positive energy carried to infinity is accompanied, in the semiclassical description, by negative Killing-energy flux into the [black hole](../../../general-relativity.md#black-hole). Including that flux in slow backreaction decreases its [mass](../../../classical-mechanics.md#mass), giving [black-hole evaporation](../../../general-relativity.md#black-hole-evaporation).

The approximation applies to the late radiation of a large nonextremal [black hole](../../../general-relativity.md#black-hole) while its [surface gravity](../../../general-relativity.md#surface-gravity) changes slowly on a time scale $\kappa^{-1}$. Backward propagation involves very high locally measured frequencies, so the calculation assumes the usual regular short-distance quantum-field state. It determines the leading radiation and temperature, not the Planck-scale endpoint of [black-hole evaporation](../../../general-relativity.md#black-hole-evaporation). **The exponential horizon redshift forces positive/negative frequency mixing with a thermal ratio, giving outgoing Hawking radiation at $T_H=\kappa/(2\pi)$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
