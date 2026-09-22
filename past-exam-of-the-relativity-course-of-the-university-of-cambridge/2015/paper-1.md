# Paper 1

↑ **Parent:** [2015](../2015.md)

Original paper: [Public original PDF, physical pages 339–342; questions on pages 340–342](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=339).

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use [arc length](../../riemannian-geometry.md#arc-length) $s$ as the [affine parameter](../../riemannian-geometry.md#affine-parameter), and put a dot over derivatives with respect to $s$. The [geodesic Lagrangian](../../riemannian-geometry.md#geodesic-lagrangian) on the [sphere](../../euclidean-geometry.md#sphere) is

$$
L=\frac{a^2}{2}(\dot\theta^2+\sin^2\theta\,\dot\phi^2).
$$

The [cyclic coordinate](../../lagrangian-mechanics.md#cyclic-coordinate) $\phi$ gives $\partial L/\partial\dot\phi=a^2\sin^2\theta\,\dot\phi=\text{constant}$. With the constant normalized as in the paper,

$$
\boxed{\sin^2\theta\,\dot\phi=h.}
$$

Here $h$ has units of inverse length, because $s$ is physical [arc length](../../riemannian-geometry.md#arc-length). Unit-speed normalization gives

$$
a^2\dot\theta^2+\frac{a^2h^2}{\sin^2\theta}=1.
$$

For $h\ne0$, division by $\dot\phi^2$ yields the [spherical-geodesic first integral](../../differential-geometry.md#spherical-geodesic-first-integral)

$$
\boxed{\left(\frac{d\theta}{d\phi}\right)^2+V_1(\theta)=0,
\qquad V_1(\theta)=\sin^2\theta-\frac{\sin^4\theta}{a^2h^2}.}
$$

The turning latitudes satisfy $\sin\theta=|ah|$. In the usual polar-coordinate range $0\le\theta\le\pi$,

$$
\boxed{\theta_{\min}=\arcsin|ah|,\qquad
\theta_{\max}=\pi-\arcsin|ah|,\qquad 0<|ah|\le1.}
$$

The maximum departure from the equator, often the geometric quantity intended by an angular amplitude, is instead

$$
\boxed{\max|\theta-\pi/2|=\arccos|ah|.}
$$

Thus **[polar angle](../../multivariable-calculus.md#polar-angle) and signed latitude must not be interchanged**. At $|ah|=1$ the [geodesic](../../riemannian-geometry.md#geodesic) is the equator. At $h=0$ it is a meridian through the poles; $\phi$ cannot serve as a global parameter and the divided equation is inapplicable. The limiting polar range is then $[0,\pi]$.

The original PDF prints an ambiguous derivative with the square on $\theta$ rather than a conventional derivative notation. If the intended equation was second order, differentiating the first integral, or eliminating $\dot\theta$ from the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation), gives the equally useful form

$$
\boxed{\frac{d^2\theta}{d\phi^2}+V_2(\theta)=0,\qquad
V_2(\theta)=\sin\theta\cos\theta-
\frac{2\sin^3\theta\cos\theta}{a^2h^2}.}
$$

It has the same normalized [geodesics](../../riemannian-geometry.md#geodesic) and the same turning angles. Giving both forms resolves the typographical ambiguity without pretending that a second derivative is the square of a first derivative. Geometrically these trajectories are [great circles](../../euclidean-geometry.md#great-circle), with inclination $\arccos|ah|$ to the equator.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Assume an emitter at rest on the stellar surface and a static observer at infinity. Write $f(r)=1-2GM/(rc^2)$. The time-translation [Killing energy](../../killing-vector-field.md#killing-energy) of a [photon](../../quantum-mechanics.md#photon) is conserved, while the locally measured [photon](../../quantum-mechanics.md#photon) [energy](../../energy.md) is proportional to $1/\sqrt{f(r)}$. Consequently

$$
\frac{\nu_\infty}{\nu_R}=\sqrt{f(R)},\qquad
\boxed{1+z=\frac1{\sqrt{1-2GM/(Rc^2)}}.}
$$

Using $G=6.67430\times10^{-11}\ {\rm m^3\,kg^{-1}\,s^{-2}}$, $c=299792458\ {\rm m\,s^{-1}}$, $M=4\times10^{30}\ {\rm kg}$ and $R=1.1\times10^4\ {\rm m}$,

$$
\frac{2GM}{Rc^2}=0.54008438,\qquad
\boxed{z=0.4745548\simeq0.475.}
$$

The [Schwarzschild radius](../../schwarzschild-spacetime.md#schwarzschild-radius) is approximately $5.94\ {\rm km}$, below the given surface radius. The positive shift is therefore a [gravitational redshift](../../general-relativity.md#gravitational-redshift) of an escaping [photon](../../quantum-mechanics.md#photon), with received wavelength about $1.475$ times the emitted wavelength. A moving emitter would introduce an additional [Doppler factor](../../special-relativity.md#doppler-factor); that is outside this static-surface model. The weak-field estimate $z\simeq GM/(Rc^2)=0.270$ is insufficient at this compactness. These stated constants are numerical conventions, not a claim about an unavailable historical handbook's last digits.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use [metric signature](../../topological-manifold.md#metric-signature) $(+---)$ and [four-velocities](../../special-relativity.md#four-velocity) $U_i^a=\gamma_i c(1,\boldsymbol\beta_i)$, with $\gamma_i=(1-\beta_i^2)^{-1/2}$. Their [Lorentz invariant](../../special-relativity.md#lorentz-invariance) [inner product](../../inner-product.md) is

$$
\frac{U_1\cdot U_2}{c^2}
=\gamma_1\gamma_2(1-\boldsymbol\beta_1\cdot\boldsymbol\beta_2).
$$

In the [rest frame](../../mathematical-physics.md#rest-frame) of either particle this same [scalar](../../vector-space.md#scalar) is the relative [Lorentz factor](../../special-relativity.md#lorentz-factor) $\gamma_{\rm rel}$. Hence

$$
\beta_{\rm rel}^2
=1-\frac{(1-\beta_1^2)(1-\beta_2^2)}
{(1-\boldsymbol\beta_1\cdot\boldsymbol\beta_2)^2}.
$$

Let $d=\boldsymbol\beta_1\cdot\boldsymbol\beta_2$. The numerator after combining terms is

$$
(1-d)^2-(1-\beta_1^2)(1-\beta_2^2)
=\beta_1^2+\beta_2^2-2d-\beta_1^2\beta_2^2+d^2.
$$

Use $|\boldsymbol\beta_1\times\boldsymbol\beta_2|^2=\beta_1^2\beta_2^2-d^2$ to obtain

$$
\boxed{\beta_{\rm rel}^2=
\frac{|\boldsymbol\beta_1-\boldsymbol\beta_2|^2-
|\boldsymbol\beta_1\times\boldsymbol\beta_2|^2}
{(1-\boldsymbol\beta_1\cdot\boldsymbol\beta_2)^2}.}
$$

The two [rest frames](../../mathematical-physics.md#rest-frame) agree on the relative speed, although their [velocity vectors](../../tangent-vector.md#velocity-vector) are expressed in different spatial frames. Checks include equal velocities giving zero, collinear velocities giving $|\beta_1-\beta_2|/|1-\beta_1\beta_2|$, and low speeds reducing to the Galilean relative speed. For timelike particles the [four-velocity](../../special-relativity.md#four-velocity) [inner product](../../inner-product.md) also ensures $0\le\beta_{\rm rel}<1$.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**A [tidal force](../../newton-s-law-of-universal-gravitation.md#tidal-force) is a difference of [gravitational acceleration](../../newton-s-law-of-universal-gravitation.md#gravitational-acceleration) across an extended region.** In [Newtonian gravity](../../newton-s-law-of-universal-gravitation.md#gravitational-acceleration), $g_i=-\partial_i\Phi$. Two neighboring freely falling particles separated by $\xi^j$ have, to first order,

$$
\ddot\xi^i=\frac{\partial g_i}{\partial x^j}\xi^j
=-\frac{\partial^2\Phi}{\partial x^i\partial x^j}\xi^j.
$$

For a [point mass](../../classical-mechanics.md#point-mass), $\Phi=-GM/r$. In a local orthonormal radial/transverse frame,

$$
\boxed{\ddot\xi_r=\frac{2GM}{r^3}\xi_r,\qquad
\ddot\xi_{\perp1}=-\frac{GM}{r^3}\xi_{\perp1},\qquad
\ddot\xi_{\perp2}=-\frac{GM}{r^3}\xi_{\perp2}.}
$$

A small freely falling cloud stretches radially and compresses transversely. Outside the source the three eigenvalues sum to zero, consistently with $\nabla^2\Phi=0$; within matter the trace is $-4\pi G\rho$. These are accelerations of separations, not the much larger common acceleration of the cloud's centre.

<a id="2/a/image-original-local-tidal-map-a-freely-falling-cloud-stretches-along-the-radial-direction-and-contracts-in-both-transverse-directions"></a>
![](../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2015/paper-1-tidal-deviation.png)

**[Figure 1](#2/a/image-original-local-tidal-map-a-freely-falling-cloud-stretches-along-the-radial-direction-and-contracts-in-both-transverse-directions). Original local tidal map: a freely falling cloud stretches along the radial direction and contracts in both transverse directions**.

In [general relativity](../../general-relativity.md), freely falling test particles follow [timelike geodesics](../../general-relativity.md#timelike-geodesic). A freely falling frame can eliminate the connection at one event, but not the [Riemann curvature tensor](../../riemann-curvature-tensor.md) throughout a finite laboratory. Let $u$ be the [geodesic](../../riemannian-geometry.md#geodesic) tangent and $\xi$ a connecting [vector](../../vector-space.md#vector) for neighboring [geodesics](../../riemannian-geometry.md#geodesic) with $[u,\xi]=0$. In the explicitly chosen [curvature](../../differential-geometry.md#curvature) convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,
$$

the [geodesic deviation](../../riemann-curvature-tensor.md#geodesic-deviation) equation is

$$
\boxed{\frac{D^2\xi}{d\tau^2}=R(u,\xi)u.}
$$

It follows by commuting $\nabla_u\nabla_\xi u$, using $\nabla_u u=0$ and zero torsion. In a [parallel-propagated orthonormal frame](../../general-relativity.md#parallel-propagated-orthonormal-frame), its spatial components directly describe measured relative acceleration. The weak-field, slow-motion limit recovers the Newtonian Hessian above. Reversing the [curvature sign convention](../../riemann-curvature-tensor.md#curvature-sign-convention) reverses the displayed [curvature](../../differential-geometry.md#curvature) side, without changing the physical stretching. The [equivalence principle](../../general-relativity.md#equivalence-principle) removes locally uniform gravity, while [geodesic deviation](../../riemann-curvature-tensor.md#geodesic-deviation) measures the residual tidal field. The connection between [parallel transport](../../vector-bundle.md#parallel-transport), [curvature](../../differential-geometry.md#curvature) and neighboring [geodesics](../../riemannian-geometry.md#geodesic) is developed systematically in the standard geometric construction.[Section 3, Curvature: parallel transport and geodesic deviation; translate the chosen curvature sign consistently](../../physics-bibliography.md#lecture-notes-on-general-relativity-by-sean-m-carroll)

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [cosmological principle](../../cosmology.md#cosmological-principle) idealizes spatial slices as homogeneous and isotropic. The corresponding [Friedmann-Lemaître-Robertson-Walker metric](../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) can be written

$$
ds^2=c^2dt^2-a(t)^2\left[\frac{d\chi^2}{1-K\chi^2}
+\chi^2(d\theta^2+\sin^2\theta\,d\phi^2)\right],\qquad K=+1,0,-1.
$$

Here $t$ is [cosmic time](../../cosmology.md#cosmic-time), $a(t)$ has dimensions of length in this convention, and $\chi$ is a dimensionless [comoving coordinate](../../cosmology.md#comoving-coordinate). The sign of $K$ gives positive, zero or negative spatial [curvature](../../differential-geometry.md#curvature). It does not alone determine global topology. A comoving pair at fixed radial coordinates has proper separation scaling with $a(t)$, so the [Hubble parameter](../../cosmology.md#hubble-parameter) is $H=\dot a/a$, and [cosmological redshift](../../cosmology.md#cosmological-redshift) satisfies $1+z=a(t_{\rm obs})/a(t_{\rm em})$.

For a [perfect fluid](../../general-relativity.md#perfect-fluid) of mass-equivalent [energy density](../../statistical-physics.md#energy-density) $\rho$ and [pressure](../../pressure.md) $p$, Einstein's equations give

$$
\boxed{H^2=\frac{8\pi G\rho}{3}-\frac{Kc^2}{a^2}+\frac{\Lambda c^2}{3},}
$$



$$
\boxed{\frac{\ddot a}{a}=-\frac{4\pi G}{3}\left(\rho+\frac{3p}{c^2}\right)
+\frac{\Lambda c^2}{3},\qquad
\dot\rho+3H\left(\rho+\frac p{c^2}\right)=0.}
$$

The last equation is local [energy](../../energy.md) conservation for constant $\Lambda$, with [vacuum energy](../../perturbative-quantum-field-theory.md#vacuum-energy) kept separate from $\rho,p$. A component with $p=w\rho c^2$ has $\rho\propto a^{-3(1+w)}$: [pressureless matter](../../cosmology.md#pressureless-matter) dilutes as $a^{-3}$ and [radiation](../../physics.md#radiation) as $a^{-4}$, the additional [radiation](../../physics.md#radiation) factor being [photon](../../quantum-mechanics.md#photon) [redshift](../../optics.md#redshift). With $K=\Lambda=0$, matter domination gives $a\propto t^{2/3}$ and [radiation](../../physics.md#radiation) domination gives $a\propto t^{1/2}$. Positive [vacuum energy](../../perturbative-quantum-field-theory.md#vacuum-energy) alone gives exponential expansion, $a\propto e^{Ht}$ with $H=c\sqrt{\Lambda/3}$.

<a id="2/b/image-original-comparison-of-normalized-scale-factors-in-flat-radiation-matter-and-positive-vacuum-models-the-vacuum-model-has-no-finite-time-big-bang-origin-in-this-chart"></a>
![](../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2015/paper-1-flrw-expansion.png)

**[Figure 2](#2/b/image-original-comparison-of-normalized-scale-factors-in-flat-radiation-matter-and-positive-vacuum-models-the-vacuum-model-has-no-finite-time-big-bang-origin-in-this-chart). Original comparison of normalized scale factors in flat radiation, matter and positive-vacuum models; the vacuum model has no finite-time big-bang origin in this chart**.

**Geometry, contents and initial conditions together determine the expansion history.** A closed matter-only model recollapses; an open matter-only model expands indefinitely. With a [cosmological constant](../../cosmology.md#cosmological-constant), positive spatial [curvature](../../differential-geometry.md#curvature) no longer by itself implies recollapse. Present [critical density](../../cosmology.md#critical-density) is $\rho_c=3H_0^2/(8\pi G)$ and the density parameters obey $\Omega_m+\Omega_r+\Omega_\Lambda+\Omega_K=1$, where $\Omega_K=-Kc^2/(a_0^2H_0^2)$. These models describe the large-scale background, while local structure and inhomogeneities require perturbations or more general metrics.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Ordinary component differences at neighboring points depend on how the local bases vary. The [covariant derivative](../../general-relativity.md#covariant-derivative) corrects for that variation:

$$
\boxed{\nabla_b V^a=\partial_bV^a+\Gamma^a_{bc}V^c,
\qquad \nabla_bW_a=\partial_bW_a-\Gamma^c_{ba}W_c.}
$$

Each upper [tensor](../../multilinear-algebra.md#tensor) index adds a connection term and each lower index subtracts one. A [scalar](../../vector-space.md#scalar) has $\nabla_a f=\partial_a f$, while the derivative of a [tensor](../../multilinear-algebra.md#tensor) transforms as a [tensor](../../multilinear-algebra.md#tensor) with one additional covariant index. The [Christoffel symbols](../../riemannian-geometry.md#christoffel-symbol) themselves are not [tensor](../../multilinear-algebra.md#tensor) components; their inhomogeneous transformation cancels that of the ordinary derivative.

For the [Levi-Civita connection](../../general-relativity.md#levi-civita-connection),

$$
\Gamma^a_{bc}=\frac12g^{ad}
(\partial_b g_{dc}+\partial_c g_{bd}-\partial_d g_{bc}),
\qquad \nabla_cg_{ab}=0,\qquad\Gamma^a_{bc}=\Gamma^a_{cb}.
$$

These express [metric compatibility](../../vector-bundle.md#metric-compatibility) and zero torsion. Along $x^a(\lambda)$, [parallel transport](../../vector-bundle.md#parallel-transport) is the [initial value problem](../../differential-equation.md#initial-value-problem)

$$
\boxed{\frac{DV^a}{d\lambda}
=\frac{dV^a}{d\lambda}
+\Gamma^a_{bc}\frac{dx^b}{d\lambda}V^c=0.}
$$

It preserves [inner products](../../inner-product.md) for the [Levi-Civita connection](../../general-relativity.md#levi-civita-connection). [Parallel transport](../../vector-bundle.md#parallel-transport) of the tangent itself gives the affinely parametrized [geodesic equation](../../riemannian-geometry.md#geodesic-equation), $\ddot x^a+\Gamma^a_{bc}\dot x^b\dot x^c=0$.

Transport generally depends on the path. On a round [sphere](../../euclidean-geometry.md#sphere), transport a [tangent vector](../../tangent-vector.md) around the triangle bounded by two meridians $90$ degrees apart and the intervening equatorial arc. All three sides are [geodesics](../../riemannian-geometry.md#geodesic); the enclosed spherical area is $\pi a^2/2$. The returning [vector](../../vector-space.md#vector) is rotated by $90$ degrees, with sign set by traversal orientation. Locally this [holonomy](../../fiber-bundle.md#holonomy) is controlled by [curvature](../../differential-geometry.md#curvature), even though the connection can be made zero at a single point. A [vector](../../vector-space.md#vector) can therefore have changing coordinate components while remaining parallel, and constant components do not generally mean [parallel transport](../../vector-bundle.md#parallel-transport).

<a id="2/c/image-original-spherical-triangle-transport-a-tangent-initially-pointing-along-the-first-meridian-returns-rotated-by-ninety-degrees"></a>
![](../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2015/paper-1-spherical-transport.png)

**[Figure 3](#2/c/image-original-spherical-triangle-transport-a-tangent-initially-pointing-along-the-first-meridian-returns-rotated-by-ninety-degrees). Original spherical-triangle transport: a tangent initially pointing along the first meridian returns rotated by ninety degrees**.

This construction compares directions at separate points through a chosen connection, rather than assuming that a curved manifold supplies a path-independent comparison.[Section 3, Curvature: the covariant derivative, Levi-Civita connection and parallel transport](../../physics-bibliography.md#lecture-notes-on-general-relativity-by-sean-m-carroll)

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use Cartesian coordinates $x^a=(t,x,y,z)$ with $c=1$ and $\eta_{ab}=\operatorname{diag}(1,-1,-1,-1)$. Spatial dot and [cross products](../../vector-space.md#cross-product) below use the Euclidean three-metric. The alternating [tensor](../../multilinear-algebra.md#tensor) is given the orientation $\epsilon^{0123}=+1$.

**[Vector](../../vector-space.md#vector) and [covector](../../dual-space.md#covector) transformation.** The [vector](../../vector-space.md#vector) $A=A^b\partial_b$ is independent of coordinates, and the [chain rule](../../calculus.md#chain-rule) gives $\partial_b=(\partial x'^a/\partial x^b)\partial'_a$. Likewise the [one-form](../../differential-form.md#one-form) $A_bdx^b$ is independent of coordinates. Comparing coefficients proves

$$
\boxed{A'^a=\frac{\partial x'^a}{\partial x^b}A^b,
\qquad A'_a=\frac{\partial x^b}{\partial x'^a}A_b.}
$$

Their contraction $A_a B^a$ is unchanged because the forward and inverse Jacobians cancel. Here lowering an index uses the metric, not an identification of the numerical upper and lower components.

**Why antisymmetrization matters.** Write $J^c{}_a=\partial x^c/\partial x'^a$. Differentiating the [covector](../../dual-space.md#covector) law gives

$$
\partial'_a A'_b
=J^c{}_aJ^d{}_b\,\partial_c A_d
+\frac{\partial^2x^d}{\partial x'^a\partial x'^b}A_d.
$$

The last term obstructs the general [tensor](../../multilinear-algebra.md#tensor) transformation law. It is symmetric in $a,b$, so it cancels from $\partial'_aA'_b-\partial'_bA'_a$. Therefore

$$
\boxed{F'_{ab}=J^c{}_aJ^d{}_bF_{cd}.}
$$

Equivalently $F=dA$ is the [exterior derivative](../../differential-form.md#exterior-derivative) of the [electromagnetic four-potential](../../relativistic-electromagnetism.md#electromagnetic-four-potential) [one-form](../../differential-form.md#one-form). The statement that $\partial_aA_b$ is not a [tensor](../../multilinear-algebra.md#tensor) needs a qualification: **under affine Cartesian [Lorentz transformations](../../special-relativity.md#lorentz-transformation) it does transform tensorially**, because the second derivatives vanish. The failure concerns arbitrary nonlinear coordinate changes, including curvilinear coordinates in flat spacetime. This distinction is precisely the difference between general covariance and covariance under the restricted inertial-frame transformations.[Section 2, Manifolds, equations 2.26–2.27: the extra second-derivative term and its cancellation under antisymmetrization](../../physics-bibliography.md#lecture-notes-on-general-relativity-by-sean-m-carroll)

**Electric and magnetic components.** Choose $A^a=(\Phi,\mathbf A)$, so $A_a=(\Phi,-\mathbf A)$, $\mathbf E=-\boldsymbol\nabla\Phi-\partial_t\mathbf A$ and $\mathbf B=\boldsymbol\nabla\times\mathbf A$. Then

$$
F_{0i}=\partial_t(-A_i^{\rm spatial})-\partial_i\Phi=E_i,
\qquad F_{ij}=-\epsilon_{ijk}B_k.
$$

Thus the lower-index field [tensor](../../multilinear-algebra.md#tensor) is

$$
F_{ab}=\begin{pmatrix}
0&E_x&E_y&E_z\\
-E_x&0&-B_z&B_y\\
-E_y&B_z&0&-B_x\\
-E_z&-B_y&B_x&0
\end{pmatrix}.
$$

This is a derived component representation of the field, with the source's sign convention.

**Raised indices and the first invariant.** Raising both indices changes the time-space signs and leaves the spatial block unchanged:

$$
\boxed{F^{ab}=\begin{pmatrix}
0&-E_x&-E_y&-E_z\\
E_x&0&-B_z&B_y\\
E_y&B_z&0&-B_x\\
E_z&-B_y&B_x&0
\end{pmatrix}.}
$$

In the [scalar](../../vector-space.md#scalar) contraction, each independent antisymmetric pair is counted twice, giving

$$
\boxed{F_{ab}F^{ab}=2(B^2-E^2).}
$$

Under a [Lorentz transformation](../../special-relativity.md#lorentz-transformation) each inverse transformation from a lower index cancels its matching transformation from an upper index, leaving the same [scalar](../../vector-space.md#scalar). In particular a [plane electromagnetic wave](../../electromagnetic-wave.md#plane-electromagnetic-wave) has $E=B$ in these units and makes this invariant vanish, while a pure [electric field](../../electric-field.md) makes it negative.

**The printed dual convention.** The PDF explicitly defines ${}^*F^{ab}=\epsilon^{abcd}F_{cd}$, with no $1/2$. Each independent pair therefore contributes twice: for example ${}^*F^{01}=F_{23}-F_{32}=-2B_x$. The complete result is

$$
\boxed{{}^*F^{ab}=2\begin{pmatrix}
0&-B_x&-B_y&-B_z\\
B_x&0&E_z&-E_y\\
B_y&-E_z&0&E_x\\
B_z&E_y&-E_x&0
\end{pmatrix},\qquad {}^*F^{ab}F_{ab}=-8\mathbf E\cdot\mathbf B.}
$$

The time-space pairs contribute $-4\mathbf E\cdot\mathbf B$ and the spatial pairs contribute another $-4\mathbf E\cdot\mathbf B$. The conventional Hodge dual includes $1/2$ and would instead give the contraction $-4\mathbf E\cdot\mathbf B$; it must not silently replace this paper's definition. With fixed orientation the latter contraction is a [pseudoscalar](../../quantum-mechanics.md#pseudoscalar): invariant under proper [Lorentz transformations](../../special-relativity.md#lorentz-transformation) but odd under orientation reversal if compared using a fixed alternating symbol.

**[Energy density](../../statistical-physics.md#energy-density) and flux.** Substitution into the given mixed stress-energy [tensor](../../multilinear-algebra.md#tensor) yields

$$
\boxed{T^0{}_0=\frac{E^2+B^2}{2\mu_0},\qquad
T^0{}_i=-\frac{(\mathbf E\times\mathbf B)_i}{\mu_0}.}
$$

For the first formula, $F^{0c}F_{0c}=-E^2$ and $F_{cd}F^{cd}/4=(B^2-E^2)/2$. For the second, $F^{0j}F_{ij}=(\mathbf E\times\mathbf B)_i$. The minus sign on $T^0{}_i$ arises from its lowered spatial index; it does not reverse the physical [energy](../../energy.md) flow. Raising that index gives $T^{0i}=S_i$, and symmetry gives $T^{i0}=S_i$, with $\mathbf S=\mathbf E\times\mathbf B/\mu_0$ the [Poynting vector](../../electromagnetic-wave.md#poynting-vector) in $c=1$ units. Thus $T^{00}$ is [energy density](../../statistical-physics.md#energy-density) and $T^{i0}$ represents [energy](../../energy.md) flux. In SI coordinates $x^0=ct$, restore $T^{0i}=S_i/c$ and $T^{00}=(\epsilon_0 E_{\rm SI}^2+B^2/\mu_0)/2$, with $\epsilon_0\mu_0c^2=1$. This keeps the mixed-index signs and the units distinct.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Put $f(r)=1-2\mu/r$, where $\mu=GM/c^2$, and work in the orbital plane. A dot denotes an affine-parameter derivative; for a material particle choose that parameter to be [proper time](../../special-relativity.md#proper-time).

**First integrals and normalization.** The [geodesic Lagrangian](../../riemannian-geometry.md#geodesic-lagrangian) is

$$
L=\frac12\left(fc^2\dot t^2-f^{-1}\dot r^2-r^2\dot\phi^2\right).
$$

Time translation and axial rotation make $t$ and $\phi$ cyclic, giving

$$
\boxed{f\dot t=k,\qquad r^2\dot\phi=h.}
$$

The tangent norm is constant along an affine [geodesic](../../riemannian-geometry.md#geodesic) because the [Levi-Civita connection](../../general-relativity.md#levi-civita-connection) preserves the metric. Therefore

$$
fc^2\dot t^2-f^{-1}\dot r^2-r^2\dot\phi^2=\mathcal E.
$$

For proper-time parametrization of a timelike [worldline](../../special-relativity.md#world-line) this norm is $c^2$. For a [null geodesic](../../special-relativity.md#null-geodesic) it is zero, for every affine normalization. Thus **$\mathcal E=c^2$ for the chosen material-particle normalization and $\mathcal E=0$ for light**. [Proper time](../../special-relativity.md#proper-time) cannot itself parametrize a null ray, despite the same printed symbol $\tau$ being used for its [affine parameter](../../riemannian-geometry.md#affine-parameter).

**Null normalization and [impact parameter](../../classical-mechanics.md#impact-parameter).** Under $\tau\mapsto A\tau+B$ with $A>0$, both $k$ and $h$ scale as $1/A$, while the null path is unchanged. Their ratio is invariant. At large radius the spatial speed with respect to asymptotic time is $c$, and orbital [angular momentum](../../momentum.md#angular-momentum) per affine tangent gives

$$
\boxed{b=\frac{|h|}{kc};\qquad k=1\ \Longrightarrow\ |h|=bc.}
$$

For an orientation chosen with $h>0$, this is $h=bc$. Setting $k=1$ is a choice of affine scale, not a claim that all [photons](../../quantum-mechanics.md#photon) have equal measured [energy](../../energy.md). Once a tangent is identified with a physically normalized [four-momentum](../../special-relativity.md#four-momentum), its [energy](../../energy.md) fixes that scale.

**Orbit shape.** Substituting the constants in the norm and multiplying by $f$ gives

$$
\dot r^2=k^2c^2-f\left(\mathcal E+\frac{h^2}{r^2}\right).
$$

For $u=1/r$ and $h\ne0$, $du/d\phi=-\dot r/h$. Hence

$$
\boxed{(u')^2+u^2=\frac{k^2c^2}{h^2}+2\mu u^3
-\frac{\mathcal E}{h^2}(1-2\mu u),\qquad u'=\frac{du}{d\phi}.}
$$

The $h=0$ radial orbit must be treated with the radial equation, because azimuth is then constant.

**Circular [photons](../../quantum-mechanics.md#photon) and stability.** For a null ray define $W(r)=f(r)/r^2$. Its radial equation becomes

$$
\dot r^2+h^2W(r)=k^2c^2,\qquad
W'(r)=-\frac2{r^3}+\frac{6\mu}{r^4}.
$$

The circular orbit requires $\dot r=0$ and $W'=0$, so

$$
\boxed{r_{\rm ph}=3\mu,\qquad W''(3\mu)=-\frac2{81\mu^4}<0.}
$$

It is at a maximum of the null [effective potential](../../mathematical-physics.md#effective-potential) and is unstable. Equivalently the [Binet equation](../../celestial-mechanics.md#binet-equation) $u''+u=3\mu u^2$ linearizes about $u_0=1/(3\mu)$ to $\delta u''=\delta u$, admitting exponentially growing radial deviations in azimuth.

**Capture from infinity.** Divide the null radial equation by $k^2c^2$. The quantity opposing inward motion is $b^2W(r)$, whose exterior maximum is $b^2/(27\mu^2)$. There is no outer radial [turning point](../../energy.md#turning-point) precisely when

$$
\boxed{b<3\sqrt3\,\mu.}
$$

At equality an exactly critical ray from infinity asymptotes to the [photon sphere](../../schwarzschild-spacetime.md#photon-sphere); it does not cross the horizon at a finite [affine parameter](../../riemannian-geometry.md#affine-parameter). Above the threshold an initially inward ray from infinity reaches an outer [turning point](../../energy.md#turning-point) and scatters. The radial case $b=0$ is also captured. These statements refer to inward rays launched from the asymptotically flat exterior, not arbitrary initial data inside the angular-momentum barrier.

<a id="4/image-original-schwarzschild-capture-calculation-the-null-potential-barrier-and-a-captured-equatorial-ray-crossing-the-horizon-and-ending-at-finite-azimuth"></a>
![](../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2015/paper-1-photon-capture.png)

**[Figure 4](#4/image-original-schwarzschild-capture-calculation-the-null-potential-barrier-and-a-captured-equatorial-ray-crossing-the-horizon-and-ending-at-finite-azimuth). Original Schwarzschild capture calculation: the null-potential barrier and a captured equatorial ray crossing the horizon and ending at finite azimuth**.

**Approach to the singularity.** A captured nonradial ray bends inward, crosses $r=3\mu$ and then the [event horizon](../../black-hole.md#event-horizon) $r=2\mu$, and continues toward the [curvature singularity](../../general-relativity.md#curvature-singularity). A plot in $(r\cos\phi,r\sin\phi)$ is only a coordinate projection, not a Euclidean spatial slice inside the horizon. For large $u$ the cubic term in the shape equation dominates:

$$
\frac{du}{d\phi}\simeq\sqrt{2\mu}\,u^{3/2}
$$

for the inward branch with $h>0$. Its integral is

$$
\phi_*-\phi\simeq\sqrt{\frac2\mu}\,u^{-1/2},\qquad
\boxed{r\simeq\frac\mu2(\phi_*-\phi)^2.}
$$

Thus the azimuth tends to a finite limit at the singularity, rather than winding infinitely often there. Near-critical rays can accumulate many turns near $3\mu$ before capture, which is a separate phenomenon. A strictly radial ray has constant azimuth and does not admit this azimuthal asymptotic form. The radial equation also gives $r\propto(\tau_*-\tau)^{2/5}$ for a nonradial null ray, confirming finite remaining [affine parameter](../../riemannian-geometry.md#affine-parameter).

**Material capture and the condition at infinity.** To recover the quoted threshold, take the usual marginally bound orbit, initially at rest at infinity: $k=1$. With $\mathcal E=c^2$,

$$
\dot r^2=\frac{2\mu c^2}{r}-\frac{h^2}{r^2}+\frac{2\mu h^2}{r^3}
=\frac{2\mu c^2r^2-h^2r+2\mu h^2}{r^3}.
$$

The turning-point quadratic has [discriminant](../../polynomial.md#discriminant) $h^2(h^2-16\mu^2c^2)$. It is positive for large $r$ and has no real positive root when $0<|h|<4\mu c$, while the radial case also falls in. Therefore

$$
\boxed{|h|<4\mu c\quad\Longrightarrow\quad\text{capture from rest at infinity}.}
$$

At equality the quadratic is proportional to $(r-4\mu)^2$ and the orbit asymptotes to the unstable marginally bound circular orbit at $r=4\mu$. For larger $|h|$, an incoming marginally bound particle encounters the outer [turning point](../../energy.md#turning-point) and scatters.

The source says only “from infinity”, without explicitly fixing the asymptotic speed. For a general incoming speed $v_\infty$, $k=(1-v_\infty^2/c^2)^{-1/2}\ge1$ and

$$
\dot r^2=c^2(k^2-1)+\frac{2\mu c^2}{r}
-\frac{h^2}{r^2}+\frac{2\mu h^2}{r^3}.
$$

The same bound $|h|<4\mu c$ remains sufficient for capture, since the added constant is nonnegative. It is **the exact threshold only for $k=1$**. At fixed $k>1$, the critical unstable orbit satisfies

$$
k^2=\frac{(r_c-2\mu)^2}{r_c(r_c-3\mu)},\qquad
h_c^2=\frac{\mu c^2r_c^2}{r_c-3\mu},\qquad3\mu<r_c<4\mu.
$$

Then $h_c>4\mu c$. This states both the printed sufficient condition and the additional assumption needed to call it a sharp capture boundary.

## ↑ Ancestors (11)

1. [2015](../2015.md)
2. [Past exam of the relativity course of the University of Cambridge](../../past-exam-of-the-relativity-course-of-the-university-of-cambridge.md)
3. [Relativity course of the University of Cambridge](../../university-of-cambridge.md#relativity-course-of-the-university-of-cambridge)
4. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
