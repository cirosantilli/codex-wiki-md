# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_107.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma) requires an [interior sphere condition](../../../elliptic-boundary-value-problem.md#interior-sphere-condition), strictness of the boundary maximum, and quantitative control of the [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) near the contact point. Assume that $y\in\partial\Omega$, that $B_R(z)\subset\Omega$ and $\overline{B_R(z)}\setminus\{y\}\subset\Omega$, and that $|y-z|=R$. After shrinking the tangent [open ball](../../../topology.md#open-ball), we may suppose that the coefficients are bounded there and that, for constants $0<\lambda\leq\Lambda$ and $B<\infty$,

$$
\lambda|\xi|^2\leq a^{ij}(x)\xi_i\xi_j\leq\Lambda|\xi|^2,
\qquad |b(x)|\leq B.
$$

The coefficient [matrix](../../../vector-space.md#matrix) may be replaced by its [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) part because the [Hessian matrix](../../../calculus.md#hessian-matrix) is symmetric. Assume also that $u(x)<u(y)$ throughout the tangent [open ball](../../../topology.md#open-ball). In the usual statement, one assumes $u(x)<u(y)$ throughout $\Omega$; when $\Omega$ is [connected](../../../geometry-and-topology.md#connected-space), the [strong maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-maximum-principle-for-elliptic-operators) supplies this strictness from a nonconstant solution attaining its global maximum at $y$.

Put $\mathbf n=(y-z)/R$, the outward [unit normal](../../../differential-geometry.md#unit-normal) of the tangent [open ball](../../../topology.md#open-ball). With only the given [continuity](../../../calculus.md#continuous-function) at $y$, the precise conclusion is

$$
\boxed{\liminf_{t\downarrow0}\frac{u(y)-u(y-t\mathbf n)}{t}>0.}
$$

**If the outward normal derivative exists, it is strictly positive.** In particular, if $u$ is [continuously differentiable](../../../calculus.md#continuously-differentiable-function) up to $y$ and the domain has this outward [unit normal](../../../differential-geometry.md#unit-normal), then $\partial_{\mathbf n}u(y)>0$. The stated $C^0$ boundary regularity alone does not assert existence of a [normal derivative](../../../differential-geometry.md#normal-derivative).

For the proof, use the annulus $A=\{R/2<|x-z|<R\}$ and the [barrier for the Dirichlet problem](../../../analysis.md#barrier-for-the-dirichlet-problem)

$$
v(x)=e^{-k|x-z|^2}-e^{-kR^2}.
$$

Writing $q=x-z$, direct [differentiation](../../../calculus.md#differentiation) gives

$$
Lv=e^{-k|q|^2}\bigl(4k^2a^{ij}q_iq_j-2k\operatorname{tr}a-2kb\cdot q\bigr)
\geq e^{-k|q|^2}\bigl(k^2\lambda R^2-2k(n\Lambda+BR)\bigr).
$$

Choose $k>2(n\Lambda+BR)/(\lambda R^2)$, so that $Lv>0$ on $A$. On the inner sphere, [compactness](../../../topology.md#compact-space) and the strict maximum give $m=\min_{|x-z|=R/2}(u(y)-u(x))>0$. Choose $\varepsilon>0$ with $\varepsilon\max_{|x-z|=R/2}v\leq m$. On the outer sphere $v=0$ and $u-u(y)\leq0$, including at $y$ by [continuity](../../../calculus.md#continuous-function). Consequently $w=u-u(y)+\varepsilon v$ has $Lw\geq0$ and nonpositive boundary values. The allowed comparison principle, or the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators), yields $w\leq0$ in $A$.

Along the inward radius this gives

$$
\frac{u(y)-u(y-t\mathbf n)}t\geq
\varepsilon\frac{e^{-k(R-t)^2}-e^{-kR^2}}t
\longrightarrow 2\varepsilon kR e^{-kR^2}>0.
$$

This proves the [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma). There is no sign restriction on $u(y)$ here, because the operator has no zeroth-order term.

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

**A bounded-domain hypothesis is needed for the requested global construction and uniqueness.** The printed question does not include it. For example, the upper half-plane satisfies the stated [exterior cone condition](../../../analysis.md#exterior-cone-condition), but both $u=0$ and $u(x_1,x_2)=x_2$ are [harmonic functions](../../../partial-differential-equation.md#harmonic-function) with zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition). Thus part (iv), in its printed unrestricted solution class, is false. In this question's solutions we add that $\Omega$ is bounded; the [exterior cone condition](../../../analysis.md#exterior-cone-condition) and all other data remain as printed.

The half-plane also rules out the printed global separated barrier. In its angular interval $(0,\pi)$, varying $r$ on a fixed ray forces $\nu=2$ if $r^{\nu-2}(h''+\nu^2h)\geq\delta>0$ for every $r>0$. We would then have $h''+4h\geq\delta$ and $h<0$. Put $a=\pi/4$ and $b=3\pi/4$. Twice [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\int_a^b(h''+4h)\sin(2(\theta-a))\,d\theta=2\bigl(h(a)+h(b)\bigr)<0,
$$

contradicting the positive integrand. Thus a source qualification is necessary for part (i) as well as part (iv).

Fix $x_0$ and its exterior cone of half-angle $\alpha$. Choose $0<\alpha_0<\min(\alpha,\pi/2)$ and set

$$
\beta=\frac{\pi}{2(\pi-\alpha_0)},\qquad 0<\nu<\beta<1.
$$

On the complement of the cone, unwrap the angle in [polar coordinates](../../../calculus.md#polar-coordinates) as $\vartheta\in(\alpha,2\pi-\alpha)$, measured from the cone axis. Then $\psi=\vartheta-\pi$ is the angle from the opposite axis and $|\psi|\leq\pi-\alpha$ on $\overline\Omega\setminus\{x_0\}$. Define the [power barrier for an exterior cone](../../../analysis.md#power-barrier-for-an-exterior-cone) by

$$
\boxed{g(r,\vartheta)=-r^\nu\cos\bigl(\beta(\vartheta-\pi)\bigr),\qquad g(x_0)=0.}
$$

This has the requested separated form $r^\nu h(\vartheta)$. In the printed signed-angle convention, the same function is $-r^\nu\cos(\beta(\pi-|\theta|))$ outside the cone. It is smooth across the negative axis: near that axis the angular expression is the even function $\cos(\beta\psi)$.

Since $\beta(\pi-\alpha)<\pi/2$, put $m=\cos(\beta(\pi-\alpha))>0$. The cosine is at least $m$, so $g\leq-mr^\nu<0$ away from $x_0$, and $g$ is [continuous](../../../calculus.md#continuous-function) at $x_0$. The [Laplacian in polar coordinates](../../../calculus.md#laplacian-in-polar-coordinates) gives

$$
\Delta g=(\beta^2-\nu^2)r^{\nu-2}\cos(\beta\psi).
$$

Let $D=\sup_{x\in\Omega}|x-x_0|<\infty$. Since $\nu<2$, the [barrier for the Dirichlet problem](../../../analysis.md#barrier-for-the-dirichlet-problem) satisfies

$$
\boxed{\Delta g\geq\delta:=(\beta^2-\nu^2)mD^{\nu-2}>0.}
$$

Both the uniform lower bound and the later global comparison use boundedness. In particular, $-g$ is positive at every other boundary point, and is bounded away from zero on boundary sets staying a positive distance from $x_0$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For the bounded-domain correction, let $\mathcal S$ be the family of [Perron subfunctions for the Poisson equation](../../../analysis.md#perron-subfunction-for-the-poisson-equation) $v\in C^0(\overline\Omega)$ with $v\leq\varphi$ on $\partial\Omega$. The subfunction condition is ball comparison: whenever $\overline B\subset\Omega$ and a [classical solution](../../../partial-differential-equation.md#classical-solution) $H$ of $\Delta H=f$ on $B$ satisfies $v\leq H$ on $\partial B$, it also satisfies $v\leq H$ throughout $B$. For a $C^2$ function this is the sign condition $\Delta v\geq f$. A superfunction reverses both inequalities.

**The Perron solution is the pointwise upper envelope of the subfunctions:**

$$
\boxed{u(x)=\sup_{v\in\mathcal S}v(x),\qquad x\in\Omega.}
$$

This is the [Perron method for the Dirichlet problem](../../../analysis.md#perron-method) with the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) replacing the homogeneous [Laplace equation](../../../partial-differential-equation.md#laplace-equation). The [power barrier for an exterior cone](../../../analysis.md#power-barrier-for-an-exterior-cone) supplies a global member of $\mathcal S$ and a global superfunction, as constructed below. The permitted subfunction-superfunction comparison therefore makes this envelope finite. The standard interior Perron theorem, available in the question, gives $u\in C^2(\Omega)$ and $\Delta u=f$; neither result needs to be proved in this part.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Fix $x_0\in\partial\Omega$, $\varepsilon>0$, and the [power barrier for an exterior cone](../../../analysis.md#power-barrier-for-an-exterior-cone) $g$ from part (i). Write $M=\|f\|_\infty$. By [continuity](../../../calculus.md#continuous-function) of the boundary data, there is $\rho>0$ such that $|\varphi(x)-\varphi(x_0)|<\varepsilon$ on $\partial\Omega\cap B_\rho(x_0)$. On the rest of the boundary, $-g\geq m\rho^\nu$. The boundary is [compact](../../../topology.md#compact-space), so $\varphi$ is bounded. Choose $A>0$ large enough that $A\delta\geq M$ and

$$
A(-g(x))\geq|\varphi(x)-\varphi(x_0)|
\quad\text{on }\partial\Omega\setminus B_\rho(x_0).
$$

Then the [Perron subfunction for the Poisson equation](../../../analysis.md#perron-subfunction-for-the-poisson-equation) and its superfunction counterpart

$$
v_-(x)=\varphi(x_0)-\varepsilon+Ag(x),\qquad
v_+(x)=\varphi(x_0)+\varepsilon-Ag(x)
$$

satisfy $\Delta v_-\geq M\geq f$, $\Delta v_+\leq-M\leq f$, and $v_-\leq\varphi\leq v_+$ on the whole boundary. The near-boundary ordering uses the choice of $\rho$; the remaining ordering uses the choice of $A$. In particular the Perron family is nonempty and bounded above.

The [Perron method for the Dirichlet problem](../../../analysis.md#perron-method) and the permitted comparison give $v_-\leq u\leq v_+$. Since $g(x)\to0$ as $x\to x_0$, we obtain

$$
\varphi(x_0)-\varepsilon\leq\liminf_{x\to x_0}u(x)
\leq\limsup_{x\to x_0}u(x)\leq\varphi(x_0)+\varepsilon.
$$

Letting $\varepsilon\downarrow0$ proves

$$
\boxed{\lim_{\Omega\ni x\to x_0}u(x)=\varphi(x_0).}
$$

The interior Perron theorem gives [continuity](../../../calculus.md#continuous-function) inside $\Omega$, and the displayed limit together with [continuity](../../../calculus.md#continuous-function) of $\varphi$ proves **the continuous extension $u\in C^0(\overline\Omega)$ with the required boundary trace**. Thus every boundary point is a [regular boundary point](../../../analysis.md#regular-boundary-point).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For the corrected bounded-domain problem, the interior theorem for the [Perron method for the Dirichlet problem](../../../analysis.md#perron-method) gives a [classical solution](../../../partial-differential-equation.md#classical-solution) of the [Poisson equation](../../../partial-differential-equation.md#poisson-equation), and the [power barrier for an exterior cone](../../../analysis.md#power-barrier-for-an-exterior-cone) argument gives its continuous extension with the required [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition). Hence existence holds in $C^2(\Omega)\cap C^0(\overline\Omega)$.

If $u_1,u_2$ are two such [classical solutions](../../../partial-differential-equation.md#classical-solution), then $w=u_1-u_2$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) with zero boundary trace. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators), applied to $w$ and $-w$ on the bounded domain, gives $w\leq0$ and $-w\leq0$. Consequently

$$
\boxed{u_1=u_2.}
$$

**There is exactly one solution after adding boundedness of $\Omega$.** For the printed unbounded-domain version, the half-plane counterexample in part (i) disproves uniqueness; an additional condition at infinity or a suitable restricted solution class would instead have to be specified.

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Choose a [smooth cutoff function](../../../analysis.md#smooth-cutoff-function) $\eta$ supported in $B_2$, equal to one on $B_1$, with $0\leq\eta\leq1$ and $|D\eta|\leq C$. For $i<n$, put $v_i=D_i u$. The zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) implies that the [tangential boundary derivative](../../../differential-equation.md#tangential-boundary-derivative) $v_i$ vanishes on the flat face. Differentiating the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) gives $\Delta v_i=D_i f$. Test this equation with $\eta^2v_i$. The boundary terms vanish because $v_i=0$ on the flat face and $\eta=0$ near the curved face. [Integration by parts](../../../calculus.md#integration-by-parts) in the tangential direction moves $D_i$ off $f$, yielding

$$
\int_{B_2^+}\eta^2|Dv_i|^2
=\int_{B_2^+}fD_i(\eta^2v_i)
-2\int_{B_2^+}\eta v_i Dv_i\cdot D\eta.
$$

This is the essential [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) step: it involves $f$, rather than $Df$. Expanding $D_i(\eta^2v_i)$ and using the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) gives

$$
\int\eta^2|Dv_i|^2
\leq\frac12\int\eta^2|Dv_i|^2
+C\int\bigl(f^2+v_i^2|D\eta|^2\bigr).
$$

The term $f\eta(D_i\eta)v_i$ is bounded by $C f^2+C|D\eta|^2v_i^2$. Absorbing the first term and summing over $i<n$ proves the hinted estimate:

$$
\sum_{i<n}\sum_{j=1}^n\|D_{ij}u\|_{L^2(B_1^+)}^2
\leq C(n)\left(\|Du\|_{L^2(B_2^+)}^2+\|f\|_{L^2(B_2^+)}^2\right).
$$

All mixed second [partial derivatives](../../../calculus.md#partial-derivative) are now controlled, since $D_{ni}u=D_{in}u$. The remaining [normal derivative](../../../differential-geometry.md#normal-derivative) is recovered from the equation:

$$
D_{nn}u=f-\sum_{i<n}D_{ii}u.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) bounds its squared [L2 norm](../../../real-analysis.md#l2-norm) by $n$ times the sum of the squared [L2 norms](../../../real-analysis.md#l2-norm) on the right. Including the already controlled zeroth and first [partial derivatives](../../../calculus.md#partial-derivative), and taking square roots, gives the [second-derivative estimate at a flat Dirichlet boundary](../../../distribution-theory.md#second-derivative-estimate-at-a-flat-dirichlet-boundary):

$$
\boxed{\|u\|_{W^{2,2}(B_1^+)}\leq C(n)\left(\|u\|_{W^{1,2}(B_2^+)}+\|f\|_{L^2(B_2^+)}\right).}
$$

**The full second-order Sobolev norm is controlled without any norm of $Df$.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use [homogenization of Dirichlet boundary data](../../../sobolev-space.md#homogenization-of-dirichlet-boundary-data): put $v=u-\varphi$, using the supplied extension of $\varphi$ to the half-ball. Then $v=0$ on the flat face and $\Delta v=f-\Delta\varphi$. The [second-derivative estimate at a flat Dirichlet boundary](../../../distribution-theory.md#second-derivative-estimate-at-a-flat-dirichlet-boundary) from part (a) gives

$$
\|v\|_{W^{2,2}(B_1^+)}
\leq C(n)\left(\|v\|_{W^{1,2}(B_2^+)}+\|f-\Delta\varphi\|_{L^2(B_2^+)}\right).
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $\|v\|_{W^{1,2}}\leq\|u\|_{W^{1,2}}+\|\varphi\|_{W^{1,2}}$, while the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) bounds $\|\Delta\varphi\|_{L^2}$ by $\sqrt n\|D^2\varphi\|_{L^2}$. Finally $u=v+\varphi$, so restriction from the larger half-ball and another [triangle inequality](../../../topological-analysis.md#triangle-inequality) give

$$
\boxed{\|u\|_{W^{2,2}(B_1^+)}\leq C(n)\left(\|u\|_{W^{1,2}(B_2^+)}+\|f\|_{L^2(B_2^+)}+\|\varphi\|_{W^{2,2}(B_2^+)}\right).}
$$

**Nonzero boundary data contribute the second-order Sobolev norm of their extension.** No estimate for a separately constructed extension is needed, because $\varphi$ is already given on the half-ball.

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Write the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph) as $\operatorname{div}F(Du)=0$ in its [weak formulation](../../../partial-differential-equation.md#weak-formulation), where $F(p)=p/\sqrt{1+|p|^2}$. For negative increments use the same [difference quotient](../../../calculus.md#difference-quotient) convention, so

$$
w_h=\delta_{\ell,-h}u=\frac{u(x)-u(x-he_\ell)}h.
$$

For $\zeta\in C_c^1(\Omega'')$, the function $\delta_{\ell,h}\zeta$ is an admissible [test function](../../../distribution-theory.md#test-function) in $\Omega$. Commuting the first [partial derivative](../../../calculus.md#partial-derivative) with translation, then applying [discrete integration by parts](../../../calculus.md#discrete-integration-by-parts), gives

$$
0=\int_\Omega F_i(Du)\delta_{\ell,h}(D_i\zeta)
=-\int_{\Omega''}\delta_{\ell,-h}(F_i(Du))D_i\zeta.
$$

The [fundamental theorem of calculus along a line segment](../../../calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) gives the [averaged linearization of a nonlinear divergence-form equation](../../../partial-differential-equation.md#averaged-linearization-of-a-nonlinear-divergence-form-equation)

$$
\delta_{\ell,-h}(F_i(Du))=A_h^{ij}(x)D_jw_h,
\qquad
A_h(x)=\int_0^1DF\bigl((1-t)Du(x-he_\ell)+tDu(x)\bigr)\,dt.
$$

Thus **the backward difference quotient solves a linear equation in divergence form**:

$$
\boxed{D_i(A_h^{ij}D_jw_h)=0\quad\text{weakly on }\Omega''.}
$$

To verify the [ellipticity of the minimal surface flux](../../../second-fundamental-form.md#ellipticity-of-the-minimal-surface-flux), compute

$$
DF(p)=\frac{I}{\sqrt{1+|p|^2}}-\frac{p\otimes p}{(1+|p|^2)^{3/2}},
$$

and hence

$$
\frac{|\xi|^2}{(1+|p|^2)^{3/2}}
\leq \xi\cdot DF(p)\xi
\leq |\xi|^2.
$$

The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) parallel to $p$ is $(1+|p|^2)^{-3/2}$; every orthogonal [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $(1+|p|^2)^{-1/2}$. The same lower and upper bounds pass to the averaged [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A_h$ whenever both endpoint [gradients](../../../calculus.md#gradient) have norm at most $M$:

$$
\boxed{(1+M^2)^{-3/2}|\xi|^2\leq A_h^{ij}\xi_i\xi_j\leq|\xi|^2.}
$$

The printed $C^1(\Omega)$ hypothesis supplies such an $M$ on each [relatively compact subset](../../../topological-analysis.md#relatively-compact-subset), uniformly for sufficiently small $h$. It therefore establishes a locally [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator). A single lower bound on all of $\Omega''$ additionally requires bounded [gradients](../../../calculus.md#gradient) there and at the shifted points; this is automatic for bounded $\Omega$ and fixed $h$, but is not supplied on an arbitrary open set.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Fix nested [relatively compact subsets](../../../topological-analysis.md#relatively-compact-subset) of $\Omega$ and let $M$ bound the [gradient](../../../calculus.md#gradient) on the larger one. The [fundamental theorem of calculus along a line segment](../../../calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) gives $|w_h|\leq M$ on the smaller one. Part (i) gives coefficient bounds independent of small $h$, so the [De Giorgi-Nash-Moser theorem](../../../elliptic-boundary-value-problem.md#de-giorgi-nash-moser-theorem) gives uniform interior [Hölder continuity](../../../sobolev-space.md#holder-condition) estimates for these [weak solutions](../../../partial-differential-equation.md#weak-solution). Since $Du$ is [continuous](../../../calculus.md#continuous-function), the [difference quotients](../../../calculus.md#difference-quotient) $w_h$ converge locally uniformly to $D_\ell u$. Passing to the limit in the [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) estimate, and repeating for every coordinate, yields

$$
\boxed{u\in C^{1,\alpha}\text{ on each compactly contained subdomain, for some }\alpha>0.}
$$

**The first derivatives are locally Hölder continuous.** Here the initially obtained exponent depends on $n$ and the local [gradient](../../../calculus.md#gradient) bound. This is the interior interpretation of the printed regularity conclusion; a uniform global estimate does not follow from $u\in C^1(\Omega)$ alone.

## 5

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Assume $u\in W^{1,2}(B_2(0))$ is nonnegative [almost everywhere](../../../measure-theory.md#almost-everywhere), and that the real coefficient [matrix](../../../vector-space.md#matrix) $A=(a^{ij})$ is measurable and satisfies, for almost every $x$ and every $\xi\in\mathbb R^n$,

$$
\xi\cdot A(x)\xi\geq\lambda|\xi|^2,\qquad
|A(x)\xi|\leq\Lambda|\xi|,
\qquad 0<\lambda\leq\Lambda<\infty.
$$

The [operator norm](../../../continuous-dual-space.md#operator-norm) bound controls all coefficients, including any antisymmetric part. For a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), these assumptions are exactly the usual lower and upper quadratic-form bounds. The [weak solution](../../../partial-differential-equation.md#weak-solution) condition is

$$
\int_{B_2}a^{ij}D_j uD_i\zeta=0\qquad(\zeta\in C_c^\infty(B_2)).
$$

Then the [Harnack inequality for uniformly elliptic divergence-form equations](../../../elliptic-boundary-value-problem.md#harnack-inequality-for-uniformly-elliptic-divergence-form-equations) is

$$
\boxed{\operatorname*{ess\,sup}_{B_1}u\leq C(n,\Lambda/\lambda)\operatorname*{ess\,inf}_{B_1}u.}
$$

**A nonnegative weak solution has its supremum controlled by its infimum on the smaller ball.** The [De Giorgi-Nash-Moser theorem](../../../elliptic-boundary-value-problem.md#de-giorgi-nash-moser-theorem) supplies a [Hölder continuous function](../../../sobolev-space.md#holder-condition) representative, for which ordinary supremum and infimum can replace the [essential supremum](../../../measure-theory.md#essential-supremum) and [essential infimum](../../../real-analysis.md#essential-infimum). Nonnegativity and the larger ball are essential hypotheses; there is no differentiability requirement on the coefficients.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

There is no need to assume that the original zeroth-order coefficient is nonpositive. Set $c_+=\max(c,0)$ and $\widetilde c=\min(c,0)$, and use the [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator)

$$
\widetilde L=a^{ij}D_{ij}+b^iD_i+\widetilde c.
$$

Because $u\geq0$ and $f\leq0$,

$$
\widetilde Lu=f-c_+u\leq0.
$$

Now $\widetilde c\leq0$, so the [strong minimum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators) applies. If $u$ vanished at an interior point of the [connected](../../../geometry-and-topology.md#connected-space) domain, this principle would force $u$ to vanish identically. The given nontriviality therefore proves

$$
\boxed{u(x)>0\qquad(x\in\Omega).}
$$

**Every nontrivial nonnegative solution is strictly positive inside.** This uses the nondivergence-form [strong minimum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators); the divergence-form [Harnack inequality for uniformly elliptic divergence-form equations](../../../elliptic-boundary-value-problem.md#harnack-inequality-for-uniformly-elliptic-divergence-form-equations) in part (a) is not being applied to this operator.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Take $\Omega'$ nonempty and compactly contained in $\Omega$. The argument is a [compactness proof of a nonnegative elliptic solution estimate](../../../elliptic-boundary-value-problem.md#compactness-proof-of-a-nonnegative-elliptic-solution-estimate), with the [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) retaining control all the way to the boundary. The operator and the [Hölder space](../../../sobolev-space.md#holder-space) exponent are fixed throughout.

Suppose the estimate fails. For each integer $k$ there is an admissible nonnegative solution $u_k$, with forcing $f_k$, such that

$$
M_k:=\sup_\Omega u_k>k\left(\inf_{\Omega'}u_k+\|f_k\|_{C^{0,\mu}(\overline\Omega)}\right).
$$

Put $v_k=u_k/M_k$ and $g_k=f_k/M_k$. Then $0\leq v_k\leq1$, $\max_{\overline\Omega}v_k=1$, $v_k=0$ on the boundary, $Lv_k=g_k$, and

$$
\inf_{\Omega'}v_k<\frac1k,\qquad
\|g_k\|_{C^{0,\mu}(\overline\Omega)}<\frac1k.
$$

Global [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) and the [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) for zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) give

$$
\|v_k\|_{C^{2,\mu}(\overline\Omega)}\leq C\left(\|v_k\|_{C^0(\overline\Omega)}+\|g_k\|_{C^{0,\mu}(\overline\Omega)}\right)\leq2C.
$$

This estimate includes the $C^0$ term, so it does not require invertibility of $L$ or a sign restriction on $c$. The [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces), or the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) applied through second [partial derivatives](../../../calculus.md#partial-derivative), gives a subsequence converging in $C^2(\overline\Omega)$ to $v$. Thus $v\geq0$, $Lv=0$, $v=0$ on the boundary, and $\max v=1$.

Choose $x_k\in\Omega'$ with $v_k(x_k)\leq\inf_{\Omega'}v_k+1/k$. A further subsequence has $x_k\to x_*\in\overline{\Omega'}\subset\Omega$. [Uniform convergence](../../../real-analysis.md#uniform-convergence) yields $v(x_*)=0$. Part (b) says that a nonnegative homogeneous solution on the [connected](../../../geometry-and-topology.md#connected-space) domain is either zero everywhere or strictly positive inside. Both alternatives contradict, respectively, $\max v=1$ and $v(x_*)=0$. Therefore

$$
\boxed{\sup_\Omega u\leq C(n,L,\Omega',\Omega)\left(\inf_{\Omega'}u+\|f\|_{C^{0,\mu}(\overline\Omega)}\right).}
$$

**The interior infimum and the forcing control the global supremum.** Global boundary control is crucial here: an interior-only [compactness](../../../topology.md#compact-space) argument could lose the normalized maximum at the boundary.

## 6

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Multiply the [Dirichlet Laplacian eigenfunction](../../../partial-differential-equation.md#dirichlet-laplacian-eigenfunction) equation by $u$ and use [integration by parts](../../../calculus.md#integration-by-parts). The zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) removes the boundary term and gives

$$
\lambda\int_\Omega u^2=\int_\Omega|Du|^2.
$$

The denominator is positive because the [eigenfunction](../../../linear-operator-theory.md#eigenfunction) is nonzero. The numerator is also positive: if it were zero, the given [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) for $u\in W_0^{1,2}(\Omega)$ would force $u=0$. Therefore the [Dirichlet Laplacian eigenvalue](../../../partial-differential-equation.md#dirichlet-laplacian-eigenvalue) has the positive [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient)

$$
\boxed{\lambda=\frac{\int_\Omega|Du|^2}{\int_\Omega u^2}>0.}
$$

**Every nonzero Dirichlet eigenfunction in this problem has a positive eigenvalue.**

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Use a [signed power test for a Laplacian eigenfunction](../../../partial-differential-equation.md#signed-power-test-for-a-laplacian-eigenfunction). For $\gamma\geq2$, test the [Dirichlet Laplacian eigenfunction](../../../partial-differential-equation.md#dirichlet-laplacian-eigenfunction) equation with $|u|^{\gamma-2}u$. Its derivative is $(\gamma-1)|u|^{\gamma-2}Du$; at $\gamma=2$ the test function is just $u$. [Integration by parts](../../../calculus.md#integration-by-parts) gives the exact [energy estimate](../../../partial-differential-equation.md#energy-estimate)

$$
(\gamma-1)\int_\Omega |u|^{\gamma-2}|Du|^2=\lambda\int_\Omega |u|^\gamma.
$$

Set $v=|u|^{\gamma/2}$. It belongs to the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) and obeys the [Sobolev chain rule](../../../distribution-theory.md#sobolev-chain-rule):

$$
\int_\Omega|Dv|^2=\frac{\gamma^2}{4}\int_\Omega|u|^{\gamma-2}|Du|^2
=\frac{\lambda\gamma^2}{4(\gamma-1)}\int_\Omega|u|^\gamma.
$$

For $\gamma>2$, the power map is $C^1$ with bounded derivative on the bounded range of $u$. For $\gamma=2$, the [absolute value](../../../real-analysis.md#absolute-value) map is Lipschitz, and $D|u|=\operatorname{sgn}(u)Du$ [almost everywhere](../../../measure-theory.md#almost-everywhere); on the zero set, use the fact that a [gradient of a Sobolev function vanishes on a level set](../../../distribution-theory.md#gradient-of-a-sobolev-function-vanishes-on-a-level-set). These facts justify the identity even when $u$ changes sign.

Apply the given [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) with the [Sobolev conjugate exponent](../../../sobolev-space.md#sobolev-conjugate-exponent) $2\kappa=2n/(n-2)$:

$$
\boxed{\left(\int_\Omega|u|^{\gamma\kappa}\right)^{1/\kappa}
\leq\frac{C(n)\lambda\gamma^2}{4(\gamma-1)}\int_\Omega|u|^\gamma.}
$$

**Testing with a signed power raises the integrability exponent from $\gamma$ to $\gamma\kappa$.** Absorbing the factor $1/4$ into $C(n)$ gives precisely the requested inequality.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

Put $p_j=2\kappa^j$, where $\kappa=n/(n-2)>1$. Since $p_j^2/(p_j-1)\leq2p_j$, part (ii), followed by a $p_j$-th root, gives the [Moser iteration](../../../elliptic-boundary-value-problem.md#moser-iteration) step

$$
\|u\|_{L^{p_{j+1}}(\Omega)}\leq\bigl(C(n)\lambda p_j\bigr)^{1/p_j}\|u\|_{L^{p_j}(\Omega)}.
$$

After $N$ steps,

$$
\|u\|_{L^{p_N}}\leq(C(n)\lambda)^{S_N}
\exp\left(\sum_{j=0}^{N-1}\frac{\log p_j}{p_j}\right)\|u\|_{L^2},
\qquad S_N=\sum_{j=0}^{N-1}\frac1{p_j}.
$$

The [geometric series](../../../real-analysis.md#geometric-series) and its differentiated form give

$$
\sum_{j=0}^\infty\frac1{p_j}=\frac{\kappa}{2(\kappa-1)}=\frac n4,
\qquad
\sum_{j=0}^\infty\frac j{\kappa^j}=\frac{\kappa}{(\kappa-1)^2}.
$$

In particular the exact convergent product is

$$
\prod_{j=0}^\infty(2\kappa^j)^{1/(2\kappa^j)}
=2^{\kappa/(2(\kappa-1))}\kappa^{\kappa/(2(\kappa-1)^2)}<\infty.
$$

The printed hint's equality to a single power of $2\kappa$ is not correct in general; its claimed finiteness is correct and the displayed expression supplies the correction.

On a finite-measure domain, [Lp norms converge to the supremum norm](../../../measure-theory.md#lp-norms-converge-to-the-supremum-norm) for a bounded continuous function. Indeed, the upper bound is $\|u\|_p\leq|\Omega|^{1/p}\|u\|_\infty$; for every $a<\|u\|_\infty$, the set $\{|u|>a\}$ has positive measure, giving $\|u\|_p\geq a|\{|u|>a\}|^{1/p}$. Let $N\to\infty$ in the iteration and use part (i), which gives $\lambda>0$. The [Dirichlet eigenfunction supremum estimate](../../../partial-differential-equation.md#dirichlet-eigenfunction-supremum-estimate) is

$$
\boxed{\sup_\Omega|u|\leq C(n)\lambda^{n/4}\|u\|_{L^2(\Omega)}.}
$$

**The eigenvalue exponent is exactly $n/4$.** The constant depends only on $n$: the supplied zero-boundary [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) has a dimension-only constant, and every product factor above depends only on $\kappa$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
