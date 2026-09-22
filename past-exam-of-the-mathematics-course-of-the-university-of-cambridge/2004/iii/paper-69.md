# Paper 69

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper69.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper69.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Apply the [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) to the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) and put $z=h\lambda$. Its [stability function](../../../numerical-analysis.md#stability-function) is

$$
R(z)=1+z\,b^T(I-zA)^{-1}\mathbf1=\frac{P(z)}{Q(z)},\qquad Q(z)=\det(I-zA).
$$

Since $A$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), $Q$ has [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) $s$. The [adjugate matrix](../../../linear-algebra.md#adjugate-matrix) formula gives $\deg P\le s$, but the additional condition gives

$$
\lim_{z\to\infty}R(z)=1-b^TA^{-1}\mathbf1=0,
$$

so actually $\deg P\le s-1$. The specified [order of a numerical method](../../../numerical-analysis.md#order-of-a-numerical-method) implies $R(z)=e^z+O(z^{2s})$ near zero. Therefore the [Padé identification of a Radau stability function](../../../numerical-analysis.md#pade-identification-of-a-radau-stability-function) makes $R$ the $[s-1/s]$ [Padé approximant](../../../isolated-singularity.md#pade-approximant) to the [exponential function](../../../calculus.md#exponential-function): its numerator and denominator have the required degrees, and its [Taylor series](../../../calculus.md#taylor-series) agrees through degree $2s-1$.

In the permitted [A-stability of near-diagonal exponential Padé approximants](../../../numerical-analysis.md#a-stability-of-near-diagonal-exponential-pade-approximants), take $m=s-1$, $n=s$. Then $n-2\le m\le n$, so **the scheme is [A-stable](../../../numerical-analysis.md#a-stability)**. The same [stability function](../../../numerical-analysis.md#stability-function) also tends to zero at infinity, giving [L-stability](../../../numerical-analysis.md#l-stability).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For one stage, first-order [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) gives $b_1=1$. The condition $b^TA^{-1}\mathbf1=1$ then gives $a_{11}=1$. Hence the scheme is **the [Backward Euler method](../../../numerical-analysis.md#backward-euler-method)**:

$$
y_{n+1}=y_n+h f(t_n+h,y_{n+1}).
$$

It is a one-node [collocation Runge-Kutta method](../../../numerical-analysis.md#collocation-runge-kutta-method) with $c_1=1$. Specifically, choose a linear [polynomial](../../../polynomial.md) $p(t)$ on $[t_n,t_n+h]$ with $p(t_n)=y_n$ and impose $p'(t_n+h)=f(t_n+h,p(t_n+h))$. Its derivative is constant, so $p(t_n+h)-p(t_n)=hp'(t_n+h)$, exactly the [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) update.

## 2

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $h=\Delta x$, $k=\Delta t$, and assume $a,u$ are sufficiently [smooth](../../../analysis.md#smooth-function) for the following [Taylor expansions](../../../calculus.md#taylor-expansion). The [symmetric half-grid diffusion consistency](../../../finite-difference.md#symmetric-half-grid-diffusion-consistency) calculation gives

$$
L_hu=\frac{a(x-h/2)[u(x-h)-u(x)]+a(x+h/2)[u(x+h)-u(x)]}{h^2}=(au_x)_x+h^2E_2+O(h^4),
$$

where

$$
E_2=\frac{a u_{xxxx}}{12}+\frac{a'u_{xxx}}6+\frac{a''u_{xx}}8+\frac{a'''u_x}{24}.
$$

The [normalized local truncation error](../../../numerical-analysis.md#normalized-local-truncation-error) of the full update is consequently

$$
\mathcal T_{h,k}=\frac{u(x,t+k)-u(x,t)}k-L_hu=u_t-(au_x)_x+\frac{k}{2}u_{tt}-h^2E_2+O(k^2+h^4).
$$

**The PDF prints an [advection equation](../../../partial-differential-equation.md#transport-equation), $u_t=a(x)u_x$, whereas this stencil approximates conservative diffusion, $u_t=(au_x)_x$.** For the literal printed equation the leading defect is $(a-a')u_x-a u_{xx}$, which generally does not vanish: the method is **inconsistent, with an $O(1)$ normalized defect**.

For the intended [variable-coefficient conservative diffusion equation](../../../diffusion-equation.md#variable-coefficient-conservative-diffusion-equation), the first two terms cancel and $\mathcal T_{h,k}=O(k+h^2)$. Under the parabolic step scaling $k=O(h^2)$, this is **$O(h^2)$**, while the unnormalized one-step [local truncation error](../../../numerical-analysis.md#local-truncation-error) is $k\mathcal T_{h,k}=O(h^4)$. These two orders use different normalizations. With [numerical stability](../../../numerical-analysis.md#stability-of-a-numerical-method) and compatible smooth initial and [boundary conditions](../../../differential-equation.md#boundary-condition), the intended diffusion problem has global error $O(k+h^2)$ on a fixed time interval. Positivity and boundedness of $a$ alone do not justify the displayed [Taylor expansion](../../../calculus.md#taylor-expansion); coefficient regularity is also needed for that error formula.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Put $r=k/h^2$. The update is

$$
U_m^{n+1}=r a_{m-1/2}U_{m-1}^n+[1-r(a_{m-1/2}+a_{m+1/2})]U_m^n+r a_{m+1/2}U_{m+1}^n.
$$

Under $k\le h^2/(2\beta)$, all three weights are nonnegative and sum to one. With the imposed zero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), this is a [convex combination](../../../mathematical-optimization.md#convex-combination) including any boundary values. Thus the [monotone half-grid diffusion update](../../../finite-difference.md#monotone-half-grid-diffusion-update) gives

$$
\boxed{\|U^{n+1}\|_\infty\le\|U^n\|_\infty\le\|U^0\|_\infty}.
$$

Differences of two computed solutions obey the same estimate, proving [numerical stability](../../../numerical-analysis.md#stability-of-a-numerical-method) in the discrete [maximum norm](../../../functional-analysis.md#supremum-norm), uniformly in $h,k,n$.

There is also an [L2 norm](../../../real-analysis.md#l2-norm) proof. The diffusion [matrix](../../../vector-space.md#matrix) $L_h$ is [symmetric](../../../set-theory.md#symmetric-relation) and satisfies

$$
v^TL_hv=-h^{-2}\sum_{m=0}^{M-1}a_{m+1/2}(v_{m+1}-v_m)^2,\qquad v_0=v_M=0.
$$

Since $(v_{m+1}-v_m)^2\le2(v_{m+1}^2+v_m^2)$, every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) lies in $[-4\beta/h^2,0]$. Hence the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $I+kL_h$ lie in $[-1,1]$ under the same step restriction, and the [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) gives an [L2 norm](../../../real-analysis.md#l2-norm) contraction. These stability estimates are valid for the printed recurrence, although they cannot repair its inconsistency with the printed [advection equation](../../../partial-differential-equation.md#transport-equation).

## 3

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Expanding the symmetric spatial stencil by the [Taylor theorem](../../../calculus.md#taylor-theorem) gives

$$
L_hu=\frac{\alpha+2\beta+2\gamma}{h^2}u+(\beta+4\gamma)u_{xx}+\frac{h^2}{12}(\beta+16\gamma)u_{xxxx}+\frac{h^4}{360}(\beta+64\gamma)u_{xxxxxx}+O(h^6).
$$

[Consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) and cancellation of the $h^2$ term require $\alpha+2\beta+2\gamma=0$, $\beta+4\gamma=1$, and $\beta+16\gamma=0$. Solving this [linear system](../../../linear-algebra.md#system-of-linear-equations) gives

$$
\boxed{\alpha=-\frac52,\qquad\beta=\frac43,\qquad\gamma=-\frac1{12}}.
$$

The resulting [fourth-order centered second derivative](../../../finite-difference.md#fourth-order-centered-second-derivative) has

$$
L_hu=u_{xx}-\frac{h^4}{90}u_{xxxxxx}+O(h^6).
$$

The nonzero next coefficient proves that **the highest spatial [order of a numerical method](../../../numerical-analysis.md#order-of-a-numerical-method) is four** for this three-parameter stencil.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the [method of lines](../../../finite-difference.md#method-of-lines) in part (a), the [Fourier symbol](../../../finite-difference.md#fourier-symbol-of-a-difference-operator) of the spatial operator is

$$
\lambda_h(\theta)=h^{-2}\left(-\frac52+\frac83\cos\theta-\frac16\cos2\theta\right)=-\frac4{h^2}\sin^2\frac\theta2\left(1+\frac13\sin^2\frac\theta2\right)\le0.
$$

Each [Fourier mode](../../../fourier-analysis.md#fourier-mode) therefore evolves by $\widehat U(\theta,t)=e^{t\lambda_h(\theta)}\widehat U(\theta,0)$, whose multiplier has [modulus](../../../complex-analysis.md#modulus) at most one. The [discrete Parseval identity](../../../numerical-analysis.md#discrete-parseval-identity) gives

$$
\boxed{\|U(t)\|_{\ell_h^2}\le\|U(0)\|_{\ell_h^2}},\qquad\|U\|_{\ell_h^2}^2=h\sum_{m\in\mathbb Z}|U_m|^2.
$$

Thus the [fourth-order centered second derivative](../../../finite-difference.md#fourth-order-centered-second-derivative) gives an **unconditionally stable semidiscrete evolution in the [L2 norm](../../../real-analysis.md#l2-norm)**. No time integration method has yet been chosen, so no time-step restriction belongs to this conclusion.

An arbitrary [L2 function](../../../measure-theory.md#square-integrable-function) does not have well-defined point samples. For the stated initial data one may use [cell-average projection](../../../finite-difference.md#cell-average-projection), $U_m(0)=h^{-1}\int_{x_m-h/2}^{x_m+h/2}u_0(x)\,dx$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $h\sum_m|U_m(0)|^2\le\|u_0\|_{L^2}^2$, providing a bounded initialization for the stability estimate.

## 4

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $V$ be a real [Hilbert space](../../../hilbert-space.md), $a:V\times V\to\mathbb R$ a [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form), and $\ell\in V'$ a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional). Assume constants $C<\infty$, $\alpha>0$ satisfy

$$
|a(v,w)|\le C\|v\|_V\|w\|_V,\qquad a(v,v)\ge\alpha\|v\|_V^2\qquad(v,w\in V).
$$

The second hypothesis says that $a$ is a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form). The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) then supplies a unique [weak solution](../../../partial-differential-equation.md#weak-solution) $u\in V$ with $a(u,v)=\ell(v)$ for every $v\in V$, and $\|u\|_V\le\|\ell\|_{V'}/\alpha$.

For a finite-dimensional trial [linear subspace](../../../vector-space.md#vector-subspace) $V_h\subset V$, the same boundedness and coercivity constants apply to the restricted form. Since a [finite-dimensional subspace is closed](../../../functional-analysis.md#finite-dimensional-subspace-is-closed), $V_h$ is itself a [Hilbert space](../../../hilbert-space.md). Thus there is a unique [Galerkin method](../../../partial-differential-equation.md#galerkin-method) solution $u_h\in V_h$ satisfying $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$. The [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality) $a(u-u_h,v_h)=0$ gives the [Céa lemma](../../../numerical-analysis.md#cea-s-lemma):

$$
\boxed{\|u-u_h\|_V\le\frac C\alpha\inf_{v_h\in V_h}\|u-v_h\|_V}.
$$

In particular, approximation by the trial spaces implies [numerical convergence](../../../numerical-analysis.md#convergence-of-a-numerical-method). For a complex [Hilbert space](../../../hilbert-space.md), replace bilinearity by a [sesquilinear form](../../../linear-algebra.md#sesquilinear-form), take $\ell$ antilinear in the test variable, and require $\operatorname{Re}a(v,v)\ge\alpha\|v\|_V^2$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) $V=H_0^1(0,1)$ with $\|v\|_V=\|v'\|_{L^2}$. The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) $\|v\|_{L^2}\le\pi^{-1}\|v'\|_{L^2}$ makes this a complete [Hilbert space](../../../hilbert-space.md) norm. The [weak formulation](../../../partial-differential-equation.md#weak-formulation) is

$$
a(u,v)=\int_0^1[p(x)u'(x)v'(x)+q(x)u(x)v(x)]\,dx=\ell(v),\qquad\ell(v)=\int_0^1f(x)v(x)\,dx.
$$

Assume $p,q$ are measurable and satisfy the supplied bounds almost everywhere. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) give

$$
|a(u,v)|\le\left(p_1+\frac{q_1}{\pi^2}\right)\|u'\|_{L^2}\|v'\|_{L^2}.
$$

Because $p\ge p_0>0$ and $q\ge0$,

$$
a(v,v)=\int_0^1[p(v')^2+qv^2]\,dx\ge p_0\|v'\|_{L^2}^2.
$$

This is the [coercive variable-coefficient Dirichlet form](../../../functional-analysis.md#coercive-variable-coefficient-dirichlet-form). If $f\in L^2(0,1)$, then $|\ell(v)|\le\pi^{-1}\|f\|_{L^2}\|v\|_V$; more generally one may assume $f\in H^{-1}(0,1)=V'$. Some such source regularity is necessary to invoke the theorem. All hypotheses of the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) now hold, with **coercivity constant $p_0$ and boundedness constant $p_1+q_1/\pi^2$**, giving the unique [weak solution](../../../partial-differential-equation.md#weak-solution) and every conforming [Galerkin method](../../../partial-differential-equation.md#galerkin-method) approximation. This argument does not require a pointwise derivative of $p$.

## 5

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Along the exact [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) solution, the [chain rule](../../../calculus.md#chain-rule) gives $g(y)=f'(y)f(y)=y''$. Insert the exact solution into the [symmetric two-step two-derivative formula](../../../numerical-analysis.md#symmetric-two-step-two-derivative-formula) and expand about the middle time $t=t_{n+1}$. Its unnormalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) is

$$
\begin{aligned}
\delta_h={}&y(t+h)-y(t-h)-\frac{7h}{15}[y'(t+h)+y'(t-h)]-\frac{16h}{15}y'(t)\\
&+\frac{h^2}{15}[y''(t+h)-y''(t-h)].
\end{aligned}
$$

The coefficients of $hy'$, $h^3y'''$ and $h^5y^{(5)}$ are respectively

$$
2-\frac{14}{15}-\frac{16}{15}=0,\qquad\frac13-\frac7{15}+\frac2{15}=0,\qquad\frac1{60}-\frac7{180}+\frac1{45}=0.
$$

The centered residual is an [odd function](../../../calculus.md#odd-function) of $h$, so every even power cancels. The next coefficient is

$$
\frac1{2520}-\frac7{5400}+\frac1{900}=\frac1{4725},\qquad\delta_h=\frac{h^7}{4725}y^{(7)}(t)+O(h^9).
$$

Thus **the method has order six**. Its [zero-stability](../../../numerical-analysis.md#zero-stability) roots at $h=0$ are the simple roots $1,-1$. With sufficiently accurate starts and smooth derivative evaluation maps, [convergence of a zero-stable multiderivative method](../../../numerical-analysis.md#convergence-of-a-zero-stable-multiderivative-method) gives sixth-order error on fixed time intervals. The [first Dahlquist barrier](../../../numerical-analysis.md#first-dahlquist-barrier) for ordinary [linear multistep methods](../../../numerical-analysis.md#linear-multistep-method) does not apply, because this is a [multiderivative multistep method](../../../numerical-analysis.md#multiderivative-multistep-method).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The stability convention matters. The [Cambridge numerical analysis notes](https://www.damtp.cam.ac.uk/user/na/PartIB/Lect10.pdf) define a [strict linear stability domain](../../../numerical-analysis.md#strict-linear-stability-domain) through decay $y_n\to0$. For a multistep recurrence, robust decay requires every [amplification root](../../../numerical-analysis.md#amplification-root) to lie strictly inside the [unit disk](../../../geometry-and-topology.md#unit-disk). With that convention we can prove the stronger result that **this method's strict linear stability domain is empty**, and therefore bounded. Mere boundedness of oscillatory sequences gives a different answer, described below.

On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), $g(y)=\lambda^2y$. With $z=h\lambda$, the [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) is

$$
D\xi^2-16z\xi-A=0,\qquad D=z^2-7z+15,\qquad A=z^2+7z+15.
$$

Exclude $D=0$, where the intended two-step update cannot be solved. If both [polynomial roots](../../../polynomial.md#root-of-a-polynomial) have [modulus](../../../complex-analysis.md#modulus) below one, their product requires $|A|<|D|$. But

$$
|A|^2-|D|^2=28\operatorname{Re}z\,(|z|^2+15),
$$

so necessarily $\operatorname{Re}z<0$. The [complex quadratic Schur criterion](../../../numerical-analysis.md#complex-quadratic-schur-criterion) also requires

$$
|\overline D(-16z)-(-A)(-16\overline z)|<|D|^2-|A|^2.
$$

Its left-hand side equals $32|\operatorname{Re}z|(|z|^2+15)$, while for $\operatorname{Re}z<0$ its right-hand side is only $28|\operatorname{Re}z|(|z|^2+15)$. The inequality is impossible. Thus

$$
\boxed{\mathcal D_{\rm decay}=\varnothing}.
$$

For comparison, the [bounded-root stability set of the symmetric two-derivative formula](../../../numerical-analysis.md#bounded-root-stability-set-of-the-symmetric-two-derivative-formula) is unbounded. On $z=iy$, rotate the [amplification polynomial](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) into a real reciprocal quadratic. Its two roots are distinct and on the [unit circle](../../../complex-analysis.md#complex-unit-circle) precisely when

$$
(15-y^2)^2-15y^2>0,
$$

equivalently $y^2<(45-15\sqrt5)/2$ or $y^2>(45+15\sqrt5)/2$. In particular, arbitrarily large imaginary parameters give bounded, undamped numerical oscillations. At the two equality thresholds, repeated [unit-circle roots](../../../polynomial.md#unit-circle-root) produce unbounded solutions. Hence the question's bounded-domain claim holds for the strict decay convention; it does not hold if the phrase is interpreted using the non-growing [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method).

## 6

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A constant-step [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) has the form

$$
\sum_{j=0}^k\alpha_jY_{n+j}=h\sum_{j=0}^k\beta_jf(t_{n+j},Y_{n+j}),\qquad\rho(\zeta)=\sum_{j=0}^k\alpha_j\zeta^j,\quad\sigma(\zeta)=\sum_{j=0}^k\beta_j\zeta^j,
$$

with $\alpha_k\ne0$. The [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) encode both accuracy and error propagation. The method has [order of a numerical method](../../../numerical-analysis.md#order-of-a-numerical-method) $p$ when insertion of a sufficiently smooth exact solution leaves an unnormalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) $O(h^{p+1})$. The [exponential-symbol order criterion for a multistep method](../../../numerical-analysis.md#exponential-symbol-order-criterion-for-a-multistep-method) expresses this as $\rho(e^z)-z\sigma(e^z)=O(z^{p+1})$. In particular, first-order [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) requires $\rho(1)=0$ and $\rho'(1)=\sigma(1)$.

Accuracy alone is insufficient. For $f=0$, perturbations obey the recurrence $\rho(E)e_n=0$. The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) requires every [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) $\rho$ to lie in the closed [unit disk](../../../geometry-and-topology.md#unit-disk), with each [unit-circle root](../../../polynomial.md#unit-circle-root) simple. This is [zero-stability](../../../numerical-analysis.md#zero-stability). A root outside the [unit disk](../../../geometry-and-topology.md#unit-disk) causes geometric amplification as $n\sim T/h$ increases; a repeated [unit-circle root](../../../polynomial.md#unit-circle-root) permits polynomial growth in $n$. Either can destroy convergence even for starting perturbations tending to zero.

The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) states that, for a fixed-coefficient method and a well-posed [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) with a suitably [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) right-hand side, [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) and [zero-stability](../../../numerical-analysis.md#zero-stability) are equivalent to convergence for all convergent starting data. If the starting errors are $O(h^p)$ and the exact solution is sufficiently smooth, the global error is $O(h^p)$ on a fixed time interval. A stability estimate bounds the propagated sum of $O(h^{p+1})$ local defects over $O(1/h)$ steps; the [discrete Gronwall inequality](../../../probability-and-statistics.md#discrete-gronwall-inequality) controls the dependence of $f$ on the accumulated error. Implicit methods also require the locally consistent, uniquely solvable update branch for sufficiently small $h$.

For example, the [explicit Euler method](../../../numerical-analysis.md#euler-method) has order one and $\rho(\zeta)=\zeta-1$, satisfying the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method). The two-step [Adams-Bashforth method](../../../numerical-analysis.md#adams-bashforth-method) has order two and $\rho(\zeta)=\zeta(\zeta-1)$, again satisfying it. The [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule) has order two with one step. The two-step [Simpson multistep method](../../../numerical-analysis.md#simpson-multistep-method), $Y_{n+2}-Y_n=h(f_{n+2}+4f_{n+1}+f_n)/3$, has order four and the simple roots $1,-1$: it is [zero-stable](../../../numerical-analysis.md#zero-stability), although its [parasitic amplification root](../../../numerical-analysis.md#parasitic-amplification-root) can spoil long-time decay. These examples distinguish finite-time [numerical convergence](../../../numerical-analysis.md#convergence-of-a-numerical-method) from [absolute stability](../../../numerical-analysis.md#linear-stability-domain).

The [first Dahlquist barrier](../../../numerical-analysis.md#first-dahlquist-barrier) gives the maximum possible order of a convergent ordinary real $k$-step method:

$$
\boxed{p\le\begin{cases}k+1,&k\text{ odd},\\k+2,&k\text{ even},\end{cases}\qquad p\le k\text{ for an explicit method}.}
$$

These bounds assume only first-derivative evaluations, fixed coefficients and [zero-stability](../../../numerical-analysis.md#zero-stability); the sixth-order [multiderivative multistep method](../../../numerical-analysis.md#multiderivative-multistep-method) in [solution](#5/a/solution) is outside that class.

To obtain arbitrarily high convergent order within the ordinary class, increase the number of steps. The [Adams-Bashforth method](../../../numerical-analysis.md#adams-bashforth-method) integrates a [polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) of $k$ past derivative values and has order $k$. The [Adams–Moulton method](../../../numerical-analysis.md#adams-moulton-method) includes the new endpoint and has order $k+1$ for $k$ steps. In both families $\rho(\zeta)=\zeta^{k-1}(\zeta-1)$, so the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) holds for every fixed $k$. Starting values can be generated by a [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) of sufficient accuracy. The [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula) instead differentiates an interpolating [polynomial](../../../polynomial.md); its order-$k$ members are [zero-stable](../../../numerical-analysis.md#zero-stability) only for $1\le k\le6$.

Finally, high order and favorable stiff stability are separate design goals. By the [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier), an ordinary [A-stable](../../../numerical-analysis.md#a-stability) [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) has order at most two. One may accept a smaller [linear stability domain](../../../numerical-analysis.md#linear-stability-domain), use suitable [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula) members for stiff problems, or switch to high-order implicit [Runge-Kutta methods](../../../numerical-analysis.md#runge-kutta-method) or [multiderivative multistep methods](../../../numerical-analysis.md#multiderivative-multistep-method). A convergent high-order formula still needs time steps appropriate to its stability properties and the problem's [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

## 7

↑ **Parent:** [Paper 69](paper-69.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

A spatial [finite difference method](../../../finite-difference.md#finite-difference-method) and time discretization for a linear evolution problem give a recurrence $U^{n+1}=B_{h,k}U^n$. To obtain [numerical stability](../../../numerical-analysis.md#stability-of-a-numerical-method) on $0\le nk\le T$, one needs a bound $\|B_{h,k}^n\|\le C_T$ uniform in the permitted grid sizes and time steps. More generally a growth estimate $\|B_{h,k}^n\|\le C e^{c nk}$ is sufficient. The [finite-time stability versus power boundedness](../../../finite-difference.md#finite-time-stability-versus-power-boundedness) distinction matters: growth per step of $1+O(k)$ can be compatible with the latter finite-time estimate, whereas unrestricted geometric growth at a fixed [Courant number](../../../finite-difference.md#courant-number) is not.

The eigenvalue method diagonalizes $B_{h,k}$ into modes. If $B_{h,k}$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix), the [spectral theorem](../../../hilbert-space.md#spectral-theorem) gives $\|B_{h,k}^n\|_2=\max_j|\mu_j|^n$. Thus $|\mu_j|\le1$ gives contraction, and $|\mu_j|\le e^{ck}$ gives the preceding growth estimate. A [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) $B=V\Lambda V^{-1}$ has $\|B^n\|_2\le\|V\|_2\|V^{-1}\|_2\max_j|\mu_j|^n$, so its [condition number](../../../linear-algebra.md#condition-number) must remain bounded uniformly as the mesh changes. A stable-looking list of [eigenvalues](../../../linear-operator-theory.md#eigenvalue) alone is insufficient.

Indeed,

$$
B=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad B^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}.
$$

Both [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are one, but the [Jordan block](../../../linear-operator-theory.md#jordan-block) gives growth proportional to $n\sim T/k$, violating uniform finite-time [numerical stability](../../../numerical-analysis.md#stability-of-a-numerical-method). A [nonnormal Fourier amplification matrix](../../../finite-difference.md#nonnormal-fourier-amplification-matrix) can similarly exhibit large amplification even with its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) inside the [unit disk](../../../geometry-and-topology.md#unit-disk). [Eigenvector](../../../linear-operator-theory.md#eigenvector) conditioning and the full powers of the amplification operator are essential.

For constant-coefficient schemes on a periodic or infinite grid, a [Fourier transform](../../../analysis.md#fourier-transform) diagonalizes scalar translation-invariant stencils. This yields [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis) using the [Fourier amplification symbol](../../../finite-difference.md#fourier-amplification-symbol) $G(\theta)$. The [discrete Parseval identity](../../../numerical-analysis.md#discrete-parseval-identity) turns a bound on $G(\theta)^n$ into a discrete [L2 norm](../../../real-analysis.md#l2-norm) estimate. For systems, the symbol is a [matrix](../../../vector-space.md#matrix); a [uniform power bound for matrix Fourier symbols](../../../finite-difference.md#uniform-power-bound-for-matrix-fourier-symbols) is required, rather than a bound on its [spectral radius](../../../analysis.md#spectral-radius) alone.

For the [heat equation](../../../diffusion-equation.md#heat-equation), a [central finite difference](../../../finite-difference.md#central-finite-difference) in space and the [explicit Euler method](../../../numerical-analysis.md#euler-method) in time give

$$
G(\theta)=1-4r\sin^2(\theta/2),\qquad r=k/h^2.
$$

The scalar condition $|G|\le1$ for every frequency is exactly **$0\le r\le1/2$**. With zero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), the spatial [matrix](../../../vector-space.md#matrix) is [symmetric](../../../set-theory.md#symmetric-relation) and diagonalized by sine modes, leading to the same uniform sufficient restriction. By contrast, the [Backward Euler diffusion scheme](../../../finite-difference.md#backward-euler-diffusion-scheme) has $G(\theta)=[1+4r\sin^2(\theta/2)]^{-1}$ and is stable for every $r\ge0$.

For the [advection equation](../../../partial-differential-equation.md#transport-equation) $u_t+a u_x=0$, $a>0$, centered space with the [explicit Euler method](../../../numerical-analysis.md#euler-method) gives $G=1-i\nu\sin\theta$, $\nu=ak/h$, and $|G|^2=1+\nu^2\sin^2\theta$. At fixed positive [Courant number](../../../finite-difference.md#courant-number), repeated powers are unbounded as the mesh is refined. The [upwind finite difference scheme](../../../finite-difference.md#upwind-finite-difference-scheme) instead has

$$
G=1-\nu+\nu e^{-i\theta},\qquad |G|^2=1-2\nu(1-\nu)(1-\cos\theta),
$$

which gives contraction precisely for **$0\le\nu\le1$**. This comparison shows why the spatial stencil and time method must be analyzed together.

Boundary treatment can destroy the normality or mode decomposition available on a periodic grid, so a finite-interval scheme needs its own uniform operator estimate. Multilevel time schemes likewise require the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) and uniform bounds for the associated amplification matrices; simple scalar root tests do not establish these bounds for arbitrary systems. Once [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method), a well-posed linear evolution problem and the required [numerical stability](../../../numerical-analysis.md#stability-of-a-numerical-method) estimate hold, the [Lax equivalence theorem](../../../finite-difference.md#lax-equivalence-theorem) gives [numerical convergence](../../../numerical-analysis.md#convergence-of-a-numerical-method). Eigenvalues provide a powerful route to that estimate when the accompanying eigenvector and boundary analysis is justified.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
