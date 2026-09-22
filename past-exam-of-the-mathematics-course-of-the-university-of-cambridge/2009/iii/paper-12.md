# Paper 12

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper12.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper12.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
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
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
  - [iv](#6/iv)
    - [Solution](#6/iv/solution)

## 1

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Take a [compactly supported](../../../function.md#compact-support) smooth variation $\varphi\in C_c^\infty(\Omega)$ and set $u_t=u+t\varphi$. Its support is away from the boundary, so it preserves any prescribed boundary values. Differentiating the [functional](../../../calculus-of-variations.md#functional) at $t=0$ gives the [first variation](../../../calculus-of-variations.md#first-variation)

$$
0=\left.\frac{d}{dt}\mathcal F(u_t)\right|_{t=0}=\int_\Omega\left[F_z(x,u,Du)\varphi+F_{p_i}(x,u,Du)D_i\varphi\right]dx.
$$

By [integration by parts](../../../calculus.md#integration-by-parts), there is no boundary term. The [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\boxed{D_i\bigl(F_{p_i}(x,u,Du)\bigr)=F_z(x,u,Du)\quad\text{in }\Omega.}
$$

Expanding the total derivative, an equivalent classical form is

$$
\boxed{F_{p_ip_j}(x,u,Du)D_{ij}u+F_{p_i z}(x,u,Du)D_i u+F_{p_i x_i}(x,u,Du)-F_z(x,u,Du)=0.}
$$

Repeated indices are summed. In the last term involving $x_i$, the derivative holds $z,p$ fixed; the other terms account for their dependence on $u(x),Du(x)$. [Compactly supported](../../../function.md#compact-support) variations derive the interior equation without imposing a natural boundary condition.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) gives the clipped boundary bounds

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\},\qquad\inf_\Omega u\geq\min\{0,\inf_{\partial\Omega}u\}.}
$$

If $c=0$, constants solve the equation, and applying these bounds after subtracting the boundary maximum or minimum gives the sharper conclusion that both extrema occur on the boundary. For $c<0$, the clipping by zero is necessary in the general statement.

To prove the upper bound, write $B=\|b_1\|_\infty$ and $C_0=\|c\|_\infty$, and choose $\alpha>0$ large enough that $\lambda\alpha^2-B\alpha-C_0>0$. For $\phi(x)=e^{\alpha x_1}$, [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) gives

$$
L\phi=\phi(a_{11}\alpha^2+b_1\alpha+c)\geq\phi(\lambda\alpha^2-B\alpha-C_0)>0.
$$

Put $u_\varepsilon=u+\varepsilon\phi$. Then $Lu_\varepsilon>0$. If $u_\varepsilon$ had a positive maximum at an interior point, its [gradient](../../../calculus.md#gradient) would vanish there and its [Hessian matrix](../../../calculus.md#hessian-matrix) would be [negative semidefinite](../../../calculus.md#negative-semidefinite-matrix). Only the symmetric part of $a_{ij}$ contracts with this [Hessian](../../../calculus.md#hessian-matrix), and its positive definiteness implies $a_{ij}D_{ij}u_\varepsilon\leq0$. Also $cu_\varepsilon\leq0$. These facts would give $Lu_\varepsilon\leq0$, a contradiction.

Since $\overline\Omega$ is compact and $u_\varepsilon$ is continuous on it, its maximum exists. It is therefore either nonpositive or attained on the boundary, proving $\sup_\Omega u_\varepsilon\leq\max\{0,\sup_{\partial\Omega}u_\varepsilon\}$. The exponential is bounded on the bounded domain; letting $\varepsilon\downarrow0$ proves the upper estimate. Apply the same argument to $-u$ for the lower estimate. This is the [exponential perturbation proof of the weak maximum principle with drift](../../../elliptic-boundary-value-problem.md#exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift) and requires no continuity of the coefficient functions.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

On the bounded interval $\Omega=(0,\pi)$, take $L=d^2/dx^2+1$ and $u(x)=\sin x$. Its principal coefficient is $1$, so the operator is [uniformly elliptic](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator), and

$$
Lu=-\sin x+\sin x=0,\qquad u(0)=u(\pi)=0,\qquad u(\pi/2)=1.
$$

Thus

$$
\boxed{\sup_\Omega u=1>0=\max\{0,\sup_{\partial\Omega}u\}.}
$$

The positive zeroth-order coefficient $c=1$ permits a zero-boundary [eigenfunction](../../../linear-operator-theory.md#eigenfunction), demonstrating [failure of the weak maximum principle with a positive zeroth-order coefficient](../../../elliptic-boundary-value-problem.md#failure-of-the-weak-maximum-principle-with-a-positive-zeroth-order-coefficient). The function $-\sin x$ similarly violates the lower bound.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Let $u,v$ be two [critical points](../../../analysis.md#critical-point) with the same classical boundary values, and put $w=u-v$. Since $F$ is independent of $z$, the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) for each is $D_iF_{p_i}(x,Du)=0$. By the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) along the segment between the [gradients](../../../calculus.md#gradient),

$$
F_{p_i}(x,Du)-F_{p_i}(x,Dv)=A_{ij}(x)D_jw,\qquad A_{ij}(x)=\int_0^1F_{p_ip_j}(x,Dv+tDw)\,dt.
$$

Subtracting the equations gives $D_i(A_{ij}D_jw)=0$. The [uniformly convex variational integrand](../../../real-analysis.md#uniformly-convex-variational-integrand) makes $A$ symmetric and [uniformly elliptic](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) with the same positive lower bound. Since $F$ is smooth and $u,v\in C^2(\overline\Omega)$, $A$ is continuously differentiable locally in $\Omega$, so

$$
A_{ij}D_{ij}w+(D_iA_{ij})D_jw=0
$$

is a classical [nondivergence-form elliptic operator](../../../elliptic-boundary-value-problem.md#nondivergence-form-elliptic-operator) with no zeroth-order term.

To avoid assuming that derivatives of $F$ stay bounded all the way to the boundary, apply the proved [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) on inner open sets $\Omega_\delta=\{x\in\Omega:\operatorname{dist}(x,\partial\Omega)>\delta\}$. Their closures lie compactly in $\Omega$, so all linearized coefficients there are bounded. The maximum principle applies on each component and yields

$$
\sup_{\Omega_\delta}|w|\leq\sup_{\partial\Omega_\delta}|w|.
$$

Every point of the inner boundary is at distance $\delta$ from $\partial\Omega$. Since $w$ is continuous on the compact closure and equals zero on that boundary, the right-hand side tends uniformly to zero as $\delta\downarrow0$. Every fixed interior point eventually belongs to $\Omega_\delta$, proving

$$
\boxed{u=v\text{ in }\Omega.}
$$

This establishes [uniqueness for uniformly convex gradient Dirichlet problems](../../../real-analysis.md#uniqueness-for-uniformly-convex-gradient-dirichlet-problems) using precisely the boundary continuity and ellipticity needed for the comparison.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

**No: the conclusion need not survive without an additional restriction at infinity.** A counterexample that keeps the [functional](../../../calculus-of-variations.md#functional) finite is $\Omega=\mathbb R^n$ and $F(p)=\tfrac12|p|^2$. The distinct functions $u\equiv0$ and $v\equiv1$ both lie in $C^2(\overline\Omega)$ and have energy zero. Their boundary data agree because $\partial\Omega$ is empty. For any variation with finite [gradient](../../../calculus.md#gradient) energy,

$$
\mathcal F(u+t\varphi)=\mathcal F(v+t\varphi)=\frac{t^2}{2}\int_{\mathbb R^n}|D\varphi|^2,
$$

so both are genuine [critical points](../../../analysis.md#critical-point), not merely formal solutions with infinite [functional](../../../calculus-of-variations.md#functional) value.

With nonempty boundary, the classical [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) also illustrates the missing condition: in dimension $n\geq3$, on $\Omega=\{|x|>1\}$, both $0$ and $1-|x|^{2-n}$ are [harmonic functions](../../../partial-differential-equation.md#harmonic-function) with zero boundary values. The latter has finite [Dirichlet energy](../../../differential-geometry.md#dirichlet-energy), because its gradient-energy integral is proportional to $\int_1^\infty r^{1-n}dr$, and is stationary under [compactly supported](../../../function.md#compact-support) variations. It approaches $1$ at infinity while the zero solution approaches $0$.

This is [nonuniqueness of Dirichlet data without control at infinity](../../../analysis.md#nonuniqueness-of-dirichlet-data-without-control-at-infinity). For a global variational formulation one must specify the admissible variations: the exterior example is not critical against every finite-energy zero-boundary variation, since varying it in its own direction changes its energy to first order. Prescribing an appropriate limit at infinity, or a variational space in which the difference is an admissible zero-boundary [test function](../../../distribution-theory.md#test-function) and constants are excluded, can restore uniqueness.

## 2

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Write $H^1=W^{1,2}$ and $H_0^1=W_0^{1,2}$. The [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) in the [Sobolev space](../../../sobolev-space.md) sense means $u-\psi\in H_0^1(\Omega)$; this definition remains meaningful even without regularity assumptions on the boundary. For bounded full coefficients, a [weak solution](../../../partial-differential-equation.md#weak-solution) is a function satisfying

$$
\boxed{u\in H^1(\Omega),\quad u-\psi\in H_0^1(\Omega),\quad B(u,\varphi)=-\int_\Omega f\varphi\quad\text{for every }\varphi\in H_0^1(\Omega),}
$$

where

$$
B(u,\varphi)=\int_\Omega a_{ij}D_ju\,D_i\varphi-\int_\Omega qu\varphi.
$$

The sign follows by [integration by parts](../../../calculus.md#integration-by-parts) in $D_i(a_{ij}D_ju)+qu=f$. No classical derivatives of the measurable coefficients are taken. Equivalently one may first test against $C_c^\infty(\Omega)$ and extend by density, provided this [bilinear form](../../../linear-algebra.md#bilinear-form) is bounded on $H^1\times H_0^1$. All integrals in this definition must exist: as explained below, the printed quadratic bounds alone do not guarantee this when $A=(a_{ij})$ is nonsymmetric.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

There is a qualification in the printed hypotheses: [quadratic ellipticity does not bound a nonsymmetric coefficient matrix](../../../elliptic-boundary-value-problem.md#quadratic-ellipticity-does-not-bound-a-nonsymmetric-coefficient-matrix). The intended standard existence proof needs $a_{ij}\in L^\infty(\Omega)$, or more generally a bounded principal [bilinear form](../../../linear-algebra.md#bilinear-form). To see why this does not follow from the displayed inequalities, take $\Omega=(-1,1)^2$ and

$$
A(x)=\begin{pmatrix}1&k(x_1)\\-k(x_1)&1\end{pmatrix},\qquad k(t)=\begin{cases}|t|^{-1}&t\ne0,\\0&t=0.\end{cases}
$$

Then $\zeta^TA(x)\zeta=|\zeta|^2$ for every $x,\zeta$. However, choose $u_0,\varphi_0\in C_c^\infty(\Omega)$ equal to $x_2,x_1$, respectively, on a small rectangle about the origin. There $(A Du_0)\cdot D\varphi_0=k(x_1)$, whose positive part has infinite integral. Thus the standard principal pairing is not a finite Lebesgue integral even for these smooth [test functions](../../../distribution-theory.md#test-function). This demonstrates the missing form hypothesis, rather than assuming that all unbounded skew coefficients prevent solvability.

Under the intended bounded-coefficient hypothesis the proof is as follows. On $H=H_0^1(\Omega)$ use the [Hilbert space](../../../hilbert-space.md) [norm](../../../functional-analysis.md#norm) $\|Dw\|_2$, equivalent to the $H^1$ [norm](../../../functional-analysis.md#norm) by the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) on a bounded domain. The form from part (i) is bounded, since

$$
|B(w,v)|\leq\|A\|_{\infty,\mathrm{op}}\|Dw\|_2\|Dv\|_2+\|q\|_\infty\|w\|_2\|v\|_2\leq C\|Dw\|_2\|Dv\|_2.
$$

It is a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form) even without symmetry:

$$
B(w,w)=\int_\Omega a_{ij}D_jwD_iw-\int_\Omega qw^2\geq\lambda\|Dw\|_2^2.
$$

Here the nonpositive sign of $q$ is essential. With $u=\psi+w$, the required equation becomes

$$
B(w,v)=\ell(v),\qquad\ell(v)=-\int_\Omega fv-B(\psi,v).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), bounded coefficients and the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) show that $\ell$ is a bounded [linear functional](../../../linear-algebra.md#linear-functional) on $H$. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) states that a bounded coercive [bilinear form](../../../linear-algebra.md#bilinear-form) on a real Hilbert space represents each bounded [linear functional](../../../linear-algebra.md#linear-functional) in this way with a unique $w\in H$. It therefore yields $u=\psi+w$ with the required boundary condition and weak equation. For completeness, if $u_1,u_2$ are solutions, $z=u_1-u_2\in H_0^1$ satisfies $B(z,z)=0$; [coercivity](../../../real-analysis.md#coercive-function) and the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) imply $z=0$.

**With the missing bounded-form hypothesis, the weak solution exists and is unique.** For nonsymmetric matrices the printed quadratic inequalities omit the hypothesis needed for this standard formulation and proof. No maximum principle is used. In part (iii), symmetry makes the quadratic upper bound a bound on the whole matrix, so no such qualification is needed there.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Symmetry implies that all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A(x)$ lie between $\lambda$ and $\Lambda$, so $\|A(x)\|_{\mathrm{op}}\leq\Lambda$. In particular the [bilinear form](../../../linear-algebra.md#bilinear-form) $B$ from part (i) is bounded and symmetric under the printed assumptions. The [symmetric elliptic Dirichlet energy with a nonpositive potential](../../../calculus-of-variations.md#symmetric-elliptic-dirichlet-energy-with-a-nonpositive-potential) is

$$
\boxed{J(u)=\frac12\int_\Omega\left(a_{ij}D_juD_iu-qu^2\right)+\int_\Omega fu,\qquad u\in\psi+H_0^1(\Omega).}
$$

All its terms are finite. For an admissible variation $\varphi\in H_0^1$, its [first variation](../../../calculus-of-variations.md#first-variation) is $B(u,\varphi)+\int f\varphi$. Thus stationarity is exactly the [weak formulation](../../../partial-differential-equation.md#weak-formulation) of $Lu=f$.

Here is the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations). Put $u=\psi+w$. Expanding the symmetric [quadratic form](../../../linear-algebra.md#quadratic-form) gives

$$
J(\psi+w)=\frac12B(w,w)+B(\psi,w)+\int_\Omega fw+J(\psi)\geq\frac\lambda2\|Dw\|_2^2-C\|Dw\|_2-C.
$$

The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) controls $\|w\|_2$ by $\|Dw\|_2$. Therefore $J$ is bounded below on the admissible class, and a [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) is bounded in $H^1$. By weak compactness in this [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space), a subsequence converges weakly to $u$. The affine closed subspace $\psi+H_0^1$ is weakly closed, so $u$ remains admissible.

The symmetric square root $A^{1/2}(x)$ is measurable and bounded. Since $-q\geq0$, the two bounded linear maps

$$
v\longmapsto A^{1/2}Dv,\qquad v\longmapsto\sqrt{-q}\,v
$$

take weak $H^1$ convergence to weak $L^2$ convergence. The [weak lower semicontinuity of the Hilbert norm](../../../hilbert-space.md#weak-lower-semicontinuity-of-the-hilbert-norm) shows that $B(u,u)$ is weakly lower semicontinuous. The term $\int fu$ is weakly continuous. Hence $J(u)\leq\liminf J(u_k)$ and $u$ attains the minimum. Varying in either sign yields the weak equation.

The sign $q\leq0$ was used both to make the potential energy nonnegative, hence weakly lower semicontinuous by this argument, and to obtain [coercivity](../../../real-analysis.md#coercive-function). Finally $J(u+z)-J(u)=B(z,z)/2\geq\lambda\|Dz\|_2^2/2$ for $z\in H_0^1$, since the first variation at $u$ vanishes. Therefore

$$
\boxed{\text{the minimizer is unique and is the weak solution of }Lu=f.}
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Take $\Omega=(0,\pi)$, $a_{11}=1$, $q=1$, $\psi=0$ and $f(x)=\sin x$. The coefficients are bounded and the operator is [uniformly elliptic](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator). If a [weak solution](../../../partial-differential-equation.md#weak-solution) $u\in H_0^1(0,\pi)$ existed, testing its [weak formulation](../../../partial-differential-equation.md#weak-formulation) with $\varphi=\sin x\in H_0^1(0,\pi)$ would give

$$
\int_0^\pi u'\cos x-\int_0^\pi u\sin x=-\int_0^\pi\sin^2x.
$$

By [integration by parts](../../../calculus.md#integration-by-parts) for $H_0^1$ functions, the first integral on the left is $\int_0^\pi u\sin x$, so the left side is zero. The right side equals $-\pi/2$, a contradiction. Thus

$$
\boxed{u''+u=\sin x,\quad u(0)=u(\pi)=0\text{ has no }H^1\text{ weak solution}.}
$$

The forcing is not orthogonal to the homogeneous zero-boundary [eigenfunction](../../../linear-operator-theory.md#eigenfunction) $\sin x$. This is the obstruction described by the [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem), proved here directly without assuming that theorem.

## 3

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $d=\operatorname{dist}(\Omega',\partial\Omega)>0$. Choose a [smooth cutoff function](../../../analysis.md#smooth-cutoff-function) $\eta\in C_c^\infty(\Omega)$ with $0\leq\eta\leq1$, $\eta=1$ on $\Omega'$ and $|D\eta|\leq C(n)/d$. Such cutoffs can be constructed by mollifying the indicator of a fixed small neighbourhood of $\overline{\Omega'}$. Write $M=\|A\|_{\infty,\mathrm{op}}$, $B=\|b\|_\infty$ and $C_0=\|c\|_\infty$; these are controlled by the individual coefficient bounds and dimension.

The [weak formulation](../../../partial-differential-equation.md#weak-formulation), extended to [compactly supported](../../../function.md#compact-support) $H^1$ tests by density, is

$$
\int_\Omega A Du\cdot D\varphi-\int_\Omega(b\cdot Du+cu)\varphi=-\int_\Omega f\varphi.
$$

We may use $\varphi=\eta^2u$, since $u\in H^1_{\mathrm{loc}}$. Expanding its [gradient](../../../calculus.md#gradient) and using [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) gives

$$
\lambda\int\eta^2|Du|^2\leq2M\int\eta|u||Du||D\eta|+B\int\eta^2|u||Du|+C_0\int\eta^2u^2+\int\eta^2|fu|.
$$

Apply [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) to the first two terms, allocating at most $\lambda/4$ of the [gradient](../../../calculus.md#gradient) integral to each. Bound $|fu|\leq(f^2+u^2)/2$ in the last term. Absorbing those [gradient](../../../calculus.md#gradient) contributions yields the [Caccioppoli inequality with bounded lower-order terms](../../../partial-differential-equation.md#caccioppoli-inequality-with-bounded-lower-order-terms)

$$
\int\eta^2|Du|^2\leq C(n,\lambda,M,B,C_0)\left[\int(1+|D\eta|^2)u^2+\int\eta^2f^2\right].
$$

Consequently $\|Du\|_{L^2(\Omega')}\leq C(\|u\|_{L^2(\Omega)}+\|f\|_{L^2(\Omega)})$. Adding the $L^2$ [norm](../../../functional-analysis.md#norm) of $u$ proves

$$
\boxed{\|u\|_{W^{1,2}(\Omega')}\leq C\left(\|u\|_{L^2(\Omega)}+\|f\|_{L^2(\Omega)}\right),}
$$

where $C$ has precisely the stated dependence on dimension, ellipticity, coefficient bounds and $d$. The proof uses $|c|$, so no sign condition on the zeroth-order term is required.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

First use weak compactness of bounded sets in the [Hilbert space](../../../hilbert-space.md) $L^2(\Omega)$ to pass to a subsequence with $u_k\rightharpoonup u$ globally in $L^2$. The [weak lower semicontinuity of the Hilbert norm](../../../hilbert-space.md#weak-lower-semicontinuity-of-the-hilbert-norm) gives $\|u\|_{L^2(\Omega)}\leq K$. This global step also applies if $\Omega$ is unbounded.

Choose a nested exhaustion $U_j\Subset U_{j+1}\Subset\Omega$ by bounded smooth open sets. Part (i) bounds $u_k$ in $H^1(U_j)$ for every $j$. By the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem), $H^1(U_j)$ embeds compactly in $L^2(U_j)$. Weak compactness in $H^1(U_j)$ and a [diagonal subsequence argument](../../../real-analysis.md#diagonal-subsequence-argument) therefore give, for the same subsequence,

$$
u_k\rightharpoonup u\text{ in }H^1(U_j),\qquad u_k\longrightarrow u\text{ in }L^2(U_j)\quad\text{for every }j.
$$

The local limit agrees with the global weak $L^2$ limit. Using smooth exhaustion sets avoids imposing any unprinted boundary regularity on a general $\Omega'$.

For a smooth [compactly supported](../../../function.md#compact-support) [test function](../../../distribution-theory.md#test-function), the weak equation passes to the limit: the fixed bounded coefficients multiply fixed [test functions](../../../distribution-theory.md#test-function), and local [weak gradient](../../../distribution-theory.md#weak-gradient) convergence handles both the principal and drift terms. The zeroth-order term passes by local $L^2$ convergence. Thus $Lu=f$ weakly, $u\in H^1_{\mathrm{loc}}(\Omega)$, and the global bound already proved gives $u\in S_K$.

To improve convergence of the [gradients](../../../calculus.md#gradient), put $w_k=u_k-u$. Crucially the forcing is the same for all $k$, so $Lw_k=0$. Given $\Omega'\Subset\Omega$, choose $j$ with $\overline{\Omega'}\subset U_j$. Apply part (i) on $U_j$ to the homogeneous equation for $w_k$:

$$
\|w_k\|_{H^1(\Omega')}\leq C\|w_k\|_{L^2(U_j)}\longrightarrow0.
$$

This establishes [strong local Sobolev compactness for a fixed elliptic equation](../../../partial-differential-equation.md#strong-local-sobolev-compactness-for-a-fixed-elliptic-equation) and proves

$$
\boxed{u\in S_K,\qquad u_{k'}\longrightarrow u\text{ in }W^{1,2}(\Omega')\text{ for every }\Omega'\Subset\Omega.}
$$

## 4

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

We prove the [Interior second-derivative estimate for the Poisson equation](../../../distribution-theory.md#interior-second-derivative-estimate-for-the-poisson-equation) using [difference quotients](../../../calculus.md#difference-quotient), rather than differentiating the $L^2$ forcing. Fix a coordinate $e_k$ and write $\delta_hv(x)=(v(x+he_k)-v(x))/h$. Choose a [smooth cutoff function](../../../analysis.md#smooth-cutoff-function) $\eta$ equal to one on $\Omega'$ with support compactly contained in $\Omega$, leaving room for all translations with sufficiently small $|h|$. We can arrange $|D\eta|\leq C(n)/d$, where $d=\operatorname{dist}(\Omega',\partial\Omega)$.

The standard difference quotient lemmas give discrete [integration by parts](../../../calculus.md#integration-by-parts), $\int a\delta_{-h}b=-\int(\delta_ha)b$, and $\|\delta_hv\|_2\leq\|D_kv\|_2$ on the relevant enlarged set. In the [weak formulation](../../../partial-differential-equation.md#weak-formulation) $\int Du\cdot D\varphi=-\int f\varphi$, use the admissible [test function](../../../distribution-theory.md#test-function) $\varphi=-\delta_{-h}(\eta^2\delta_hu)$. Moving a difference quotient onto $Du$ gives

$$
\int\eta^2|D\delta_hu|^2+2\int\eta\delta_hu\,D\delta_hu\cdot D\eta=\int f\,\delta_{-h}(\eta^2\delta_hu).
$$

Set $X=\|\eta D\delta_hu\|_2$ and $Y=\|D\eta\,\delta_hu\|_2$. The cross term has absolute value at most $2XY$. Since $0\leq\eta\leq1$, the difference quotient lemma on the right gives

$$
\left|\int f\,\delta_{-h}(\eta^2\delta_hu)\right|\leq\|f\|_2\|D_k(\eta^2\delta_hu)\|_2\leq\|f\|_2(X+2Y).
$$

The [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) now implies $X^2\leq C(Y^2+\|f\|_2^2)$. Moreover $Y\leq C(n)d^{-1}\|Du\|_{L^2(\Omega)}$, independently of $h$. Hence, for every coordinate $k$,

$$
\|D\delta_hu\|_{L^2(\Omega')}\leq C(n,d)\left(\|Du\|_{L^2(\Omega)}+\|f\|_{L^2(\Omega)}\right).
$$

By the [Sobolev characterization by bounded difference quotients](../../../sobolev-space.md#sobolev-characterization-by-bounded-difference-quotients), applied to each first [weak derivative](../../../distribution-theory.md#weak-derivative) on smaller interior sets, these uniform bounds give all second [weak derivatives](../../../distribution-theory.md#weak-derivative). Their bounds pass to the weak limit as $h\to0$. Thus $u\in W^{2,2}_{\mathrm{loc}}(\Omega)$ and

$$
\boxed{\|u\|_{W^{2,2}(\Omega')}\leq C(n,d)\left(\|u\|_{W^{1,2}(\Omega)}+\|f\|_{L^2(\Omega)}\right).}
$$

No derivative of $f$ is used, and no boundary condition is needed for this interior [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) argument.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

First perform [homogenization of Dirichlet boundary data](../../../sobolev-space.md#homogenization-of-dirichlet-boundary-data): put $v=u-\psi\in H_0^1(B_1^+)$ and $g=f-\Delta\psi\in L^2(B_1^+)$. Then $\Delta v=g$ weakly. Extend both functions oddly across the flat face:

$$
\widetilde v(x',t)=\begin{cases}v(x',t)&t>0,\\-v(x',-t)&t<0,\end{cases}\qquad\widetilde g(x',t)=\begin{cases}g(x',t)&t>0,\\-g(x',-t)&t<0.\end{cases}
$$

The zero [Sobolev trace](../../../sobolev-space.md#trace-operator) of $v$ makes this [odd reflection](../../../sobolev-space.md#odd-reflection) an $H^1(B_1)$ function. This can also be seen by approximating $v$ by smooth [compactly supported](../../../function.md#compact-support) functions in $B_1^+$ and reflecting the approximants. Its $H^1$ [norm](../../../functional-analysis.md#norm) is $\sqrt2$ times that of $v$, and $\|\widetilde g\|_{L^2(B_1)}=\sqrt2\|g\|_{L^2(B_1^+)}$.

For $\phi\in C_c^\infty(B_1)$, the function $\phi(x',t)-\phi(x',-t)$ on the upper half-ball has zero trace on the flat face and vanishes near the curved face, hence is an admissible $H_0^1$ test. Splitting the integrals over the two half-balls and changing $t$ to $-t$ shows

$$
\int_{B_1}D\widetilde v\cdot D\phi=-\int_{B_1}\widetilde g\phi.
$$

Thus $\Delta\widetilde v=\widetilde g$ weakly throughout the full ball; there is no extra distribution on the reflecting face.

Apply part (i) to $B_{1/2}\Subset B_1$, restrict to the upper half-ball, and then add $\psi$. Since $\|\Delta\psi\|_2\leq C(n)\|\psi\|_{H^2}$, this gives $u\in W^{2,2}(B_{1/2}^+)$ and the [second-derivative estimate at a flat Dirichlet boundary](../../../distribution-theory.md#second-derivative-estimate-at-a-flat-dirichlet-boundary)

$$
\boxed{\|u\|_{W^{2,2}(B_{1/2}^+)}\leq C(n)\left(\|u\|_{W^{1,2}(B_1^+)}+\|f\|_{L^2(B_1^+)}+\|\psi\|_{W^{2,2}(B_1^+)}\right).}
$$

The fixed radii leave distance $1/2$ for the interior estimate, so the constant depends only on dimension.

## 5

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $B_r(x_0)$ have closure contained in the domain of a [harmonic function](../../../partial-differential-equation.md#harmonic-function) $u$. Put $\omega_n=|B_1(0)|$, so $|B_r|=\omega_nr^n$ and $|\partial B_r|=n\omega_nr^{n-1}$. The sphere and ball [mean value properties for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) are

$$
\boxed{u(x_0)=\frac1{|\partial B_r|}\int_{\partial B_r(x_0)}u\,dS=\frac1{|B_r|}\int_{B_r(x_0)}u\,dx.}
$$

To prove the sphere formula, define its average using a fixed unit sphere:

$$
M(r)=\frac1{n\omega_n}\int_{S^{n-1}}u(x_0+r\theta)\,dS_\theta.
$$

Differentiating under the integral and applying the [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
M'(r)=\frac1{n\omega_nr^{n-1}}\int_{\partial B_r(x_0)}\partial_\nu u\,dS=\frac1{n\omega_nr^{n-1}}\int_{B_r(x_0)}\Delta u\,dx=0.
$$

Continuity gives $M(r)\to u(x_0)$ as $r\downarrow0$, proving the spherical average identity. Integrating that identity over radii with the polar-coordinate weight yields

$$
\int_{B_r(x_0)}u=\int_0^r n\omega_nt^{n-1}M(t)\,dt=\omega_nr^n u(x_0),
$$

which proves the ball identity. For $n=1$, the sphere average is the average of the two endpoints, and the same formulas hold with the counting surface measure.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

A local form of the [Harnack inequality for harmonic functions](../../../partial-differential-equation.md#harnack-inequality-for-harmonic-functions) is: if $u\geq0$ is harmonic on a neighbourhood of $\overline{B_{4r}(y)}$, then

$$
\boxed{\sup_{B_r(y)}u\leq3^n\inf_{B_r(y)}u.}
$$

For $x,z\in B_r(y)$, the triangle inequality gives $B_r(x)\subset B_{3r}(z)\subset B_{4r}(y)$. The ball [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) and nonnegativity therefore imply

$$
u(x)=\frac1{|B_r|}\int_{B_r(x)}u\leq\frac1{|B_r|}\int_{B_{3r}(z)}u=\frac{|B_{3r}|}{|B_r|}u(z)=3^nu(z).
$$

Taking the supremum over $x$ and infimum over $z$ proves the inequality, including the case where the infimum is zero. No strict positivity assumption was used.

On a connected domain $\Omega$, the equivalent compact-set statement is that for each nonempty compact $K\Subset\Omega$ there exists $C(K,\Omega,n)$ with

$$
\boxed{\sup_Ku\leq C(K,\Omega,n)\inf_Ku.}
$$

Here is the passage from balls to this statement. Cover $K$ by finitely many small balls $B_{r_j}(y_j)$ whose quadrupled closed balls lie in $\Omega$. Join their centres to a fixed centre by paths in $\Omega$. Each of the finitely many paths has compact image and positive distance from the boundary, so subdividing it gives a finite chain of overlapping small balls whose quadrupled closures also lie in $\Omega$. The local inequality compares any two points in each ball; using a point in each successive overlap propagates comparisons along the chain. The number of comparisons is bounded uniformly over this finite collection of chains and covering balls. Multiplying the factors $3^n$ gives one finite constant for all pairs $x,z\in K$, proving the compact-set inequality. In particular a nonnegative harmonic function vanishing at one interior point vanishes throughout a connected domain.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Let $m=\inf_{\mathbb R^n}u$, which is finite because $u$ is bounded, and put $v=u-m$. Then $v\geq0$ is harmonic. Choose points $y_j$ with $v(y_j)\to0$. For any fixed $x$, choose $r_j$ large enough that $x,y_j\in B_{r_j}(0)$. Since $v$ is harmonic on all of $\mathbb R^n$, the [Harnack inequality for harmonic functions](../../../partial-differential-equation.md#harnack-inequality-for-harmonic-functions) on $B_{4r_j}(0)$ gives

$$
0\leq v(x)\leq3^nv(y_j)\longrightarrow0.
$$

The comparison factor is independent of the growing radius, which is essential. Thus $v(x)=0$ for every $x$ and

$$
\boxed{u\equiv m\text{ on }\mathbb R^n.}
$$

This proves the [Liouville theorem for harmonic functions](../../../partial-differential-equation.md#harmonic-liouville-theorem) in every dimension. In fact the argument only needs an entire harmonic function to be bounded below; changing its sign gives the corresponding bounded-above result.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

Set $X=Du/\sqrt{1+|Du|^2}$. Since $u\in C^2(\mathbb R^n)$, the field is $C^1$, and $|X|\leq1$ everywhere, even when the [gradient](../../../calculus.md#gradient) of $u$ is unbounded. The [divergence theorem](../../../calculus.md#divergence-theorem) on $B_R(0)$ gives

$$
\kappa|B_R|=\int_{\partial B_R}X\cdot\nu\,dS,\qquad |\kappa|\leq\frac{|\partial B_R|}{|B_R|}=\frac nR.
$$

Letting $R\to\infty$ proves $\kappa=0$. This is the fact that [an entire bounded vector field cannot have nonzero constant divergence](../../../calculus.md#an-entire-bounded-vector-field-cannot-have-nonzero-constant-divergence); it holds in every dimension.

The equation is now exactly the [minimal surface equation for a graph](../../../second-fundamental-form.md#minimal-surface-equation-for-a-graph). Apply the supplied [Bernstein theorem for minimal graphs](../../../second-fundamental-form.md#bernstein-theorem-for-minimal-graphs) in dimensions $1\leq n\leq7$ to conclude

$$
\boxed{\kappa=0,\qquad u(x)=a\cdot x+b\quad(a\in\mathbb R^n,\ b\in\mathbb R).}
$$

Thus no nonzero constant right-hand side is possible for an entire graph, and in the stated dimensions every possible graph is an affine plane.

## 6

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Let $M$ bound the [operator norm](../../../continuous-dual-space.md#operator-norm) of $D^2F$; the bound on individual second derivatives supplies such an $M$ depending also on dimension. The [Taylor theorem](../../../calculus.md#taylor-theorem) with integral remainder gives

$$
F(p)=F(0)+DF(0)\cdot p+\int_0^1(1-t)\,p^TD^2F(tp)p\,dt.
$$

Thus [quadratic growth from a bounded Hessian](../../../calculus.md#quadratic-growth-from-a-bounded-hessian) gives

$$
|F(p)|\leq|F(0)|+|DF(0)||p|+\frac M2|p|^2\leq C(1+|p|^2).
$$

Since $\Omega$ is bounded it has finite measure, and a function in the [Sobolev space](../../../sobolev-space.md) $H^1(\Omega)$ has $Du\in L^2(\Omega)$. The given lower bound also implies that the integrand is nonnegative. Consequently

$$
\boxed{0\leq\mathcal F(u)=\int_\Omega F(Du)\leq C\left(|\Omega|+\|Du\|_2^2\right)<\infty.}
$$

For later use the same [Hessian](../../../calculus.md#hessian-matrix) bound yields $|DF(p)|\leq|DF(0)|+M|p|$, hence $DF(Du)\in L^2(\Omega)$.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Suppose $u_k\rightharpoonup u$ in $H^1(\Omega)$. Then $Du_k\rightharpoonup Du$ in $L^2(\Omega;\mathbb R^n)$. Since $F$ is a differentiable [convex function](../../../real-analysis.md#convex-function), its supporting inequality is

$$
F(p)\geq F(q)+DF(q)\cdot(p-q).
$$

Take $p=Du_k(x)$, $q=Du(x)$ and integrate. Part (i) shows that every energy is finite and that the fixed field $DF(Du)$ belongs to $L^2$, so

$$
\mathcal F(u_k)\geq\mathcal F(u)+\int_\Omega DF(Du)\cdot(Du_k-Du).
$$

The last integral tends to zero by the definition of [weak convergence](../../../weak-topology.md#weak-convergence) in $L^2$. Therefore

$$
\boxed{\mathcal F(u)\leq\liminf_{k\to\infty}\mathcal F(u_k).}
$$

This is [weak lower semicontinuity of convex gradient energies](../../../calculus-of-variations.md#weak-lower-semicontinuity-of-convex-gradient-energies). It uses a fixed supporting [gradient](../../../calculus.md#gradient) at the limit; [weak convergence](../../../weak-topology.md#weak-convergence) alone would not justify passing pointwise through the nonlinear integrand.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

The affine class $C_\psi=\psi+H_0^1(\Omega)$ is nonempty, and part (i) gives a finite comparison energy $\mathcal F(\psi)$. Since $F(p)\geq\alpha|p|^2$, its energy infimum $m$ satisfies $0\leq m\leq\mathcal F(\psi)$. Choose a [minimizing sequence](../../../calculus-of-variations.md#minimizing-sequence) $u_k\in C_\psi$ with $\mathcal F(u_k)\leq\mathcal F(\psi)+1$. Then

$$
\alpha\|Du_k\|_2^2\leq\mathcal F(u_k)\leq\mathcal F(\psi)+1.
$$

The [gradient](../../../calculus.md#gradient) bounds also control the full [Sobolev norm](../../../sobolev-space.md#sobolev-norm). Indeed $w_k=u_k-\psi\in H_0^1$, so the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) gives

$$
\|u_k\|_2\leq\|\psi\|_2+\|w_k\|_2\leq\|\psi\|_2+C_\Omega\bigl(\|Du_k\|_2+\|D\psi\|_2\bigr).
$$

Thus $u_k$ is bounded in the [Hilbert space](../../../hilbert-space.md) $H^1(\Omega)$. Its weak compactness yields a weakly convergent subsequence $u_k\rightharpoonup u$. The closed linear subspace $H_0^1$ is weakly closed, hence $u-\psi\in H_0^1$ and $u\in C_\psi$. By part (ii),

$$
m\leq\mathcal F(u)\leq\liminf_k\mathcal F(u_k)=m.
$$

The [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) therefore proves

$$
\boxed{u\in C_\psi,\qquad\mathcal F(u)=\min_{v\in C_\psi}\mathcal F(v).}
$$

Neither a smooth boundary nor a classical trace theorem is needed: the boundary condition is encoded by the closed [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space).

<h3 id="6/iv">iv</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6/iv)

**No additional hypothesis on $F$ is needed here for scalar interior $C^{1,\beta}$ regularity.** In the elliptic sense of uniform convexity, the assumptions already give constants $0<\lambda\leq M<\infty$ with $\lambda I\leq D^2F(p)\leq MI$ for all $p$. The following argument gives [interior gradient regularity for uniformly convex autonomous energies](../../../real-analysis.md#interior-gradient-regularity-for-uniformly-convex-autonomous-energies).

The [first variation](../../../calculus-of-variations.md#first-variation) at the minimizer exists because $|DF(p)|\leq C(1+|p|)$, and its weak [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
\int_\Omega DF(Du)\cdot D\varphi=0\qquad(\varphi\in C_c^\infty(\Omega)).
$$

For a coordinate difference quotient $\delta_hu$, subtract the translated equation and the original equation. The [averaged linearization of a nonlinear divergence-form equation](../../../partial-differential-equation.md#averaged-linearization-of-a-nonlinear-divergence-form-equation) gives

$$
\operatorname{div}(A_hD\delta_hu)=0,\qquad A_h(x)=\int_0^1D^2F\bigl((1-t)Du(x)+tDu(x+he_k)\bigr)\,dt.
$$

These measurable symmetric matrices satisfy $\lambda I\leq A_h\leq MI$ independently of $h$. The [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality) and the standard bound $\|\delta_hu\|_2\leq\|D_ku\|_2$ bound $D\delta_hu$ on every smaller interior set. Quoting the [Sobolev characterization by bounded difference quotients](../../../sobolev-space.md#sobolev-characterization-by-bounded-difference-quotients) yields $u\in H^2_{\mathrm{loc}}$.

Now $DF$ is globally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity), so the [Sobolev chain rule](../../../distribution-theory.md#sobolev-chain-rule) and commutation of distributional derivatives allow differentiation of the weak equation. Each $v_k=D_ku\in H^1_{\mathrm{loc}}$ satisfies

$$
\operatorname{div}(A Dv_k)=0,\qquad A(x)=D^2F(Du(x)),\qquad\lambda I\leq A(x)\leq MI.
$$

The [De Giorgi-Nash-Moser theorem](../../../elliptic-boundary-value-problem.md#de-giorgi-nash-moser-theorem) states that [weak solutions](../../../partial-differential-equation.md#weak-solution) of this scalar divergence-form equation with bounded measurable [uniformly elliptic](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) coefficients are locally [Hölder continuous](../../../sobolev-space.md#holder-condition). It gives a common $\beta\in(0,1)$ depending only on $n$ and the ellipticity ratio $M/\lambda$, with $D_ku\in C^{0,\beta}_{\mathrm{loc}}$ for every $k$. A Sobolev function whose [weak gradient](../../../distribution-theory.md#weak-gradient) is continuous has a $C^1$ representative, as follows by local [mollification](../../../distribution-theory.md#mollification) and integration of its [gradient](../../../calculus.md#gradient). Hence

$$
\boxed{u\in C^{1,\beta}_{\mathrm{loc}}(\Omega).}
$$

The higher-regularity conclusion comes from differentiating an autonomous scalar equation; it does not rely on boundary regularity or a higher derivative such as $D^3F$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
