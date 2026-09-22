# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_309.pdf)

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
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
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

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Fix the convention

$$
(\nabla_c\nabla_d-\nabla_d\nabla_c)X^a=R^a{}_{bcd}X^b.
$$

Equivalently,

$$
R(U,V)X=\nabla_U\nabla_VX-\nabla_V\nabla_UX-\nabla_{[U,V]}X.
$$

This defines the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) because it is $C^\infty(M)$-linear in $U,V,X$: derivatives of a multiplying function cancel between the three terms. Thus its value at a point depends only on the three tangent vectors there, rather than their extensions.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Apply the definition to the coordinate basis, for which $[\partial_\mu,\partial_\nu]=0$ and $\nabla_\mu\partial_\tau=\Gamma^\rho{}_{\tau\mu}\partial_\rho$. Comparing coefficients gives

$$
\boxed{R^\sigma{}_{\tau\mu\nu}
=\partial_\mu\Gamma^\sigma{}_{\tau\nu}
-\partial_\nu\Gamma^\sigma{}_{\tau\mu}
+\Gamma^\sigma{}_{\rho\mu}\Gamma^\rho{}_{\tau\nu}
-\Gamma^\sigma{}_{\rho\nu}\Gamma^\rho{}_{\tau\mu}},
$$

equivalent to the paper's ordering after commuting scalar factors. Although the individual [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) are not tensors, the preceding intrinsic definition proves that this complete combination is tensorial.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

