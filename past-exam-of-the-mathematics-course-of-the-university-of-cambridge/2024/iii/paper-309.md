# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_309.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [proper time](../../../special-relativity.md#proper-time) elapsed along the smooth [timelike curve](../../../special-relativity.md#timelike-curve) is

$$
\boxed{T[\gamma]=\int_0^1
\sqrt{-g_{\mu\nu}(x(s))\frac{dx^\mu}{ds}\frac{dx^\nu}{ds}}\,ds}.
$$

The expression is invariant under every orientation-preserving [reparametrization](../../../differential-geometry.md#reparametrization) of the curve.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Write $\dot x^\mu=dx^\mu/ds$ and $L=\sqrt{-g_{\mu\nu}\dot x^\mu\dot x^\nu}$. Varying $T=\int L\,ds$ with fixed endpoints and then choosing [proper time](../../../special-relativity.md#proper-time) as parameter, for which $L=1$, gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\frac d{d\tau}(g_{\mu\nu}\dot x^\nu)
-\frac12\partial_\mu g_{\alpha\beta}\dot x^\alpha\dot x^\beta=0.
$$

Expanding the derivative, raising the free index with the [inverse metric](../../../general-relativity.md#inverse-metric), and using the symmetry of $\dot x^\alpha\dot x^\beta$ gives the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation)

$$
\boxed{\ddot x^\rho+\Gamma^\rho{}_{\alpha\beta}
\dot x^\alpha\dot x^\beta=0},
\qquad
\boxed{\Gamma^\rho{}_{\alpha\beta}
=\frac12g^{\rho\mu}
(\partial_\alpha g_{\mu\beta}+\partial_\beta g_{\mu\alpha}
-\partial_\mu g_{\alpha\beta})}.
$$

These are the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

For the quadratic [geodesic Lagrangian](../../../riemannian-geometry.md#geodesic-lagrangian)

$$
L_E=\frac12g_{\mu\nu}(x)\dot x^\mu\dot x^\nu,
$$

the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
g_{\mu\nu}\ddot x^\nu
+\partial_\rho g_{\mu\nu}\dot x^\rho\dot x^\nu
-\frac12\partial_\mu g_{\alpha\beta}\dot x^\alpha\dot x^\beta=0.
$$

Raising $\mu$ and symmetrizing the coefficient of the two velocities produces exactly

$$
\ddot x^\rho+\Gamma^\rho{}_{\alpha\beta}
\dot x^\alpha\dot x^\beta=0.
$$

The quadratic [action](../../../classical-mechanics.md#action) fixes an [affine parameter](../../../riemannian-geometry.md#affine-parameter); proper time is an affine parameter for a timelike geodesic.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Put $u=t-z$. Wherever $|u|>U$, the profile $A(u)$ vanishes and the displayed metric is exactly the [Minkowski metric](../../../special-relativity.md#minkowski-metric). Thus the two flat regions in the $(t,z)$-plane are the half-planes $t-z>U$ and $t-z<-U$, separated by the strip

$$
\boxed{|t-z|\leq U}.
$$

At fixed $t$ this strip is $t-U\leq z\leq t+U$, so it has longitudinal width $2U$. A surface $u=\text{constant}$ obeys $z=t-u$ and travels in the positive $z$ direction at the [speed of light](../../../special-relativity.md#speed-of-light). The curvature is confined to that moving strip, identifying the solution as a [gravitational-wave pulse](../../../general-relativity.md#gravitational-wave-pulse) represented by a [plane-fronted gravitational wave](../../../general-relativity.md#plane-fronted-gravitational-wave).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

With $u=t-z$, the quadratic [geodesic Lagrangian](../../../riemannian-geometry.md#geodesic-lagrangian) is

$$
L=\frac12(-\dot t^2+\dot x^2+\dot y^2+\dot z^2)
+xyA(u)\dot u^2.
$$

Its transverse [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) are

$$
\boxed{\ddot x=yA(u)\dot u^2,
\qquad \ddot y=xA(u)\dot u^2}.
$$

The longitudinal equations are

$$
\boxed{\ddot t=\ddot z
=2A(u)(\dot x,y+x\dot y)\dot u+xyA'(u)\dot u^2},
$$

after using the difference of those same equations. In particular,

$$
\ddot u=\ddot t-\ddot z=0,
\qquad
\boxed{\dot t-\dot z=\dot u=\text{constant}}.
$$

This conserved quantity also follows from the [Killing vector field](../../../general-relativity.md#killing-vector-field) $\partial_t+\partial_z$ and the [geodesic conserved quantity from a Killing vector](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector).

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The initial data and $\ddot u=0$ give $u=\tau$. To first order in $\epsilon$, replace $x$ and $y$ on the right-hand sides of the transverse equations by $x_0$ and $y_0$. Twice integrating with the initial rest conditions gives

$$
\boxed{x(\tau)=x_0+\epsilon y_0
\int_{-\infty}^{\tau}(\tau-s)a(s)\,ds+O(\epsilon^2)},
$$



$$
\boxed{y(\tau)=y_0+\epsilon x_0
\int_{-\infty}^{\tau}(\tau-s)a(s)\,ds+O(\epsilon^2)}.
$$

For $\tau>U$, define $A_0=\int_{-\infty}^{\infty}a(s)\,ds$ and $A_1=\int_{-\infty}^{\infty}s,a(s)\,ds$. Then

$$
x=x_0-\epsilon y_0A_1+\tau\epsilon y_0A_0,
\qquad
y=y_0-\epsilon x_0A_1+\tau\epsilon x_0A_0.
$$

Hence

$$
\boxed{\delta x=-\epsilon y_0A_1,
\quad\delta v_x=\epsilon y_0A_0,
\quad\delta y=-\epsilon x_0A_1,
\quad\delta v_y=\epsilon x_0A_0}.
$$

These permanent changes are forms of [displacement memory](../../../general-relativity.md#displacement-memory) and [velocity memory](../../../general-relativity.md#velocity-memory).

There is a discrepancy in the question's final instruction. The longitudinal equation actually gives

$$
\ddot z=\epsilon x_0y_0a'(\tau)+O(\epsilon^2),
$$

and therefore

$$
\boxed{\dot z=\epsilon x_0y_0a(\tau)+O(\epsilon^2),
\qquad
z=\epsilon x_0y_0\int_{-\infty}^{\tau}a(s)\,ds+O(\epsilon^2)}.
$$

Thus $z$ does not vanish to first order for a general allowed profile. It vanishes after the pulse under the additional hypothesis $A_0=0$ used in part (iv), but it need not vanish while that pulse is passing. The [proper-time normalization](../../../special-relativity.md#proper-time-normalization) independently gives the same relation $\dot z=xyA+O(\epsilon^2)$.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

Now $A_0=0$, so every mass is again at rest after the pulse and $z=0+O(\epsilon^2)$. Put $k=\epsilon A_1>0$. The final transverse coordinates are

$$
\begin{pmatrix}x\\y\end{pmatrix}_{\!\rm after}
=\begin{pmatrix}1&-k\\-k&1\end{pmatrix}
\begin{pmatrix}x_0\\y_0\end{pmatrix}.
$$

The unit vectors along $x=y$ and $x=-y$ are [eigenvectors](../../../linear-operator-theory.md#eigenvector) with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $1-k$ and $1+k$, respectively. Consequently an initial [circle](../../../topology.md#circle) becomes, to first order, an [ellipse](../../../geometry-and-topology.md#ellipse) compressed along the line $x=y$ and stretched along $x=-y$. This persistent deformation is [displacement memory](../../../general-relativity.md#displacement-memory).

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For any [vector field](../../../calculus.md#vector-field) $Y$, apply the [Leibniz rule](../../../calculus.md#leibniz-rule) to the scalar $\omega(Y)$:

$$
\mathcal L_V(\omega_aY^a)
=(\mathcal L_V\omega)_aY^a+\omega_a(\mathcal L_VY)^a.
$$

Using $\mathcal L_VY=[V,Y]$ and expanding the [Lie bracket](../../../lie-algebra.md#lie-bracket) in a coordinate chart leaves

$$
\boxed{(\mathcal L_V\omega)_a
=V^b\nabla_b\omega_a+\omega_b\nabla_aV^b}.
$$

The connection terms cancel because the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is torsion-free. Applying this formula to each slot of the [metric tensor](../../../general-relativity.md#metric-tensor) and using [metric compatibility](../../../fiber-bundle.md#metric-compatibility) gives

$$
\boxed{(\mathcal L_Vg)_{ab}=\nabla_aV_b+\nabla_bV_a}.
$$

Equivalently, one may prove both identities at a point in [normal coordinates](../../../general-relativity.md#normal-coordinates); since both sides are tensors, the result then holds in every coordinate system.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The trace of the [electromagnetic stress-energy tensor](../../../electromagnetism.md#electromagnetic-stress-energy-tensor) in four [spacetime dimensions](../../../general-relativity.md#spacetime-dimension) is

$$
T^a{}_a=F^{ac}F_{ac}-\frac14\delta^a_aF_{cd}F^{cd}=0.
$$

For its [covariant divergence](../../../general-relativity.md#covariant-divergence), the source-free [Maxwell equations](../../../electromagnetism.md#maxwell-equations) eliminate the derivative of the first factor. Contracting the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) $\nabla_{[a}F_{bc]}=0$ with $F^{ac}$ gives

$$
F^{ac}\nabla_aF_{bc}=\frac14\nabla_b(F_{cd}F^{cd}),
$$

which cancels the derivative of the trace term. Hence

$$
\boxed{\nabla_aT^a{}_b=0,
\qquad T^a{}_a=0}.
$$

For $J^a=T^{ab}V_b$, [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation) and symmetry of $T^{ab}$ now imply

$$
\nabla_aJ^a=T^{ab}\nabla_aV_b
=\frac12T^{ab}(\nabla_aV_b+\nabla_bV_a)
=\boxed{\frac12T^{ab}(\mathcal L_Vg)_{ab}}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

At the chosen event use the [orthonormal frame in spacetime](../../../general-relativity.md#orthonormal-frame-in-spacetime) from the hint. The electromagnetic energy density is

$$
\rho=T_{00}=\frac12(|\mathbf E|^2+|\mathbf B|^2),
$$

and the energy flux is the [Poynting vector](../../../electromagnetism.md#poynting-vector) $\mathbf S=\mathbf E\times\mathbf B$. Depending on the index convention, the required contraction is $\rho-wS_1$ or $\rho+wS_1$. In either case,

$$
T_{ab}V^aW^b\geq\rho-|\mathbf S|
\geq\frac12(|\mathbf E|^2+|\mathbf B|^2)-|\mathbf E||\mathbf B|
=\frac12(|\mathbf E|-|\mathbf B|)^2\geq0.
$$

Rescaling $V$ and rotating the spatial frame covers arbitrary future timelike $V$ and future causal $W$. Thus the Maxwell field satisfies the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Since $t=u+r$, the hypersurface $\Sigma_t$ is an ordinary constant-Minkowski-time slice. Its future unit normal is

$$
\boxed{n^a=(1,0,0,0)=\partial_u}
$$

in the $(u,r,\theta,\phi)$ basis. Lowering the index gives $n_a=(-1,-1,0,0)=-\nabla_at$. Restricting the metric to $dt=du+dr=0$ gives the Euclidean spherical metric

$$
dr^2+r^2(d\theta^2+\sin^2\theta\,d\phi^2),
$$

so its induced [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) is

$$
\boxed{d\sigma=r^2\sin\theta\,dr\,d\theta\,d\phi}.
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

For $V=r\partial_r$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
\mathcal L_Vdr=d(i_Vdr)+i_Vd(dr)=d(r)=dr,
$$

whereas contraction and exterior differentiation both vanish for $du,d\theta,d\phi$. Thus

$$
\mathcal L_Vdu=\mathcal L_Vd\theta=\mathcal L_Vd\phi=0.
$$

Applying the [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) to  
$g=-du^2-2,du,dr+r^2d\Omega^2$ yields

$$
\mathcal L_Vg=-2,du,dr+2r^2d\Omega^2.
$$

Here $n_a=-(du+dr)_a$ and $V_a=-r(du)_a$, so comparison with $2g$ gives

$$
\boxed{(\mathcal L_Vg)_{ab}
=2g_{ab}+\frac2r n_{(a}V_{b)}},
\qquad \boxed{\alpha=2}.
$$

Using tracelessness from part (b)(i),

$$
\nabla_a(T^{ab}V_b)
=\frac1rT^{ab}n_aV_b\geq0
$$

by the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition), because $n$ is future timelike and $V$ is future null.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

The integrand defining $\varepsilon(t)$ is nonnegative by the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition), hence

$$
\boxed{\varepsilon(t)\geq0}.
$$

Apply the spacetime [divergence theorem](../../../calculus.md#divergence-theorem) to $J^a=T^{ab}V_b$ on the slab $S$. The flux through the cylinder at $r\to\infty$ vanishes by the stated decay. With the Lorentzian boundary orientation, the two spacelike boundary contributions give

$$
\varepsilon(t_0)-\varepsilon(t_1)
=\int_S\nabla_aJ^a\,d\operatorname{vol}_g.
$$

Part (ii) makes the right-hand side nonnegative, so for $t_1\geq t_0$,

$$
\boxed{\varepsilon(t_1)\leq\varepsilon(t_0)}.
$$

**Therefore $\varepsilon$ is a nonnegative monotone decreasing energy functional.**

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Put $h_{ab}=\delta g_{ab}$. Varying $g^{ac}g_{cb}=\delta^a_b$ gives

$$
\boxed{\delta g^{ab}=-g^{ac}g^{bd}h_{cd}=-h^{ab}}.
$$

The determinant identity $\delta\log|\det g|=g^{ab}h_{ab}$ gives

$$
\boxed{\delta(d\operatorname{vol}_g)
=\frac12g^{ab}h_{ab}\,d\operatorname{vol}_g}.
$$

Finally, varying the formula for the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) and rewriting partial derivatives covariantly gives the tensor

$$
\boxed{\delta\Gamma^a{}_{bc}
=\frac12g^{ad}(\nabla_bh_{cd}+\nabla_ch_{bd}-\nabla_dh_{bc})}.
$$

These are the basic [metric variation](../../../general-relativity.md#metric-variation) identities.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Varying the [Ricci tensor](../../../general-relativity.md#ricci-tensor) and contracting gives

$$
\delta R=-R^{ab}h_{ab}
+\nabla_a\!\left(g^{cb}\delta\Gamma^a{}_{cb}
-g^{ab}\delta\Gamma^c{}_{cb}\right).
$$

Substitution of part (i), followed by [metric compatibility](../../../fiber-bundle.md#metric-compatibility), reduces the divergence to

$$
\nabla_a\nabla_bh^{ab}-\nabla^a\nabla_ah.
$$

Thus the [metric variation of scalar curvature](../../../general-relativity.md#metric-variation-of-scalar-curvature) is

$$
\boxed{\delta R=-R^{ab}\delta g_{ab}
-g^{ab}\nabla_c\nabla^c\delta g_{ab}
+\nabla^a\nabla^b\delta g_{ab}},
$$

and consequently

$$
\boxed{\alpha=-1,
\qquad \beta=1}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Vary the gravitational volume factor and use part (a)(ii):

$$
\delta(f(R)d\operatorname{vol}_g)
=\left[f'(R)\delta R+\frac12f(R)g^{ab}h_{ab}\right]d\operatorname{vol}_g.
$$

Twice applying [integration by parts](../../../calculus.md#integration-by-parts) moves both derivatives in $\delta R$ from the compactly supported $h_{ab}$ onto $f'(R)$. Combining the result with the stated matter variation and requiring every coefficient of $h_{ab}$ to vanish gives the [f(R) gravity](../../../general-relativity.md#f-r-gravity) equation

$$
\boxed{f'(R)R_{ab}-\frac12g_{ab}f(R)
+(g_{ab}\nabla_c\nabla^c-\nabla_a\nabla_b)f'(R)
=8\pi T_{ab}}.
$$

Therefore

$$
\boxed{\alpha'=1,
\qquad\beta'=-1}.
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

For [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), $R_{ab}=0$ and $R=0$, while $f'(R)$ is constant. In vacuum $T_{ab}=0$, so every derivative term vanishes and the remaining term is $-\tfrac12\eta_{ab}f(0)=0$. Hence Minkowski spacetime is a vacuum solution of this [modified gravity](../../../general-relativity.md#modified-gravity) theory.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Because $R=O(\epsilon)$ and

$$
f(0)=0,
\qquad f'(0)=1,
\qquad f''(0)=0,
$$

the [Taylor series](../../../calculus.md#taylor-series) gives $f(R)=R+O(\epsilon^3)$ and $f'(R)=1+O(\epsilon^2)$. The extra derivative terms in the f(R) equation are therefore at least second order. At first order the theory reduces to the [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations)

$$
G^{(1)}_{\mu\nu}=8\pi\mathcal T_{\mu\nu}.
$$

In [harmonic coordinates](../../../numerical-relativity.md#harmonic-coordinate), equivalently the [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity) $\partial_\mu\bar h^\mu{}_\nu=0$, the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation)

$$
\bar h_{\mu\nu}=h_{\mu\nu}-\frac12\eta_{\mu\nu}h
$$

satisfies

$$
\boxed{\partial^\rho\partial_\rho\bar h_{\mu\nu}
=-16\pi\mathcal T_{\mu\nu}},
\qquad
\boxed{\partial_\mu\bar h^\mu{}_\nu=0}.
$$

Thus [Linearized f(R) gravity about Minkowski spacetime](../../../general-relativity.md#linearized-f-r-gravity-about-minkowski-spacetime) has the same weak-field predictions as general relativity under these assumptions. Differences can first appear through nonlinear curvature terms or in backgrounds about which $f''(R)$ is nonzero.

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $v=\sqrt{2m/r}$. The proposed coframe gives

$$
-(e^0)^2+(e^1)^2+(e^2)^2+(e^3)^2
=-dt^2+(dr+vdt)^2+r^2d\theta^2+r^2\sin^2\theta\,d\phi^2,
$$

which expands to the stated metric. Hence it is the [orthonormal coframe in Painlevé–Gullstrand coordinates](../../../general-relativity.md#orthonormal-coframe-in-painleve-gullstrand-coordinates) with signature $(-,+,+,+)$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set

$$
a=\frac{v}{2r},
\qquad b=\frac1r,
\qquad c=\frac vr,
\qquad d=\frac{\cot\theta}{r}.
$$

Direct exterior differentiation gives

$$
de^0=0,
\qquad de^1=a,e^0\wedge e^1,
$$



$$
de^2=b,e^1\wedge e^2-c,e^0\wedge e^2,
$$



$$
de^3=b,e^1\wedge e^3-c,e^0\wedge e^3
+d,e^2\wedge e^3.
$$

Solving [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation) and imposing $\omega_{\mu\nu}=-\omega_{\nu\mu}$ gives the independent mixed-index [connection 1-forms](../../../connection-1-form.md)

$$
\boxed{\omega^0{}_1=a e^1,
\quad\omega^0{}_2=-c e^2,
\quad\omega^0{}_3=-c e^3},
$$



$$
\boxed{\omega^1{}_2=-b e^2,
\quad\omega^1{}_3=-b e^3,
\quad\omega^2{}_3=-d e^3}.
$$

The remaining forms follow from Lorentz-signature antisymmetry: $\omega^1{}_0=\omega^0{}_1$, $\omega^2{}_0=\omega^0{}_2$, $\omega^3{}_0=\omega^0{}_3$, and $\omega^j{}_i=-\omega^i{}_j$ for spatial indices.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write

$$
\Theta^\mu{}_\nu
=\frac12R^\mu{}_{\nu\rho\sigma}f^\rho\wedge f^\sigma.
$$

For a [diagonal curvature operator](../../../connection-1-form.md#diagonal-curvature-operator), $\Theta^{\mu\nu}$ contains only $f^\mu\wedge f^\nu$. Consequently $R^\mu{}_{\nu\rho\sigma}$ can be nonzero only when the plane indexed by $\rho,\sigma$ is the same as the plane indexed by $\mu,\nu$. In the contraction

$$
R_{\nu\sigma}=R^\mu{}_{\nu\mu\sigma},
$$

this condition cannot hold for $\nu\ne\sigma$. Therefore

$$
\boxed{R_{\nu\sigma}=0\quad\text{for }\nu\ne\sigma},
$$

which is the statement that a [diagonal curvature operator implies diagonal Ricci tensor](../../../connection-1-form.md#diagonal-curvature-operator-implies-diagonal-ricci-tensor).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Substituting the forms from part (b) into [Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation) gives the independent mixed-index [curvature 2-forms](../../../connection-1-form.md#curvature-2-form)

$$
\boxed{\Theta^0{}_1=\frac{2m}{r^3}e^0\wedge e^1,
\qquad
\Theta^0{}_2=-\frac{m}{r^3}e^0\wedge e^2,
\qquad
\Theta^0{}_3=-\frac{m}{r^3}e^0\wedge e^3},
$$



$$
\boxed{\Theta^1{}_2=-\frac{m}{r^3}e^1\wedge e^2,
\qquad
\Theta^1{}_3=-\frac{m}{r^3}e^1\wedge e^3,
\qquad
\Theta^2{}_3=\frac{2m}{r^3}e^2\wedge e^3}.
$$

Every form is proportional to its corresponding basis [2-form](../../../differential-form.md#2-form), so the curvature operator is diagonal. The diagonal [Ricci tensor](../../../general-relativity.md#ricci-tensor) components are contractions of these sectional curvature coefficients. In each case the coefficients cancel in the pattern $2-1-1=0$, with the Lorentzian sign included when the time direction is contracted. Hence

$$
\boxed{R_{\mu\nu}=0}.
$$

This is consistent with [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime) being a vacuum solution away from $r=0$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The [curvature 2-forms](../../../connection-1-form.md#curvature-2-form) show that orthonormal curvature components grow as $m/r^3$. The [geodesic deviation](../../../general-relativity.md#geodesic-deviation) equation converts them into the relative acceleration of nearby parts of an observer. As $r\to0$, the [Schwarzschild tidal force](../../../general-relativity.md#schwarzschild-tidal-force) stretches radial separations and compresses transverse separations with unbounded magnitude. An extended body therefore undergoes destructive tidal deformation before reaching the [Schwarzschild singularity](../../../general-relativity.md#schwarzschild-singularity).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
