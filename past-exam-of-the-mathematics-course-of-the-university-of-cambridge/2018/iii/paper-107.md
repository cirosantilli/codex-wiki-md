# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_107.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the spherical average $M(r)$, rescaling the sphere and applying the [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
M(r)=\frac1{n\omega_n}\int_{S^{n-1}}u(y+r\theta)\,dS_\theta,\qquad
M'(r)=\frac1{n\omega_n r^{n-1}}\int_{\partial B_r(y)}\partial_\nu u
=\frac1{n\omega_n r^{n-1}}\int_{B_r(y)}\Delta u=0.
$$

By [continuity](../../../calculus.md#continuous-function), $M(r)\to u(y)$ as $r\downarrow0$. Integrating these spherical averages in radius proves the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions):

$$
\boxed{u(y)=\frac1{n\omega_n r^{n-1}}\int_{\partial B_r(y)}u
=\frac1{\omega_n r^n}\int_{B_r(y)}u.}
$$

For the [strong maximum principle for harmonic functions](../../../partial-differential-equation.md#strong-maximum-principle-for-harmonic-functions), suppose an interior point attains the maximum $m$ on a connected domain. The continuous nonnegative function $m-u$ has zero average on each sufficiently small ball around that point, so it vanishes there. The maximum set is therefore open as well as closed, and [connectedness](../../../geometry-and-topology.md#connected-space) makes it the entire domain. Apply the same argument to $-u$ for a minimum.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $x,z\in B_\rho(y)$, the [open balls](../../../topology.md#open-ball) satisfy $B_\rho(x)\subset B_{3\rho}(z)\subset B_{4\rho}(y)$. Nonnegativity and the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) give

$$
u(x)=\frac1{\omega_n\rho^n}\int_{B_\rho(x)}u
\leq\frac1{\omega_n\rho^n}\int_{B_{3\rho}(z)}u=3^nu(z).
$$

Taking the supremum over $x$ and the infimum over $z$ proves the [Harnack inequality for harmonic functions](../../../partial-differential-equation.md#harnack-inequality-for-harmonic-functions):

$$
\boxed{\sup_{B_\rho(y)}u\leq3^n\inf_{B_\rho(y)}u.}
$$

This includes a zero infimum, which forces $u=0$ on the smaller ball.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Shift $u$ by a constant and, if necessary, change sign to obtain an entire nonnegative [harmonic function](../../../partial-differential-equation.md#harmonic-function) $v$. The [Harnack inequality for harmonic functions](../../../partial-differential-equation.md#harnack-inequality-for-harmonic-functions) on arbitrarily large balls centred at $x_0$ gives $v(x)\leq3^nv(x_0)$ for every $x$. Thus $v$ is globally bounded. The [interior derivative estimate for a harmonic function](../../../partial-differential-equation.md#interior-derivative-estimate-for-a-harmonic-function) now gives $|Dv(x)|\leq C\|v\|_\infty/R$ on balls of arbitrarily large radius $R$. Letting $R\to\infty$ proves $Dv=0$, hence $u$ is constant. This proves the one-sided [harmonic Liouville theorem](../../../partial-differential-equation.md#harmonic-liouville-theorem) in every dimension.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**The conclusion holds in dimension two.** Shift and change sign to obtain a nonnegative [harmonic function](../../../partial-differential-equation.md#harmonic-function) $v$. Its circular mean satisfies

$$
m(r)=\frac1{2\pi}\int_0^{2\pi}v(r\cos\theta,r\sin\theta)\,d\theta,\qquad
m''+r^{-1}m'=0.
$$

Here the angular second derivative in the polar-coordinate [Laplacian](../../../calculus.md#laplacian) integrates to zero. Thus $m(r)=a\log r+b$; nonnegativity for every $r>0$ forces $a=0$. For $|x|=r$, the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) and nonnegativity give

$$
v(x)\leq\frac4{\pi r^2}\int_{r/2<|z|<3r/2}v(z)\,dz=8b.
$$

The [removable singularity for a bounded harmonic function](../../../partial-differential-equation.md#removable-singularity-for-a-bounded-harmonic-function) fills in the origin, and the [harmonic Liouville theorem](../../../partial-differential-equation.md#harmonic-liouville-theorem) makes the extension constant.

**The conclusion fails for $n\geq3$:** $\boxed{u(x)=|x|^{2-n}}$ is positive and nonconstant, and its radial [Laplacian](../../../calculus.md#laplacian) $u''+(n-1)u'/r$ vanishes away from zero. For $n=1$, $\boxed{u(x)=|x|}$ is a nonconstant function bounded below whose second derivative vanishes on both components of the punctured line.

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume uniform ellipticity $a^{ij}\xi_i\xi_j\geq\lambda|\xi|^2$ with $\lambda>0$, bounded coefficients, and $c\leq0$. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) is

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}.}
$$

When $c=0$, zero can be omitted. The sign restriction is necessary, as shown by the [failure of the weak maximum principle with a positive zeroth-order coefficient](../../../elliptic-boundary-value-problem.md#failure-of-the-weak-maximum-principle-with-a-positive-zeroth-order-coefficient).

Let $M=\max(0,\sup_{\partial\Omega}u)$ and $w=u-M$, so $Lw=Lu-cM\geq0$ and $w\leq0$ on the boundary. For sufficiently large $k$, $q=e^{kx_1}$ satisfies

$$
Lq=q(k^2a^{11}+kb^1+c)>0.
$$

If $w$ is positive somewhere, $w+\varepsilon q$ retains a positive interior maximum above all its boundary values for small $\varepsilon>0$. At that point its [gradient](../../../calculus.md#gradient) is zero and its [Hessian matrix](../../../calculus.md#hessian-matrix) is negative semidefinite; ellipticity and $c\leq0$ give $L(w+\varepsilon q)\leq0$, contradicting its strict positivity. This [exponential perturbation proof of the weak maximum principle with drift](../../../elliptic-boundary-value-problem.md#exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift) also works with $M=\sup_{\partial\Omega}u$ of either sign when $c=0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Integration by parts gives the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph) in nondivergence form:

$$
a^{ij}(Du)u_{ij}=0,\qquad
a^{ij}(p)=\delta_{ij}-\frac{p_ip_j}{1+|p|^2}.
$$

Its eigenvalues are between $(1+|p|^2)^{-1}$ and one. On each relatively compact subdomain, $Du$ is bounded, so it is a [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator). Since $u\in C^2$, its coefficient functions are locally Lipschitz. The [interior Schauder estimate](../../../elliptic-boundary-value-problem.md#interior-schauder-estimate) gives $C^{2,\beta}_{\rm loc}$ regularity for every $0<\beta<1$; differentiating and repeatedly applying regularity estimates gives $\boxed{u\in C^\infty(\Omega)}$.

Differentiate in direction $k$. Each $u_k$ satisfies $\mathcal Lu_k=0$, with

$$
\mathcal L=a^{ij}D_{ij}+b^\ell D_\ell,\qquad
b^\ell=\frac{\partial a^{ij}}{\partial p_\ell}(Du)u_{ij}.
$$

For $v=|Du|^2$ this yields

$$
\mathcal Lv=2\sum_k a^{ij}u_{ki}u_{kj}\geq0.
$$

If $u\in C^2(\overline\Omega)$, the principal coefficients are uniformly elliptic globally and the drift is bounded. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) bounds $v$ by its boundary maximum. Boundary values are limits of interior values by [continuity](../../../calculus.md#continuous-function), proving the [gradient maximum principle for a minimal graph](../../../second-fundamental-form.md#gradient-maximum-principle-for-a-minimal-graph):

$$
\boxed{\sup_\Omega|Du|=\sup_{\partial\Omega}|Du|.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The cone condition implies $u(\lambda x)=\lambda u(x)$, so $Du(\lambda x)=Du(x)$. The [gradient](../../../calculus.md#gradient) is homogeneous of degree zero, and $v=|Du|^2$ attains its global maximum on the compact unit sphere. For $n\geq2$ the punctured space is connected. Part (b) gives $\mathcal Lv\geq0$ for a locally [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) with no zeroth-order term. The [strong maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-maximum-principle-for-elliptic-operators) makes $v$ constant. Hence

$$
0=\mathcal Lv=2\sum_k a^{ij}u_{ki}u_{kj}.
$$

Positive definiteness gives $D^2u=0$. Thus $u=a\cdot x+b$, and degree-one homogeneity forces $b=0$: $\boxed{u(x)=a\cdot x}$. This proves that a [minimal graphical cone is a plane](../../../second-fundamental-form.md#minimal-graphical-cone-is-a-plane). Strictly, the graph restricted to $x\ne0$ is the plane with its origin omitted; its closure is the full plane through the origin.

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Assume $c\leq0$, bounded coefficients and uniform ellipticity near the boundary point, an interior tangent ball there, and enough regularity for the boundary normal derivative. The [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma) says that a nonnegative maximum at $x_0$ with strictly smaller values inside the tangent ball satisfies

$$
\boxed{\partial_\nu v(x_0)>0}
$$

for the outward unit normal. If $c=0$, the maximum can have either sign. Without existence of a classical derivative, one states a strict one-sided derivative bound.

The PDF also asks to deduce the [strong maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-maximum-principle-for-elliptic-operators); that request is missing from the TeX transcription. Suppose $v$ attains a nonnegative global maximum $M$ inside a connected domain but is not constant. A ball in $\{v<M\}$ can be chosen relatively compact in the domain and tangent to $\{v=M\}$ at an interior point $z$: use the distance from a nearby point to the closed maximum set. The [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma) on that ball gives a nonzero outward derivative at $z$, contradicting $Dv(z)=0$ at an interior maximum. Therefore $v$ is constant. When $c=0$, the same proof works for a maximum of either sign.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition), the [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) is

$$
\boxed{\|u\|_{C^{2,\alpha}(\overline\Omega)}
\leq C\bigl(\|u\|_{C^0(\overline\Omega)}+\|f\|_{C^{0,\alpha}(\overline\Omega)}\bigr).}
$$

The constant depends on $n,\alpha$, domain regularity, the ellipticity lower bound, and coefficient $C^{0,\alpha}$ norms. No sign restriction on $c$ is needed. Nonzero boundary data contribute the $C^{2,\alpha}$ norm of an extension.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Nonnegativity lets us dispense with a sign restriction on $c$. Set $c_0=\min(c,0)$ and $L_0=a^{ij}D_{ij}+b^iD_i+c_0$. Then

$$
L_0u=f-\max(c,0)u\leq0.
$$

The [strong minimum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators) forces $u$ to vanish identically if it has an interior zero. Otherwise it is strictly positive:

$$
\boxed{u\equiv0\quad\text{or}\quad u>0\text{ in }\Omega.}
$$

Connectedness is part of the usual domain hypothesis; on a disconnected open set this conclusion applies separately to each component.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Take $\Omega'$ nonempty. If the bound failed, normalization would give nonnegative $v_j$ with supremum one, zero boundary values, $\inf_{\Omega'}v_j\to0$, and $\|Lv_j\|_{C^{0,\alpha}}\to0$. The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) bounds them in the [Hölder space](../../../sobolev-space.md#holder-space) $C^{2,\alpha}$. By [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces), a subsequence converges in $C^{2,\beta}$, $0<\beta<\alpha$, to $v\geq0$ with $Lv=0$, zero boundary data and supremum one.

Points approaching the infima have a subsequence converging in $\overline{\Omega'}\subset\Omega$. Uniform convergence gives an interior zero of $v$, and part (c), the [strong minimum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators) after replacing $c$ by $\min(c,0)$, gives $v=0$. This contradicts its supremum one, proving

$$
\boxed{\sup_\Omega u\leq C\bigl(\inf_{\Omega'}u+\|f\|_{C^{0,\alpha}}\bigr).}
$$

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $K(u,f)=\|u\|_{C^2(B_1)}+\|f\|_{C^{0,\alpha}(B_1)}$; the paper's $|u|_{2;B_1}$ denotes a $C^2$ norm, not an $L^2$ norm. We use a [blow-up compactness proof of an interior Schauder estimate](../../../elliptic-boundary-value-problem.md#blow-up-compactness-proof-of-an-interior-schauder-estimate). If the estimate failed for fixed $\delta>0$, normalization would produce

$$
[D^2u_j]_{\alpha;B_{1/2}}=1,\qquad [D^2u_j]_{\alpha;B_1}<\delta^{-1},
\qquad K(u_j,f_j)\to0.
$$

Choose $x_j,y_j\in B_{1/2}$ with $d_j=|y_j-x_j|$ and $|D^2u_j(y_j)-D^2u_j(x_j)|\geq\tfrac12d_j^\alpha$. Since $\|D^2u_j\|_\infty\to0$, necessarily $d_j\to0$. Subtract the quadratic [Taylor polynomial](../../../calculus.md#taylor-polynomial) $P_j$ at $x_j$ and set

$$
w_j(z)=\frac{u_j(x_j+d_jz)-P_j(x_j+d_jz)}{d_j^{2+\alpha}}.
$$

The domains expand to $\mathbb R^n$. At zero, $w_j,Dw_j,D^2w_j$ vanish; the [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) of $D^2w_j$ is at most $\delta^{-1}$. Integration along segments gives uniform $C^{2,\alpha}$ bounds on each fixed ball. Also

$$
\Delta w_j(z)=\frac{f_j(x_j+d_jz)-f_j(x_j)}{d_j^\alpha}\to0
$$

locally uniformly, since $[f_j]_\alpha\to0$. By [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces) and a diagonal subsequence, $w_j$ converges locally in $C^{2,\beta}$ to an entire [harmonic function](../../../partial-differential-equation.md#harmonic-function) $w$, with $[D^2w]_\alpha\leq\delta^{-1}$ and $D^2w(0)=0$. The unit vectors $(y_j-x_j)/d_j$ have a convergent subsequence; its limit $e$ satisfies $|D^2w(e)|\geq1/2$.

Each second derivative of $w$ is an entire [harmonic function](../../../partial-differential-equation.md#harmonic-function) with finite global [Hölder seminorm](../../../sobolev-space.md#holder-seminorm). The supplied [polynomial-growth Liouville theorem for harmonic functions](../../../partial-differential-equation.md#polynomial-growth-liouville-theorem-for-harmonic-functions), at growth exponent $\alpha<1$, makes it constant, and its value at zero makes it zero. This contradicts the nonzero Hessian at $e$, proving the estimate with the small $\delta$ term.

To remove that term, rescale the estimate to all contained balls and apply the [Simon absorption lemma](../../../elliptic-boundary-value-problem.md#simon-absorption-lemma). Explicitly, with $d(x)=1-|x|$ and $d_{xy}=\min(d(x),d(y))$, define

$$
M=\sup_{x\ne y\in B_1}d_{xy}^{2+\alpha}
\frac{|D^2u(x)-D^2u(y)|}{|x-y|^\alpha}.
$$

For $|x-y|<d_{xy}/8$, apply the rescaled estimate on $B_{d(x)/2}(x)$; its larger-ball seminorm is controlled by $M$ because all points there have boundary distance at least $d(x)/2$. For more separated pairs use $2\|D^2u\|_\infty$. The result is $M\leq C_0\delta M+C_\delta K(u,f)$. Choose $C_0\delta<1/2$ and use $d_{xy}\geq1/2$ on $B_{1/2}$ to obtain

$$
\boxed{[D^2u]_{\alpha;B_{1/2}}
\leq C(n,\alpha)\bigl(\|u\|_{C^2(B_1)}+\|f\|_{C^{0,\alpha}(B_1)}\bigr).}
$$

The forcing's [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) cannot be discarded. For integers $k\to\infty$, take

$$
\boxed{u_k(x)=k^{-2}\sin(kx_1),\qquad f_k(x)=-\sin(kx_1).}
$$

Their $C^2$ and forcing supremum norms stay bounded, but the $11$ entry of the [Hessian matrix](../../../calculus.md#hessian-matrix) differs by two at $x_1=\pm\pi/(2k)$, giving $[D^2u_k]_{\alpha;B_{1/2}}\geq2(k/\pi)^\alpha\to\infty$.

## 5

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Interpret strict ellipticity as uniform ellipticity up to the boundary, as required for the global [elliptic boundary value problem](../../../elliptic-boundary-value-problem.md). Mere pointwise positive definiteness in the interior is insufficient: $L=x^2D^2$ on $(0,1)$ has trivial homogeneous Dirichlet kernel but $Lu=1$ has no $C^2$ solution up to $x=0$.

Set $X=\{u\in C^{2,\alpha}(\overline\Omega):u|_{\partial\Omega}=0\}$ and $Y=C^{0,\alpha}(\overline\Omega)$. The [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem) says $L:X\to Y$ is a [Fredholm operator](../../../functional-analysis.md#fredholm-operator) of index zero. Its [null space](../../../linear-algebra.md#kernel-of-a-linear-map) $N$ is finite dimensional, its range is closed, and the range codimension equals $\dim N$. Hence $\boxed{N=\{0\}\iff L:X\to Y\text{ is invertible}}$; in this case every forcing has a unique solution.

Otherwise there are nonzero homogeneous solutions and finitely many compatibility conditions: $Lu=f$ is solvable exactly when $\ell(f)=0$ for every continuous linear functional on $Y$ vanishing on $L(X)$. When solvable, its solutions are $u_0+N$. This [Fredholm solvability condition](../../../analysis.md#fredholm-solvability-condition) can be expressed with formal-adjoint null solutions for smoother coefficients. The functional formulation avoids differentiating the merely $C^{0,\alpha}$ coefficients.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Failure of the bound would give normalized $v_j$ with $\|v_j\|_\infty=1$, zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition), and $\|Lv_j\|_{C^{0,\alpha}}\to0$. The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) bounds them in $C^{2,\alpha}$. By [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces), a subsequence converges in $C^{2,\beta}$ to $v$ with $Lv=0$, zero boundary data and $\|v\|_\infty=1$. The uniform [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) bounds pass to the limit, so $v\in C^{2,\alpha}$. This contradicts the trivial [null space](../../../linear-algebra.md#kernel-of-a-linear-map), proving

$$
\boxed{\|u\|_\infty\leq C_1\|f\|_{C^{0,\alpha}}.}
$$

The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) then gives $\|u\|_{C^{2,\alpha}}\leq K\|f\|_{C^{0,\alpha}}$, the bounded-inverse estimate used next.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem) and part (b) give an inverse $S:Y\to X$ of norm at most $K\geq1$. Choose

$$
\varepsilon=\min\left(1,\frac1{8KC}\right),\qquad
\delta=\min\left(\frac{\varepsilon}{4K},\frac1{4K}\right),\qquad
\varepsilon_0=\frac{\varepsilon}{4K}.
$$

On the closed radius-$\varepsilon$ ball $\mathcal B\subset X$, set $T(v)=S(\mathcal Q(v)+f)$. The stated inequalities give

$$
\|T(v)\|_{C^{2,\alpha}}\leq K(C\varepsilon^2+\delta+\varepsilon_0)
\leq\tfrac58\varepsilon,
$$

and

$$
\|T(v)-T(w)\|_{C^{2,\alpha}}
\leq K(2C\varepsilon+\delta)\|v-w\|_{C^{2,\alpha}}
\leq\tfrac12\|v-w\|_{C^{2,\alpha}}.
$$

Thus $T$ is a [contraction mapping](../../../analysis.md#contraction-mapping) of the complete metric space $\mathcal B$ into itself. The [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) gives $u=T(u)$, solving the required [nonlinear elliptic boundary value problem](../../../elliptic-boundary-value-problem.md#nonlinear-elliptic-boundary-value-problem). This [small-data existence for a nonlinear elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem) also gives uniqueness within this small ball; it does not assert global uniqueness.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Let $u=v+\psi$, so $v$ has zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition). Using the supplied form of the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph), set

$$
Q_\psi(v)=\widetilde Q(v+\psi)-\widetilde Q(\psi),\qquad
f_\psi=\widetilde Q(\psi)-\Delta\psi.
$$

For $\|\psi\|_{C^{2,\alpha}}\leq\beta\leq1$ and $\|v\|,\|w\|\leq1$, the difference bound implies

$$
\|Q_\psi(v)\|_{C^{0,\alpha}}\leq C\|v\|_{C^{2,\alpha}}^2+2C\beta,
$$

and

$$
\|Q_\psi(v)-Q_\psi(w)\|_{C^{0,\alpha}}
\leq\bigl[C(\|v\|_{C^{2,\alpha}}+\|w\|_{C^{2,\alpha}})+2C\beta\bigr]\|v-w\|_{C^{2,\alpha}}.
$$

The shifted arguments stay in the permitted radius-two ball, and $\|f_\psi\|_{C^{0,\alpha}}\leq C\beta^2+C_n\beta$. The [Laplacian](../../../calculus.md#laplacian) with zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) has trivial [null space](../../../linear-algebra.md#kernel-of-a-linear-map) by the [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions). Choose $\beta>0$ small enough that $2C\beta\leq\delta$ and $C\beta^2+C_n\beta\leq\varepsilon_0$, for the constants in part (c) with $L=\Delta$. Its [small-data existence for a nonlinear elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem) supplies $v$, and $\boxed{u=v+\psi}$ solves the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph) with the required boundary values.

## 6

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

**As printed, the hypotheses are insufficient.** They order the barriers only on the boundary; the intended [monotone iteration for a semilinear elliptic equation](../../../elliptic-boundary-value-problem.md#monotone-iteration-for-a-semilinear-elliptic-equation) needs an [ordered subsolution and supersolution](../../../elliptic-boundary-value-problem.md#ordered-subsolution-and-supersolution) throughout the domain. On $B_1$, take a positive first [Dirichlet Laplacian eigenfunction](../../../partial-differential-equation.md#dirichlet-laplacian-eigenfunction) $e_1$ with $-\Delta e_1=\lambda_1e_1$, and set

$$
V(s)=-\lambda_1s,\qquad \psi=0,\qquad \varphi^-=e_1,\qquad \varphi^+=-e_1.
$$

Both barriers satisfy $Q\varphi^\pm=0$ and vanish on the boundary, but $\varphi^->\varphi^+$ inside. No function lies between them. This also disproves the unconditional conclusions in (b) and (d).

With the intended extra hypothesis $\varphi^-\leq\varphi^+$ on $\overline\Omega$, solvability of the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) and the [Schauder estimate](../../../elliptic-boundary-value-problem.md#schauder-estimates) give a unique $u_1\in C^{2,\alpha}$ with forcing $V(\varphi^-)$ and boundary data $\psi$. Smooth $V$ composed with the $C^{0,\alpha}$ barrier has the required forcing regularity. The barrier inequalities give

$$
\Delta(u_1-\varphi^-)=V(\varphi^-)-\Delta\varphi^-\leq0,
\qquad
\Delta(\varphi^+-u_1)\leq V(\varphi^+)-V(\varphi^-)\leq0.
$$

Both differences have nonnegative boundary values. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) applied to their negatives gives $\boxed{\varphi^-\leq u_1\leq\varphi^+}$ under the corrected hypothesis.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Use the interior [ordered subsolution and supersolution](../../../elliptic-boundary-value-problem.md#ordered-subsolution-and-supersolution) correction from part (a). Recursively solve the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) $\Delta u_{k+1}=V(u_k)$ with boundary value $\psi$, starting from $u_0=\varphi^-$. Part (a) gives $u_0\leq u_1\leq\varphi^+$. If $u_{k-1}\leq u_k\leq\varphi^+$, then

$$
\Delta(u_{k+1}-u_k)=V(u_k)-V(u_{k-1})\leq0,\qquad
\Delta(\varphi^+-u_{k+1})\leq V(\varphi^+)-V(u_k)\leq0.
$$

The first difference has zero boundary values, the second nonnegative values. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) applied to their negatives gives $u_k\leq u_{k+1}\leq\varphi^+$. Induction proves the bounded [monotone sequence](../../../real-analysis.md#monotone-sequence)

$$
\boxed{\varphi^-\leq u_1\leq u_2\leq\cdots\leq\varphi^+.}
$$

Without interior ordering, the counterexample in part (a) disproves the claim.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For a sequence trapped between the fixed barriers, let $M$ bound their absolute values and put $A=\sup_{|s|\leq M}|V'(s)|$. The [mean value theorem](../../../calculus.md#mean-value-theorem) gives

$$
\|V(u_{k-1})\|_{C^{0,\alpha}}\leq C_0+A\|u_{k-1}\|_{C^{0,\alpha}}.
$$

The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate), including the fixed boundary data $\psi$, and $\|u_k\|_\infty\leq M$ imply

$$
\|u_k\|_{C^{2,\alpha}}\leq KA\|u_{k-1}\|_{C^{0,\alpha}}+C_1.
$$

Apply the supplied [Hölder interpolation inequality](../../../sobolev-space.md#holder-interpolation-inequality) with $KA\varepsilon\leq1/2$. Its remaining supremum-norm term is bounded by $M$, yielding

$$
\boxed{\|u_k\|_{C^{2,\alpha}}\leq\tfrac12\|u_{k-1}\|_{C^{2,\alpha}}+C.}
$$

If $A=0$, the stronger bound without a previous-iterate term holds directly. The constant depends on the fixed domain, exponent, barriers, boundary data and $V$, independently of $k$.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

With the interior ordering correction in part (a), iteration of part (c) gives

$$
\|u_k\|_{C^{2,\alpha}}\leq2^{-(k-1)}\|u_1\|_{C^{2,\alpha}}+2C.
$$

The bounded [monotone sequence](../../../real-analysis.md#monotone-sequence) has a pointwise limit $u$. By [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces), a subsequence converges in $C^{2,\beta}$ for $0<\beta<\alpha$, necessarily to this same limit. All convergent subsequences have that limit, so compactness gives convergence of the full sequence in $C^{2,\beta}$. Passing to the limit in $\Delta u_k=V(u_{k-1})$ gives the equation and boundary values. The uniform [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) bounds on second derivatives pass to the limit, so $u\in C^{2,\alpha}(\overline\Omega)$, and the barriers remain ordered:

$$
\boxed{Qu=0,\qquad u|_{\partial\Omega}=\psi,\qquad \varphi^-\leq u\leq\varphi^+.}
$$

This proves the intended [monotone iteration for a semilinear elliptic equation](../../../elliptic-boundary-value-problem.md#monotone-iteration-for-a-semilinear-elliptic-equation). With only the boundary ordering printed in the PDF, the counterexample in part (a) shows the requested trapped solution need not exist.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