At an arbitrary point choose [normal coordinates](../../../general-relativity.md#normal-coordinates), so the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) vanish there. Torsion freedom and commutation of partial derivatives then give the algebraic [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity)

$$
\boxed{R^a{}_{[bcd]}=0}.
$$

Differentiate the coordinate curvature expression and cyclically antisymmetrize. Third derivatives cancel, giving the [second Bianchi identity](../../../general-relativity.md#second-bianchi-identity)

$$
\boxed{\nabla_{[e}R^a{}_{|b|cd]}=0}.
$$

Both statements are tensorial and hence hold in every coordinate system. Contracting the differential identity, using the curvature symmetries and [metric compatibility](../../../fiber-bundle.md#metric-compatibility), yields

$$
\boxed{\nabla_aR^a{}_b-\frac12\nabla_bR=0},
$$

the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Contract the isotropic-curvature formula on $a,c$. In dimension $n$ it gives

$$
R_{bd}=(n-1)K g_{bd},
\qquad
R=n(n-1)K.
$$

Substitution into the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) gives

$$
(n-1)\nabla_bK=\frac12n(n-1)\nabla_bK.
$$

Since $n>2$, $\nabla_bK=0$, so $K$ is constant on each connected component. Thus this is [constant sectional curvature](../../../general-relativity.md#constant-sectional-curvature), with

$$
\boxed{K=\frac{R}{n(n-1)}}.
$$

This argument is [Schur theorem in pseudo-Riemannian geometry](../../../general-relativity.md#schur-theorem-in-pseudo-riemannian-geometry).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The vector $T^a$ is the tangent to a reference member of a one-parameter family of affinely parametrized [geodesics](../../../riemannian-geometry.md#geodesic). The [Jacobi field](../../../general-relativity.md#jacobi-field) $Y^a$ is the infinitesimal connecting vector from that geodesic to a neighboring one at equal parameter. The [geodesic deviation](../../../general-relativity.md#geodesic-deviation) equation states that curvature determines their relative acceleration.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

Parallel propagation means $\nabla_Te_\alpha=0$, where $T=\dot\lambda$. By [metric compatibility](../../../fiber-bundle.md#metric-compatibility),

$$
\frac d{dt}g(e_\alpha,e_\beta)
=g(\nabla_Te_\alpha,e_\beta)+g(e_\alpha,\nabla_Te_\beta)=0.
$$

The inner products therefore retain their initial values $\eta_{\alpha\beta}$, so the [parallel-propagated orthonormal frame](../../../general-relativity.md#parallel-propagated-orthonormal-frame) remains orthonormal.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

In the propagated frame $T=e_0$, and the [constant sectional curvature](../../../general-relativity.md#constant-sectional-curvature) formula reduces [geodesic deviation](../../../general-relativity.md#geodesic-deviation) to

$$
\ddot y^0=0,
\qquad
\ddot y^i=K y^i.
$$

The stated temporal initial data give $y^0(t)=0$. Writing $\omega=\sqrt{-K}$ for $K<0$ and $\kappa=\sqrt K$ for $K>0$, the spatial displacement is

$$
\boxed{
y^i(t)=
\begin{cases}
Y^i\cos(\omega t)+(V^i/\omega)\sin(\omega t),&K<0,\\
Y^i+V^it,&K=0,\\
Y^i\cosh(\kappa t)+(V^i/\kappa)\sinh(\kappa t),&K>0.
\end{cases}}
$$

These formulas are valid to first order in the initial separation and relative velocity.

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Vary $g^{ac}g_{cb}=\delta^a_b$. The [product rule](../../../calculus.md#product-rule) gives

$$
(\delta g^{ac})g_{cb}+g^{ac}\delta g_{cb}=0,
$$

and multiplication by $g^{bd}$ yields the [metric variation](../../../general-relativity.md#metric-variation)

$$
\boxed{\delta g^{ab}=-g^{ac}g^{bd}\delta g_{cd}}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The determinant identity $\delta\log|\det g|=g^{ab}\delta g_{ab}$ implies

$$
\delta\sqrt{|g|}=\frac12\sqrt{|g|}\,g^{ab}\delta g_{ab}.
$$

Hence the metric [volume form](../../../differential-form.md#volume-form) varies as

$$
\boxed{\delta(d\operatorname{vol}_g)
=\frac12g^{ab}\delta g_{ab}\,d\operatorname{vol}_g}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Varying the scalar and integrating by parts gives

$$
\delta S=\int_M
(\nabla_a\nabla^a\psi-\mu^2\psi)\delta\psi\,d\operatorname{vol}_g,
$$

because the boundary term vanishes by the support assumption. The [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore gives the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation)

$$
\boxed{\nabla_a\nabla^a\psi-\mu^2\psi=0}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Using both metric-variation formulas from part a gives the [Klein-Gordon scalar stress-energy tensor](../../../general-relativity.md#klein-gordon-scalar-stress-energy-tensor)

$$
\boxed{T^{ab}=\nabla^a\psi\nabla^b\psi
-\frac12g^{ab}\left(\nabla_c\psi\nabla^c\psi+\mu^2\psi^2\right)}.
$$

Its divergence is

$$
\nabla_aT^{ab}
=(\nabla_a\nabla^a\psi-\mu^2\psi)\nabla^b\psi,
$$

because the two Hessian terms cancel by symmetry. It vanishes on every solution of the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

[Killing equation](../../../general-relativity.md#killing-equation) is $\nabla_{(a}K_{b)}=0$. For the [stress-energy current from a Killing vector](../../../general-relativity.md#stress-energy-current-from-a-killing-vector) $J^a=T^a{}_bK^b$,

$$
\nabla_aJ^a=(\nabla_aT^{ab})K_b+T^{ab}\nabla_aK_b.
$$

The first term vanishes on shell, while the second contracts the symmetric tensor $T^{ab}$ with the antisymmetric derivative selected by Killing's equation. Thus $\boxed{\nabla_aJ^a=0}$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The coordinate formula for the [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) is

$$
(\mathcal L_Xg)_{ab}=X^c\partial_cg_{ab}
+g_{cb}\partial_aX^c+g_{ac}\partial_bX^c.
$$

For $X=\partial_t$, its components are constant and every metric coefficient is independent of $t$, so $\mathcal L_{\partial_t}g=0$. Hence $\partial_t$ is a timelike [Killing vector field](../../../general-relativity.md#killing-vector-field) and the metric is a [static spacetime](../../../general-relativity.md#static-spacetime).

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Let $K=\partial_t$ and let the future unit normal to $\Sigma_\tau$ be $n=f^{-1}\partial_t$. The conserved Killing energy is the flux

$$
E(\tau)=\int_{\Sigma_\tau}T_{ab}n^aK^b\sqrt h\,d^3x.
$$

Substitution of the [Klein-Gordon scalar stress-energy tensor](../../../general-relativity.md#klein-gordon-scalar-stress-energy-tensor) gives exactly

$$
E(\tau)=\frac12\int_{\Sigma_\tau}
\left[f^{-1}(\partial_t\psi)^2
+fh^{ij}\partial_i\psi\partial_j\psi+f\mu^2\psi^2\right]
\sqrt h\,d^3x.
$$

Apply the [divergence theorem](../../../calculus.md#divergence-theorem) to the slab $[\tau_1,\tau_2]\times\mathbb R^3$. The spatial-boundary flux vanishes because $\psi$ decays, and $\nabla_aJ^a=0$ makes the two time-slice fluxes equal. Thus this [conserved scalar-field energy in a static spacetime](../../../general-relativity.md#conserved-scalar-field-energy-in-a-static-spacetime) is independent of $\tau$.

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $g_{\mu\nu}=\eta_{\mu\nu}+\epsilon h_{\mu\nu}$. The [linearized inverse metric](../../../general-relativity.md#linearized-inverse-metric) is $g^{\mu\nu}=\eta^{\mu\nu}-\epsilon h^{\mu\nu}$, and all quadratic Christoffel products are $O(\epsilon^2)$. The wave-coordinate condition linearizes to

$$
\partial^\mu\bar h_{\mu\nu}=0,
\qquad
\bar h_{\mu\nu}=h_{\mu\nu}-\frac12\eta_{\mu\nu}h.
$$

Using the supplied Ricci formula then gives $G^{(1)}_{\mu\nu}=-\tfrac12\Box\bar h_{\mu\nu}$. Consequently the [Linearized Einstein equations](../../../general-relativity.md#linearized-einstein-equations) in [Lorenz gauge in linearized gravity](../../../general-relativity.md#lorenz-gauge-in-linearized-gravity) are

$$
\boxed{\Box\bar h_{\mu\nu}=-16\pi T_{\mu\nu}},
\qquad
\boxed{\partial^\mu\bar h_{\mu\nu}=0}.
$$

This Lorenz condition is the first-order form of the [harmonic coordinate](../../../numerical-relativity.md#harmonic-coordinate) equations.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

To first order in the angular velocity, $T^{00}=\rho$ and $T^{i0}=\rho v^i$ with $v=(-\Omega y,\Omega x,0)$. The conservation equation $\partial_\mu T^{\mu0}=0$ and time independence give

$$
0=\nabla\mathbin\cdot(\rho\mathbf v)
=\Omega(x\partial_y\rho-y\partial_x\rho).
$$

Thus $\boxed{x\partial_y\rho-y\partial_x\rho=0}$: the density is invariant under rotations about the z-axis.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Stationarity changes $\Box$ to the spatial [Laplace operator](../../../partial-differential-equation.md#laplace-operator). The Green function of the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) therefore gives

$$
\boxed{\bar h_{00}(\mathbf r)=4\int_{\mathbb R^3}
\frac{\rho(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r'},
$$



$$
\boxed{\bar h_{0i}(\mathbf r)=4\Omega\int_{\mathbb R^3}
\frac{\rho(\mathbf r')}{|\mathbf r-\mathbf r'|}
(y',-x',0)_i\,d^3r'},
\qquad
\boxed{\bar h_{ij}=0}.
$$

Here the bar denotes the [trace-reversed metric perturbation](../../../general-relativity.md#trace-reversed-metric-perturbation); this is the variable denoted by $h$ in the displayed field equation of the question.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

For $r\gg R$, the [multipole expansion](../../../electromagnetism.md#electric-multipole-expansion) is

$$
\frac1{|\mathbf r-\mathbf r'|}
=\frac1r+\frac{\mathbf r\cdot\mathbf r'}{r^3}
+O(R^2/r^3).
$$

The [center of mass](../../../classical-mechanics.md#center-of-mass) condition removes the mass dipole. Axisymmetry makes the mixed second moments vanish and gives $\int\rho x'^2=\int\rho y'^2$. Undoing trace reversal therefore yields

$$
ds^2=-\left(1-\frac{2m}{r}\right)dt^2
+\left(1+\frac{2m}{r}\right)d\mathbf r^2
+\frac{4ma}{r^3}(y\,dx-x\,dy)dt,
$$

where

$$
\boxed{m=\int\rho\,d^3r',
\qquad
ma=J_z=\Omega\int\rho(x'^2+y'^2)\,d^3r'}.
$$

**Thus $a=J_z/m$ is the [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum), and the cross term is the dipole part of the [slowly rotating weak-field metric](../../../general-relativity.md#slowly-rotating-weak-field-metric).**

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Contract $\nabla_aT^{ab}=0$ for the [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) with $u_b$. Using $u_bu^b=-1$ and $u_b\nabla_au^b=0$ gives the [relativistic perfect-fluid energy equation](../../../general-relativity.md#relativistic-perfect-fluid-energy-equation)

$$
\boxed{u^a\nabla_a\rho+(\rho+p)\nabla_au^a=0},
$$

the local [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics). Project instead with $g^a{}_b+u^au_b$ to obtain the [relativistic Euler equation](../../../general-relativity.md#relativistic-euler-equation)

$$
\boxed{(\rho+p)u^b\nabla_bu^a
=-(g^{ab}+u^au^b)\nabla_bp}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Direct differentiation gives, for example,

$$
d\sigma^3=-\sin\theta\,d\theta\wedge d\phi
=\sigma^1\wedge\sigma^2.
$$

Differentiating $\sigma^1,\sigma^2$ similarly and substituting the definitions yields $d\sigma^1=\sigma^2\wedge\sigma^3$ and $d\sigma^2=\sigma^3\wedge\sigma^1$. Hence these [Maurer-Cartan forms](../../../lie-theory.md#maurer-cartan-form) on the three-sphere obey

$$
\boxed{d\sigma^i=\frac12\delta^{il}\epsilon_{ljk}
\sigma^j\wedge\sigma^k}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Since $de^0=0$ and $de^i=\tfrac12\epsilon^i{}_{jk}e^j\wedge e^k$, [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation) gives

$$
\boxed{\omega^0{}_\mu=0,
\qquad \omega^i{}_j=\frac12\epsilon^i{}_{jk}e^k}.
$$

[Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation) then gives

$$
\boxed{\Theta^0{}_\mu=0,
\qquad \Theta^i{}_j=\frac14e^i\wedge e^j}.
$$

Using $\Theta^i{}_j=\tfrac12R^i{}_{jkl}e^k\wedge e^l$ yields

$$
\boxed{R_{ijkl}=\frac14(\delta_{ik}\delta_{jl}-\delta_{il}\delta_{jk})},
$$

with no time-index curvature components. Contraction gives

$$
R_{00}=0,
\qquad R_{ij}=\frac12\delta_{ij},
\qquad R=\frac32,
$$

and therefore

$$
\boxed{G_{00}=\frac34,
\qquad G_{ij}=-\frac14\delta_{ij},
\qquad G_{0i}=0}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

In the orthonormal frame, the comoving [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) has $T_{00}=\rho$ and $T_{ij}=p\delta_{ij}$. The [Einstein field equations](../../../general-relativity.md#einstein-field-equations) with [cosmological constant](../../../cosmology.md#cosmological-constant) therefore give

$$
\frac34-\Lambda=8\pi\rho,
\qquad
-\frac14+\Lambda=8\pi p.
$$

Thus

$$
\boxed{\rho=\frac{3/4-\Lambda}{8\pi},
\qquad p=\frac{\Lambda-1/4}{8\pi}}.
$$

Choosing

$$
\boxed{\Lambda=\frac14}
$$

gives $p=0$ and $\rho=1/(16\pi)>0$. The metric is then the [Einstein static universe](../../../general-relativity.md#einstein-static-universe) supported by pressureless matter and positive vacuum energy.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
