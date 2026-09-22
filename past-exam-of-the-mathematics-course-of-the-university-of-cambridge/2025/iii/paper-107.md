# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20107.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [harmonic function](../../../partial-differential-equation.md#harmonic-function) $u$, let

$$
M(r)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}u.
$$

The [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
M'(r)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}\partial_\nu u
=\frac1{|\partial B_r|}\int_{B_r(x)}\Delta u=0.
$$

Since $M(r)\to u(x)$ as $r\downarrow0$, $M(r)=u(x)$. Integrating the spherical averages in the radial variable gives the corresponding ball average, proving the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions). If $u$ attains its maximum at an interior point, the average of the nonnegative function $\max u-u$ on every sufficiently small centred sphere is zero. [Continuity](../../../calculus.md#continuous-function) makes $u$ constant on those spheres, and [connectedness](../../../geometry-and-topology.md#connected-space) propagates that value through the domain. Thus the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) gives

$$
\min_{\partial\Omega}u\leq u\leq\max_{\partial\Omega}u.
$$

For the derivative estimate, choose $r>0$ smaller than half the [distance](../../../topological-analysis.md#distance-to-a-set) from $\Omega'$ to $\partial\Omega$, and let $\rho_r$ be a smooth radial [mollifier](../../../distribution-theory.md#mollifier) supported in $B_r(0)$. Writing its convolution in polar coordinates and using the spherical mean value property shows that $u*\rho_r=u$ on $\Omega'$. Hence, for every [multi-index](../../../distribution-theory.md#multi-index-notation) $\alpha$,

$$
D^\alpha u(x)=\int_\Omega D^\alpha\rho_r(x-y)u(y)\,dy,
$$

so [Holder inequality](../../../functional-analysis.md#holder-inequality) gives

$$
\boxed{\|D^\alpha u\|_{L^\infty(\Omega')}
\leq\|D^\alpha\rho_r\|_\infty\|u\|_{L^1(\Omega)}
\leq C(n,\alpha,\Omega,\Omega')\|u\|_{L^1(\Omega)}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Suppose $u_1$ and $u_2$ are [weak solutions](../../../partial-differential-equation.md#weak-solution) with the same [trace](../../../sobolev-space.md#sobolev-trace-theorem), and put $w=u_1-u_2\in H_0^1(\Omega)$. The [weak formulation](../../../partial-differential-equation.md#weak-formulation) permits $w$ itself as a [test function](../../../distribution-theory.md#test-function), giving

$$
0=\int_\Omega Dw\mathbin\cdot Dw=\int_\Omega|Dw|^2.
$$

Thus $w$ is [almost everywhere](../../../measure-theory.md#almost-everywhere) constant, and its zero trace makes that constant zero. This proves uniqueness.

The weak identity also says that $\Delta u=0$ in the sense of [distributions](../../../distribution-theory.md). The [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma) therefore gives $u\in C^\infty(\Omega)$ and $\Delta u=0$ pointwise. The assumed [continuity](../../../calculus.md#continuous-function) on $\overline\Omega$ retains the prescribed boundary values, so the weak solution is the unique classical solution in $C^\infty(\Omega)\cap C^0(\overline\Omega)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix a closed ball $\overline{B_R(a)}\subset\Omega$, and let $v$ solve the [Dirichlet problem](../../../analysis.md#dirichlet-problem) for the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) in this ball with boundary data $u$. Put $w=u-v$. The function $w$ is continuous, vanishes on the boundary, and inherits the restricted spherical mean identity because $v$ has the full [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions).

Suppose $M=\max_{\overline{B_R(a)}}w>0$. Its maximum set $E$ is a nonempty compact subset of the open ball. Choose $x\in E$ maximizing $|x-a|$. For every sufficiently small radius in the sequence attached to $x$,

$$
M=w(x)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}w\leq M.
$$

Equality of the average with the maximum and [continuity](../../../calculus.md#continuous-function) imply that the whole sphere belongs to $E$. Its point in the direction from $a$ through $x$ lies farther from $a$ than $x$ does; if $x=a$, any point on the sphere does. Both cases contradict the choice of $x$. Hence $w\leq0$, and applying the same argument to $-w$ gives $w=0$.

**Thus $u=v$ on every relatively compact ball. It is consequently harmonic and smooth locally, proving the [local converse to the mean value property](../../../partial-differential-equation.md#local-converse-to-the-mean-value-property).**

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write the flux as

$$
A^i(x,z,\eta)=a^{ij}(x,z,\eta)\eta_j.
$$

After expanding the [divergence](../../../calculus.md#divergence), the [principal symbol of a partial differential equation](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) along a candidate solution $u$ is determined by

$$
A^{ik}(x,u,Du)=\frac{\partial A^i}{\partial\eta_k}
=a^{ik}+\frac{\partial a^{ij}}{\partial\eta_k}D_ju.
$$

Only the symmetric part $A_s=(A+A^T)/2$ contributes to $A^{ik}D_{ik}u$. The problem is elliptic along $u$ when $\xi^TA_s\xi\geq0$ for every $\xi$, and it is strictly elliptic where this quantity is positive for every nonzero $\xi$. It is uniformly elliptic on a set when constants $0<\lambda\leq\Lambda<\infty$, independent of the point, satisfy

$$
\lambda|\xi|^2\leq\xi^TA_s(x,u,Du)\xi\leq\Lambda|\xi|^2.
$$

These definitions separate pointwise positive definiteness from a quantitative lower and upper bound; a [degenerate elliptic operator](../../../elliptic-boundary-value-problem.md#degenerate-elliptic-operator) may lose strict ellipticity at some jets.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the [p-energy](../../../calculus-of-variations.md#p-energy)

$$
F[u]=\frac1p\int_\Omega|Du|^p\,dx,
$$

the [first variation](../../../calculus-of-variations.md#first-variation) in the direction $\psi\in C_c^\infty(\Omega)$ is

$$
\left.\frac d{dt}F[u+t\psi]\right|_{t=0}
=\int_\Omega|Du|^{p-2}Du\mathbin\cdot D\psi.
$$

An [integration by parts](../../../calculus.md#integration-by-parts) therefore gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\operatorname{div}(|Du|^{p-2}Du)=0,
$$

which is the [p-Laplacian equation](../../../partial-differential-equation.md#p-laplacian). In the notation of the question one takes $a^{ij}(x,z,\eta)=|\eta|^{p-2}\delta^{ij}$.

For $\eta\ne0$, the principal coefficient matrix is

$$
A^{ik}(\eta)=|\eta|^{p-2}\delta^{ik}
+(p-2)|\eta|^{p-4}\eta_i\eta_k.
$$

Its eigenvalue in directions orthogonal to $\eta$ is $|\eta|^{p-2}$, while its eigenvalue parallel to $\eta$ is $(p-1)|\eta|^{p-2}$. The coefficients are $C^{1,\alpha}$ away from $\eta=0$, and the [condition number](../../../linear-algebra.md#condition-number) there is at most $p-1$. On every region where $0<m\leq|Du|\leq M$, this gives uniform ellipticity with constants depending on $m$, $M$, and $p$. At $Du=0$ all principal eigenvalues vanish, so the operator is degenerate there and is not strictly elliptic on a domain containing a critical point.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The boundary data are encoded by the [Affine Sobolev space](../../../sobolev-space.md#affine-sobolev-space)

$$
\mathcal A_\varphi=\varphi+W_0^{1,p}(\Omega)
=\{u\in W^{1,p}(\Omega):\operatorname{Tr}u=\operatorname{Tr}\varphi\}.
$$

A function $u\in\mathcal A_\varphi$ is a weak solution of the homogeneous [p-Laplacian equation](../../../partial-differential-equation.md#p-laplacian) when

$$
\int_\Omega|Du|^{p-2}Du\mathbin\cdot D\psi=0
\qquad\text{for every }\psi\in W_0^{1,p}(\Omega).
$$

For existence, take a minimizing sequence for the [p-energy](../../../calculus-of-variations.md#p-energy) on $\mathcal A_\varphi$. The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) bounds $u-\varphi$ in $W^{1,p}$ by its gradient, so the sequence is bounded in the [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space) $W^{1,p}$. A weakly convergent subsequence remains in the weakly closed affine space, and convexity of $|\eta|^p$ gives [weak lower semicontinuity](../../../functional-analysis.md#weak-lower-semicontinuity). The [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) therefore produces a minimizer, whose first variation is precisely the displayed weak equation.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Seek a [radial function](../../../partial-differential-equation.md#radial-function) $u=u(r)$ on the unit ball. The equation and regularity at the origin give

$$
\left(r^{n-1}|u'|^{p-2}u'\right)'=r^{n-1},
\qquad
r^{n-1}|u'|^{p-2}u'=\frac{r^n}{n}.
$$

Hence $u'(r)=(r/n)^{1/(p-1)}$, and the zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) gives

$$
u(r)=\frac{p-1}{p}n^{-1/(p-1)}
\left(r^{p/(p-1)}-1\right).
$$

The power $|x|^q$ is twice differentiable at the origin exactly when $q\geq2$. Here $q=p/(p-1)$, so $u\in C^2$ at the origin exactly when $1<p\leq2$. Under the assumption $2<p<n$, this weak solution is never $C^2$ at the origin, exhibiting the regularity loss caused by [degenerate ellipticity](../../../elliptic-boundary-value-problem.md#degenerate-elliptic-operator).

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For

$$
Lu=a^{ij}D_{ij}u+b^iD_iu+cu,
\qquad c\leq0,
$$

the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) states that $Lu\geq0$ implies

$$
\max_{\overline\Omega}u\leq\max\{0,\max_{\partial\Omega}u\}.
$$

In particular, a solution of $Lu=0$ cannot have a positive interior maximum exceeding its boundary maximum.

Because the coefficient matrix is positive definite and the closure of the smooth bounded domain is compact, strict ellipticity supplies a uniform lower bound after restricting to $\overline\Omega$. Rotate and translate coordinates so that $\Omega$ is bounded in the $x_1$ direction, and set $h=e^{\gamma x_1}$. For sufficiently large $\gamma$,

$$
Lh=e^{\gamma x_1}(\gamma^2a^{11}+\gamma b^1+c)>0.
$$

If $u+\varepsilon h$ had a positive interior maximum, its gradient would vanish and its [Hessian matrix](../../../calculus.md#hessian-matrix) would be negative semidefinite there, giving $L(u+\varepsilon h)\leq0$. This contradicts $L(u+\varepsilon h)=\varepsilon Lh>0$. Comparing on the boundary and sending $\varepsilon\downarrow0$ proves the assertion.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) is

$$
\|u\|_{C^{2,\alpha}(\overline\Omega)}
\leq C\left(
\|u\|_{C^0(\overline\Omega)}
+\|f\|_{C^{0,\alpha}(\overline\Omega)}
+\|\varphi\|_{C^{2,\alpha}(\overline\Omega)}
\right).
$$

The constant depends on the dimension, $\alpha$, the domain and its boundary regularity, the ellipticity constants, and the $C^{0,\alpha}$ norms of the coefficients, but not on $u$, $f$, or $\varphi$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Fix $v\in C^{1,\beta}(\overline\Omega)$. Its jet map $x\mapsto(x,v(x),Dv(x))$ is $C^{0,\beta}$, while the barred coefficients are $C^{0,\alpha}$ in all their variables. Composition therefore makes

$$
x\longmapsto\bar a^{ij}(x,v,Dv),\qquad
x\longmapsto\bar b(x,v,Dv)
$$

$C^{0,\alpha\beta}$. The image of the jet map is compact, so strict ellipticity on the coefficient domain has a positive uniform lower bound on this image. The assumed linear [Dirichlet problem](../../../analysis.md#dirichlet-problem) theory now gives a unique

$$
u=T(v)\in C^{2,\alpha\beta}(\overline\Omega)
$$

solving $\bar a^{ij}(x,v,Dv)D_{ij}u+\bar b(x,v,Dv)=0$ with boundary value $\varphi$. Thus $T:C^{1,\beta}\to C^{1,\beta}$ is well defined.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $v$ range over a bounded subset of $C^{1,\beta}$. All jets $(x,v,Dv)$ then lie in one compact set, so the composed coefficients have uniform $C^{0,\alpha\beta}$ bounds and one ellipticity constant. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) bounds $T(v)$ in $C^0$ by the boundary data and the bounded forcing term. The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) consequently bounds $T(v)$ in $C^{2,\alpha\beta}$.

The [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces)

$$
C^{2,\alpha\beta}(\overline\Omega)Subset C^{1,\beta}(\overline\Omega)
$$

then makes the image relatively compact. Hence $T$ is a compact operator on $C^{1,\beta}(\overline\Omega)$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Suppose $v_k\to v$ in $C^{1,\beta}$ and write $u_k=T(v_k)$. The preceding uniform [Schauder estimate](../../../elliptic-boundary-value-problem.md#schauder-estimates) bounds $(u_k)$ in $C^{2,\alpha\beta}$. Every subsequence therefore has a further subsequence converging in $C^{1,\beta}$ by the [compact embedding of Hölder spaces](../../../sobolev-space.md#compact-embedding-of-holder-spaces). The composed coefficients converge uniformly, and lower-exponent Hölder compactness provides enough convergence of the second derivatives to pass to the linear equation. Every subsequential limit solves the problem defining $T(v)$.

Uniqueness of that linear [Dirichlet problem](../../../analysis.md#dirichlet-problem) forces every such limit to equal $T(v)$. Since every subsequence has a further subsequence with this same limit, the whole sequence converges to $T(v)$ in $C^{1,\beta}$. Thus $T$ is continuous.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

The [Leray-Schauder fixed point theorem](../../../analysis.md#leray-schauder-fixed-point-theorem) says that a continuous compact map $T$ on a [Banach space](../../../banach-space.md) has a fixed point if the homotopy set

$$
\{u:u=tT(u)\text{ for some }0\leq t\leq1\}
$$

is bounded. If $u=tT(u)$ with $t>0$, multiplying the equation for $T(u)$ by $t$ shows that $u$ solves

$$
\bar a^{ij}(x,u,Du)D_{ij}u+t\bar b(x,u,Du)=0
\quad\text{in }\Omega,
\qquad u=t\varphi\quad\text{on }\partial\Omega.
$$

The case $t=0$ gives $u=0$. Therefore it is enough to prove one uniform $C^{1,\beta}$ estimate for all solutions of this family and all $t\in[0,1]$. The theorem then yields a fixed point $u=T(u)$, which solves the original quasilinear problem.

Initially the construction gives $u\in C^{2,\alpha\beta}$. This makes $u$ and $Du$ Lipschitz, so composing the original $C^{0,\alpha}$ coefficients with the jet of $u$ produces $C^{0,\alpha}$ coefficients. A second application of the [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) gives $u\in C^{2,\alpha}(\overline\Omega)$. The fixed-point theorem is an existence result and supplies no uniqueness.

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Hölder interpolation inequality](../../../sobolev-space.md#holder-interpolation-inequality) says that for $u\in C^{l,\alpha}(B_R(x_0))$ and every $\varepsilon>0$,

$$
R^l\|D^lu\|_{C^0(B_R)}
\leq\varepsilon R^{l+\alpha}[D^lu]_{C^{0,\alpha}(B_R)}
+C(n,l,\alpha,\varepsilon)\|u\|_{C^0(B_R)}.
$$

More generally, each lower derivative norm can be bounded by an arbitrarily small multiple of the top $C^{l,\alpha}$ seminorm plus a constant multiple of the $C^0$ norm. The powers of $R$ make the inequality invariant under [scaling](../../../partial-differential-equation.md#scaling-symmetry-of-a-partial-differential-equation) of the ball.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For every $\Omega'\Subset\Omega$, the [interior Schauder estimate](../../../elliptic-boundary-value-problem.md#interior-schauder-estimate) is

$$
\|u\|_{C^{2,\alpha}(\overline{\Omega'})}
\leq C\left(
\|u\|_{C^0(\overline\Omega)}
+\|f\|_{C^{0,\alpha}(\overline\Omega)}
\right).
$$

The constant depends on $n$, $\alpha$, the ellipticity constants, the coefficient $C^{0,\alpha}$ norms, $\Omega$, $\Omega'$, and in particular the distance from $\Omega'$ to the boundary. It is independent of $u$ and $f$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

For $y$ in the closed upper half-space, write $B_r^+(y)=B_r(y)\cap\overline{\mathbb R_+^n}$. The boundary [Simon absorption lemma](../../../elliptic-boundary-value-problem.md#simon-absorption-lemma) has the following scaled form. Let $S$ be a nonnegative set functional that is monotone and subadditive on finite covers by such half-balls. Given $\lambda\geq0$ and $0<\theta<1$, there is $\delta_0=\delta_0(n,\lambda,\theta)>0$ such that, if $0<\delta\leq\delta_0$ and every admissible nested pair satisfies

$$
(\theta r)^\lambda S(B_{\theta r}^+(y))
\leq\delta r^\lambda S(B_r^+(y))+\gamma,
$$

then

$$
R^\lambda S(B_R^+(x))\leq C(n,\lambda,\theta)\gamma.
$$

The same conclusion holds for half-balls centred on the flat boundary and truncated balls meeting it. Iteration over a finite covering absorbs the small first term into the left-hand side.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

The [boundary Schauder estimate](../../../elliptic-boundary-value-problem.md#boundary-schauder-estimate) is

$$
\|u\|_{C^{2,\alpha}(\overline{B_{1/2}^+})}
\leq C\left(
\|u\|_{C^0(\overline{B_1^+})}
+\|f\|_{C^{0,\alpha}(\overline{B_1^+})}
+\|\varphi\|_{C^{2,\alpha}(\overline{B_1^+})}
\right),
$$

where $C$ depends only on the dimension, $\alpha$, the ellipticity constants, and the coefficient Hölder norms.

Subtract a $C^{2,\alpha}$ extension of $\varphi$ to reduce to a function $v$ with zero data on the flat boundary; this changes the forcing by a controlled $C^{0,\alpha}$ term. The key local estimate is that for every $\delta>0$,

$$
[D^2v]_{\alpha;B_{1/2}^+}
\leq\delta[D^2v]_{\alpha;B_1^+}
+C_\delta\left(\|v\|_{C^2(B_1^+)}+\|Lv\|_{C^{0,\alpha}(B_1^+)}\right).
$$

To prove it, argue by contradiction. A failing normalized sequence has points $x_k,y_k$ at which the second-derivative Hölder quotient stays nonzero. Set $r_k=|x_k-y_k|$, subtract the appropriate second-order [Taylor polynomial](../../../calculus.md#taylor-polynomial), and rescale space by $r_k$ and the functions by $r_k^{2+\alpha}[D^2v_k]_\alpha$. Necessarily $r_k\to0$.

If the rescaled distance to the flat boundary tends to infinity, the domains converge to all of $\mathbb R^n$; otherwise they converge to a half-space. Coefficient compactness freezes the principal matrix, while the normalized right-hand sides converge locally uniformly to zero. A linear change of variables turns every limiting equation into the [Laplace equation](../../../partial-differential-equation.md#laplace-equation). In the whole-space case the [polynomial-growth Liouville theorem for harmonic functions](../../../partial-differential-equation.md#polynomial-growth-liouville-theorem-for-harmonic-functions) makes the limit a polynomial of degree at most two. In the half-space case the zero boundary data permit [odd reflection](../../../sobolev-space.md#odd-reflection) across the flat boundary, after which the same theorem applies. The subtracted Taylor normalization forces that polynomial to vanish to second order, contradicting the nonzero limiting Hölder oscillation.

Apply the local estimate on all interior balls and boundary half-balls. The interior and boundary forms of the [Simon absorption lemma](../../../elliptic-boundary-value-problem.md#simon-absorption-lemma) absorb the term multiplied by $\delta$, while the [Hölder interpolation inequality](../../../sobolev-space.md#holder-interpolation-inequality) absorbs the remaining lower $C^2$ norm into the top seminorm and the $C^0$ norm. Restoring $\varphi$ yields the displayed estimate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
