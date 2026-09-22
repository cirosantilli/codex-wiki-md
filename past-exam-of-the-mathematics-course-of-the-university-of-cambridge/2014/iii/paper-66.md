# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_66.pdf)

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
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
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

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take real $\kappa$ and use the [L2 norm](../../../real-analysis.md#l2-norm) on the spatial interval. Existence, uniqueness and continuous dependence are the three requirements of [Hadamard well-posedness](../../../inverse-problem.md#well-posed-problem). An [energy method](../../../numerical-analysis.md#energy-method) supplies the decisive estimate. For a smooth solution with homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\frac12\frac d{dt}\|u(t)\|_2^2
=\operatorname{Re}\int_0^1\overline u(u_{xx}+\kappa u_x)\,dx
=-\|u_x\|_2^2+\frac{\kappa}{2}[|u|^2]_0^1
=-\|u_x\|_2^2.
$$

The drift contributes only a boundary term, which vanishes. The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) $\|u_x\|_2^2\geq\pi^2\|u\|_2^2$ further gives

$$
\boxed{\|u(t)\|_2\leq e^{-\pi^2t}\|u(0)\|_2.}
$$

Apply the same argument to the difference of two solutions to obtain uniqueness and continuous dependence on the initial data.

For existence, use the [Dirichlet gauge transform for constant drift](../../../diffusion-equation.md#dirichlet-gauge-transform-for-constant-drift): $w=e^{\kappa x/2}u$ satisfies $w_t=w_{xx}-\kappa^2w/4$ with zero boundary values. Expanding $w_0$ in its [Fourier sine series](../../../fourier-series.md#fourier-sine-series) gives

$$
w(x,t)=\sum_{j=1}^{\infty}b_j
e^{-[(j\pi)^2+\kappa^2/4]t}\sin(j\pi x).
$$

For $u_0\in L^2(0,1)$ the series defines a solution continuous in $L^2$ down to $t=0$ and smooth for positive time; multiplication by the fixed bounded exponentials preserves this interpretation. Its energy estimate follows by approximation with smooth initial data. For a classical solution at the initial corners, require the usual smoothness and boundary compatibility instead. **The problem is well posed in $L^2$, with a contraction estimate independent of the initial data.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $d=\Delta x$, impose $u_0=u_{M+1}=0$, and write the [method of lines](../../../finite-difference.md#method-of-lines) system as $U'=LU$, where

$$
L=D_2+\kappa D_1,\qquad
D_2=d^{-2}\operatorname{tridiag}(1,-2,1),\quad
(D_1)_{m,m+1}=\frac1{2d},\quad(D_1)_{m+1,m}=-\frac1{2d}.
$$

Thus $D_2$ is a negative definite [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) and $D_1$ is a [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix). Use the mesh-weighted [Euclidean norm](../../../functional-analysis.md#euclidean-norm) $\|U\|_d^2=d\sum_{m=1}^M|u_m|^2$. Discrete [summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula) yields the [centered Dirichlet drift-diffusion energy identity](../../../numerical-analysis.md#centered-dirichlet-drift-diffusion-energy-identity)

$$
\frac12\frac d{dt}\|U\|_d^2
=d\operatorname{Re}(U^*LU)
=-\frac1d\sum_{m=0}^{M}|u_{m+1}-u_m|^2\leq0.
$$

Consequently

$$
\boxed{\|e^{tL}U^0\|_d\leq\|U^0\|_d,\qquad t\geq0.}
$$

The same estimate controls perturbations and is uniform in the number of grid points and in the fixed drift coefficient. Finite-dimensional linear ODE theory guarantees existence, so this proves [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) for the semidiscretization.

The factor $d^{1/2}$ simply rescales the vector norm and does not change the induced [matrix](../../../vector-space.md#matrix) norm. Equivalently the symmetric part is $(L+L^*)/2=D_2$, whose largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $-4d^{-2}\sin^2[\pi/(2(M+1))]<0$. This is the [Euclidean logarithmic norm](../../../continuous-dual-space.md#euclidean-logarithmic-norm), rather than generally the [spectral abscissa](../../../linear-operator-theory.md#spectral-abscissa) of a nonnormal [matrix](../../../vector-space.md#matrix). No periodic [Fourier mode](../../../fourier-analysis.md#fourier-mode) assumption has been made: the zero endpoint terms are part of the proof. In particular positivity of both off-diagonal coefficients is not needed for this $L^2$ stability result.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $k=\Delta t>0$ and retain the same [matrix](../../../vector-space.md#matrix) $L$. The [Crank-Nicolson method](../../../numerical-analysis.md#crank-nicolson-method) is

$$
U^{n+1}-U^n=\frac{k}{2}L(U^{n+1}+U^n).
$$

Take the real mesh-weighted inner product with $U^{n+1}+U^n$. The cross terms cancel, and the identity from part (b) gives

$$
\|U^{n+1}\|_d^2-\|U^n\|_d^2
=\frac{k}{2}\operatorname{Re}\langle L(U^{n+1}+U^n),U^{n+1}+U^n\rangle_d
\leq0.
$$

The implicit system is uniquely solvable: if $(I-kL/2)V=0$, then

$$
\|V\|_d^2=\frac{k}{2}\operatorname{Re}\langle LV,V\rangle_d\leq0,
$$

so $V=0$. Therefore its [dissipative Cayley-transform contraction](../../../functional-analysis.md#dissipative-cayley-transform-contraction) satisfies

$$
\boxed{\left\|\left(I-\frac{k}{2}L\right)^{-1}
\left(I+\frac{k}{2}L\right)\right\|_2\leq1.}
$$

Iterating proves **unconditional stability for every $\mu=k/d^2>0$**; the perturbation bound is one and does not depend on the mesh or time-step ratio.

The printed hint's exponential estimate is valid with the logarithmic norm, but its proposed bound by $r(k\alpha[L])$ is not a general inheritance principle. For the trapezoidal [stability function](../../../numerical-analysis.md#stability-function) $r(z)=(1+z/2)/(1-z/2)$, that real number can even be negative when $k\alpha[L]<-2$, whereas a norm is nonnegative. The direct energy proof above establishes the required result without that assertion.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) are

$$
\rho(\zeta)=\zeta^2-(1+a)\zeta+a=(\zeta-1)(\zeta-a),\qquad
\sigma(\zeta)=\frac{1-3a}{2}\zeta+\frac{1+a}{2}\zeta^2.
$$

To determine formal order, substitute a smooth exact solution and expand about the first time level. The [exponential-symbol order criterion for a multistep method](../../../numerical-analysis.md#exponential-symbol-order-criterion-for-a-multistep-method) collects precisely the same coefficients:

$$
\rho(e^z)-z\sigma(e^z)
=-\frac{1+5a}{12}z^3-\frac{3+11a}{24}z^4+O(z^5).
$$

The constant, linear and quadratic coefficients vanish for every $a$. The cubic coefficient vanishes only at $a=-1/5$, where the quartic coefficient is $-1/30\ne0$. Hence

$$
\boxed{p=3\text{ if }a=-\tfrac15,\qquad p=2\text{ otherwise}.}
$$

Here order means the exact-solution step residual is $O(h^{p+1})$. It is a formal consistency result, not a convergence assertion. In particular at $a=1$ both $\rho'(1)$ and $\sigma(1)$ vanish, and the double root at one destroys [zero-stability](../../../numerical-analysis.md#zero-stability); cancelling its common factor gives a different, first-order recurrence with an additional integration constant left unspecified by the original formula.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) states that a consistent [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) is convergent for suitably consistent starting values exactly when it is [zero-stable](../../../numerical-analysis.md#zero-stability). The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) requires every root of $\rho$ to lie in the closed unit disk, with every unit-modulus root simple.

The roots are $1$ and $a$. Thus $|a|\leq1$ is necessary; $a=1$ is excluded because it gives a double root at one. At $a=-1$, the two unit roots are distinct, so the endpoint is allowed. Combined with part (a), this proves

$$
\boxed{-1\leq a<1\quad\text{for convergence}.}
$$

Assume a locally Lipschitz vector field, a smooth solution on the fixed time interval, a nearby solvable implicit branch and starting errors of the required order. The global order is three at $a=-1/5$ and two at the other convergent parameter values. Outside this interval, zero-step perturbations already grow through either an exterior root or a unit-root polynomial factor.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the standard [A-stability](../../../numerical-analysis.md#a-stability) convention including the root condition at $z=h\lambda=0$. The [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) is

$$
P_z(\zeta)=\left(1-\frac{1+a}{2}z\right)\zeta^2
-\left(1+a+\frac{1-3a}{2}z\right)\zeta+a.
$$

[Zero-stability](../../../numerical-analysis.md#zero-stability) first restricts the possible parameters to $-1\leq a<1$. For $-1<a<0$, as $z$ tends to negative infinity, one amplification root tends to $(3a-1)/(1+a)$, whose modulus exceeds one. For $a=-1$, the characteristic equation is $\zeta^2-2z\zeta-1=0$; large negative real $z$ likewise gives an exterior root. Thus $a\geq0$ is necessary.

For sufficiency take $0\leq a<1$. The leading coefficient cannot vanish in the closed left half-plane. On the unit circle $\zeta=e^{i\theta}$ the [boundary-locus test for multistep A-stability](../../../numerical-analysis.md#boundary-locus-test-for-multistep-a-stability) uses $z=\rho(\zeta)/\sigma(\zeta)$ and gives

$$
\operatorname{Re}z
=\frac{4a(1+a)(1-\cos\theta)^2}
{|1-3a+(1+a)e^{i\theta}|^2}\geq0
$$

where the denominator is nonzero. When $a=0$, the exceptional zero of $\sigma$ at $\zeta=-1$ is not a zero of $\rho$ and therefore cannot be an amplification root for a finite $z$. Near $z=0$ on the negative real axis, the root issuing from one is $1+z+O(z^2)$ and is strictly inside the disk; the other root is close to $a$ and is also inside. Roots vary continuously, cannot escape through infinity because the leading coefficient is nonzero, and cannot cross the unit circle anywhere in the open left half-plane by the displayed boundary formula. Thus every root remains inside there. Continuity gives the boundary case; for $a>0$ a unit root on the imaginary axis can occur only at $z=0$, where it is simple. For $a=0$, cancellation of the harmless zero root leaves the [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule), whose amplification factor has modulus at most one.

Therefore

$$
\boxed{0\leq a<1\quad\text{for A-stability}.}
$$

The third-order member is convergent but not [A-stable](../../../numerical-analysis.md#a-stability), consistent with the [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier). At $a=1$, $P_z=(\zeta-1)[(1-z)\zeta-1]$ has a permanent unit root and a double root at $z=0$: the unreduced method is not [zero-stable](../../../numerical-analysis.md#zero-stability) and is not [A-stable](../../../numerical-analysis.md#a-stability) under the stated convention. Testing only the open half-plane while overlooking its zero-step behavior would give a weaker conclusion.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $p$ be the collocation polynomial of degree at most $s$ over one step, with $p(t_n)=y_n$, and let $Y_i=p(t_n+c_ih)$. Its derivative, of degree at most $s-1$, is fixed by its values at the distinct nodes. [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) therefore gives

$$
p'(t_n+h\tau)=\sum_{j=1}^s\ell_j(\tau)f(t_n+c_jh,Y_j).
$$

Integrating from zero to $\tau$ yields

$$
p(t_n+h\tau)=y_n+h\sum_{j=1}^s
\left(\int_0^\tau\ell_j(v)\,dv\right)f(t_n+c_jh,Y_j).
$$

At $\tau=c_i$ this gives the stage equations of an [implicit Runge-Kutta method](../../../numerical-analysis.md#implicit-runge-kutta-method); at $\tau=1$ it gives the update. Consequently

$$
\boxed{a_{ij}=\int_0^{c_i}\ell_j(v)\,dv,\qquad
b_j=\int_0^1\ell_j(v)\,dv.}
$$

Conversely, stages satisfying these equations define the integrated polynomial displayed above. It takes the stage values at the nodes and has the required derivative there, so it solves the collocation equations. This proves equivalence for every common solution branch, not merely equality on the scalar test equation. Also $\sum_ja_{ij}=c_i$, since the Lagrange polynomials sum to one. Stage existence or uniqueness requires the usual implicit-solvability assumptions; for a Lipschitz vector field a sufficiently small step gives a contraction. This is the [collocation Runge-Kutta method](../../../numerical-analysis.md#collocation-runge-kutta-method) construction.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) polynomials for these nodes are

$$
\ell_1(\tau)=2\tau^2-3\tau+1,\qquad
\ell_2(\tau)=4\tau-4\tau^2,\qquad
\ell_3(\tau)=2\tau^2-\tau.
$$

Their integrals give the [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method) tableau

$$
\boxed{\begin{array}{c|ccc}
0&0&0&0\\
1/2&5/24&1/3&-1/24\\
1&1/6&2/3&1/6\\ \hline
&1/6&2/3&1/6
\end{array}.}
$$

To verify its nonlinear order, not just its scalar linear order, set $e=(1,1,1)^T$, $c=Ae$ and $C=\operatorname{diag}(c)$. Direct multiplication verifies the [fourth-order conditions for a Runge-Kutta method](../../../numerical-analysis.md#fourth-order-conditions-for-a-runge-kutta-method):

$$
b^Te=1,\quad b^Tc=\frac12,\quad b^Tc^2=\frac13,\quad
b^TAc=\frac16,\quad b^Tc^3=\frac14,\quad
b^TCAc=\frac18,\quad b^TAc^2=\frac1{12},\quad
b^TA^2c=\frac1{24}.
$$

Powers of $c$ are componentwise. These eight [Butcher order conditions](../../../numerical-analysis.md#butcher-order-condition) establish order at least four for general smooth ODEs. On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), elimination of the stages gives

$$
R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12},\qquad
R(z)-e^z=-\frac{z^5}{720}+O(z^6).
$$

A nonzero fifth-order step defect rules out order five. Thus **the method has exactly order four**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write $P(z)=1+z/2+z^2/12$ and $Q(z)=1-z/2+z^2/12$. The zeros of $Q$ are $3\pm i\sqrt3$, so the [stability function](../../../numerical-analysis.md#stability-function) has no pole in the closed left half-plane. A direct modulus calculation gives

$$
|Q(z)|^2-|P(z)|^2
=-2\operatorname{Re}z\left(1+\frac{|z|^2}{12}\right).
$$

For $\operatorname{Re}z\leq0$ this is nonnegative, and hence $|R(z)|=|P/Q|\leq1$. Therefore **the [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method) is [A-stable](../../../numerical-analysis.md#a-stability)**. It is not [L-stable](../../../numerical-analysis.md#l-stability), because $R(z)\to1$ for large negative real $z$; unconditional scalar stability need not strongly damp the stiffest modes.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

By [orthogonal diagonalization of a real symmetric matrix](../../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix), write $A=Q\operatorname{diag}(\lambda_1,\ldots,\lambda_d)Q^T$, with orthogonal $Q$. Its [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) has the same eigenvectors and positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $e^{t\lambda_j}$. Orthogonal invariance of the induced [Euclidean norm](../../../functional-analysis.md#euclidean-norm) gives the exact identity

$$
\boxed{\|e^{tA}\|_2=\max_j e^{t\lambda_j}
=e^{t\lambda_{\max}(A)},\qquad t\geq0.}
$$

This proves the requested inequality with equality. If a real number $\beta$ gave the bound for every $t\geq0$, evaluating on a unit eigenvector for $\lambda_{\max}(A)$ at any $t>0$ would give $e^{t\lambda_{\max}}\leq e^{t\beta}$, so $\beta\geq\lambda_{\max}$. Thus **the stated exponent is the smallest possible**. For a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) the [spectral abscissa](../../../linear-operator-theory.md#spectral-abscissa) and [Euclidean logarithmic norm](../../../continuous-dual-space.md#euclidean-logarithmic-norm) coincide, unlike the general nonsymmetric case in Question 1.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set $S=A+B$ and $E(t)=F(t)-e^{tS}$. Since $F(0)=I$, $E(0)=0$. Differentiate the ordered exponential products, using that each [matrix](../../../vector-space.md#matrix) commutes with its own exponential:

$$
F'(t)-SF(t)
=\frac12\left\{[e^{tB},A]e^{tA}+[e^{tA},B]e^{tB}\right\}
=:D(t).
$$

Here the [commutator](../../../lie-algebra.md#commutator) convention is $[X,Y]=XY-YX$; this fixes both signs. The error satisfies $E'=SE+D$, so the [variation-of-constants formula](../../../functional-analysis.md#variation-of-constants-formula) gives

$$
\boxed{E(t)=\frac12\int_0^t e^{(t-x)S}
\left\{[e^{xB},A]e^{xA}+[e^{xA},B]e^{xB}\right\}\,dx.}
$$

This is the [symmetrized exponential-splitting defect identity](../../../numerical-analysis.md#symmetrized-exponential-splitting-defect-identity). Symmetry of $A,B$ was not needed for the identity itself; it will be used to bound their exponentials in part (c).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $\beta=\mu[A]+\mu[B]$ and $\gamma=\mu[A+B]$, where all three [matrices](../../../vector-space.md#matrix) are symmetric. Submultiplicativity and the triangle inequality give

$$
\|[e^{xB},A]e^{xA}\|_2
\leq2\|A\|_2e^{x(\mu[A]+\mu[B])},
$$

and similarly the other [commutator](../../../lie-algebra.md#commutator) term is bounded by $2\|B\|_2e^{x\beta}$. Apply part (a) also to $A+B$ in the integral from part (b). The outer factor one-half cancels these twos, leaving

$$
\|F(t)-e^{t(A+B)}\|_2
\leq(\|A\|_2+\|B\|_2)\int_0^t e^{(t-x)\gamma+x\beta}\,dx.
$$

The [exponential divided difference](../../../numerical-analysis.md#exponential-divided-difference) evaluates this integral. Thus

$$
\boxed{\|F(t)-e^{t(A+B)}\|_2\leq
(\|A\|_2+\|B\|_2)
\frac{e^{t\beta}-e^{t\gamma}}{\beta-\gamma}}
$$

when $\beta\ne\gamma$, and

$$
\boxed{\|F(t)-e^{t(A+B)}\|_2\leq
(\|A\|_2+\|B\|_2)\,te^{t\gamma}}
$$

when they coincide. The second expression is both the direct equal-exponent integral and the continuous limit of the first. The [Rayleigh-Ritz variational principle](../../../linear-operator-theory.md#rayleigh-ritz-variational-principle) also gives $\gamma\leq\beta$, although the integral computation does not require a strict inequality. These are valid coarse norm bounds; the cancellation between the two products can make the actual small-step error substantially smaller.

## 5

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a smooth exact solution of the [advection equation](../../../partial-differential-equation.md#transport-equation), $u(x,t)=g(x+t)$, since the transport velocity in the convention $u_t=u_x$ is minus one. Put $d=\Delta x$, $k=\mu d$ and move the scheme's right side to the left. Substitution gives the exact-solution residual

$$
\mathcal R=g(s+k)-g(s+d-k)
-(2\mu-1)[g(s+d)-g(s)],\qquad s=x+t.
$$

Its constant, linear and quadratic [Taylor expansion](../../../calculus.md#taylor-expansion) terms cancel. The cubic term is

$$
\mathcal R
=\frac{d^3}{6}\mu(2\mu-1)(\mu-1)g^{(3)}(s)+O(d^4).
$$

The un-substituted leading term is $2k(u_t-u_x)$, so divide by $2k$ to use a normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error). For a fixed positive Courant ratio,

$$
\boxed{\frac{\mathcal R}{2k}
=\frac{d^2}{12}(2\mu-1)(\mu-1)u_{xxx}+O(d^3).}
$$

Thus **the generic method is second order**, provided stability and a compatible second-order starter are supplied.

There are two special ratios rather than an unnoticed higher generic order. At $\mu=1/2$, the scheme is $u_m^{n+1}=u_{m+1}^{n-1}$; both sides lie on the same exact characteristic, and the residual vanishes identically. At $\mu=1$ the previous-level term cancels the unshifted current term for exact data, again producing zero residual on every exact characteristic solution. The first special case is stable, while the second is not stable for arbitrary two-level perturbations, as part (b) shows. **Exact propagation of specially initialized data is not a substitute for stability.**

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use the [Fourier transform](../../../analysis.md#fourier-transform) for the spatial [Cauchy problem](../../../partial-differential-equation.md#cauchy-problem), or its periodic analogue, and regard the two starting levels as independently perturbed data. A [Fourier mode](../../../fourier-analysis.md#fourier-mode) with spatial factor $e^{im\theta}$ has amplification roots $G$ satisfying

$$
G^2-(2\mu-1)(e^{i\theta}-1)G-e^{i\theta}=0.
$$

Put $c=2\mu-1$ and $G=e^{i\theta/2}q$. Then

$$
q^2-2ic\sin(\theta/2)q-1=0,\qquad
q_\pm=ic\sin(\theta/2)\pm
\sqrt{1-c^2\sin^2(\theta/2)}.
$$

If $|c|<1$, both roots have modulus one and their separation is bounded below uniformly in frequency:

$$
|G_+-G_-|\geq2\sqrt{1-c^2}>0.
$$

The [uniform power bound from separated amplification roots](../../../finite-difference.md#uniform-power-bound-from-separated-amplification-roots) now controls the two-level companion [matrix](../../../vector-space.md#matrix) for every time step. Its entries are uniformly bounded, and its eigenvector conditioning is bounded by the reciprocal root gap. The [Parseval identity](../../../fourier-analysis.md#parseval-identity) transfers this frequency-uniform bound to the spatial $\ell^2$ norm. This proves stability, rather than merely checking each root's modulus.

If $|c|>1$, the frequency $\theta=\pi$ has a root outside the unit disk, so there is exponential instability. If $|c|=1$, the two roots at $\theta=\pi$ coincide on the unit circle. The companion [matrix](../../../vector-space.md#matrix) is not a scalar [matrix](../../../vector-space.md#matrix) and has a nontrivial [Jordan block](../../../linear-operator-theory.md#jordan-block); its powers grow linearly in the number of steps. Frequencies arbitrarily near that value produce the same lack of a uniform bound for localized Fourier packets, so this also invalidates Cauchy $\ell^2$ stability, not only periodic plane-wave stability. At $\mu=1$ the double amplification root is $-1$, and at $\mu=0$ it is $1$.

Therefore the full two-level stability range for a fixed positive Courant ratio is

$$
\boxed{0<\mu<1.}
$$

The endpoint $\mu=0$ is moreover not a positive time step. Bounds deteriorate as $\mu$ approaches either endpoint; the displayed range is not a uniform claim over ratios arbitrarily close to one. A prescribed starter that removes one special parasitic component can change behavior for selected initial data, but does not establish the requested unrestricted two-level stability.

## 6

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [stiff differential equation](../../../numerical-analysis.md#stiff-equation) can contain rapidly decaying modes as well as a slowly changing solution of interest. An explicit scheme may need a very small step solely to keep those already small fast modes from numerical growth. [A-stability](../../../numerical-analysis.md#a-stability) addresses this restriction through the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$, whose exact solution decays when $\operatorname{Re}\lambda<0$.

For a one-step method, write $y_{n+1}=R(z)y_n$, $z=h\lambda$. Its [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) consists of the points where the update is defined and $|R(z)|\leq1$. **[A-stability](../../../numerical-analysis.md#a-stability) means that this domain contains the closed left half-plane.** This is a scalar linear stability property, not an order condition, an existence theorem for an implicit solve, or a general nonlinear contractivity assertion.

For a rational approximation to the exponential, consistency requires $R(z)=1+z+O(z^2)$, and order $p$ requires $R(z)-e^z=O(z^{p+1})$. Poles must be absent from the relevant half-plane. The [Forward Euler method](../../../numerical-analysis.md#euler-method) has $R=1+z$ and the disk $|1+z|\leq1$, so negative real modes require $h|\lambda|\leq2$; it is not [A-stable](../../../numerical-analysis.md#a-stability). The [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $R=(1-z)^{-1}$, and $|1-z|\geq1$ on the left half-plane, so it is [A-stable](../../../numerical-analysis.md#a-stability). The [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule) and the [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) both have, on the scalar linear problem,

$$
R(z)=\frac{1+z/2}{1-z/2},\qquad
|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z.
$$

They are second-order and [A-stable](../../../numerical-analysis.md#a-stability) despite being different nonlinear methods. No nonconstant polynomial approximation is [A-stable](../../../numerical-analysis.md#a-stability), because its modulus grows without bound on the negative real axis. In particular every nontrivial explicit [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) has a bounded-step stability restriction.

[A-stability](../../../numerical-analysis.md#a-stability) prevents growth but need not eliminate extremely stiff modes: the trapezoidal factor tends to minus one as $z\to-\infty$. [L-stability](../../../numerical-analysis.md#l-stability) additionally requires $R(z)\to0$ within the left half-plane. Backward Euler is [L-stable](../../../numerical-analysis.md#l-stability); trapezoidal and implicit midpoint are not. The distinction explains persistent alternating transients in otherwise stable Crank-Nicolson calculations. Accuracy still constrains useful step sizes even for an [A-stable](../../../numerical-analysis.md#a-stability) method.

A [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) is characterized by polynomials $\rho,\sigma$, and its scalar modes satisfy $\rho(\zeta)-z\sigma(\zeta)=0$. There is generally no single scalar amplification factor: every root must lie in the closed unit disk and unit roots must be simple. At $z=0$, this is the [zero-stability](../../../numerical-analysis.md#zero-stability) root condition. Consistency plus [zero-stability](../../../numerical-analysis.md#zero-stability) gives convergence by the [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem), with suitable starting values. [A-stability](../../../numerical-analysis.md#a-stability) demands the amplification root condition throughout the left half-plane, including the zero-step condition. The [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier) says that an irreducible [A-stable](../../../numerical-analysis.md#a-stability) [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) has order at most two, and an explicit [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) cannot be [A-stable](../../../numerical-analysis.md#a-stability).

Examples include backward Euler, trapezoidal, and the second-order [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula)

$$
3y_{n+2}-4y_{n+1}+y_n=2hf(y_{n+2}).
$$

Its zero-step roots are $1,1/3$. Its unit-circle boundary quotient has real part $(1-\cos\theta)^2\geq0$, and the leading coefficient is nonzero on the left half-plane, giving [A-stability](../../../numerical-analysis.md#a-stability) by the same continuation argument as in Question 2. Conversely the third-order member of that question fails [A-stability](../../../numerical-analysis.md#a-stability). A formal high order without [zero-stability](../../../numerical-analysis.md#zero-stability), or after silently cancelling a problematic unit factor, does not evade the barrier.

For an [implicit Runge-Kutta method](../../../numerical-analysis.md#implicit-runge-kutta-method), the stages on the test equation satisfy $Y=e\,y_n+zAY$. Whenever these stages are solvable, its [stability function](../../../numerical-analysis.md#stability-function) is

$$
\boxed{R(z)=1+z\,b^T(I-zA)^{-1}e.}
$$

This rational function is used to test scalar [A-stability](../../../numerical-analysis.md#a-stability); the [Butcher order conditions](../../../numerical-analysis.md#butcher-order-condition) separately establish nonlinear order. The [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method) in Question 3 is an [A-stable](../../../numerical-analysis.md#a-stability) fourth-order example with $R$ the diagonal degree-two Padé approximant. More generally the $s$-stage [Gauss--Legendre Runge-Kutta method](../../../numerical-analysis.md#gauss-legendre-method) has order $2s$ and is [A-stable](../../../numerical-analysis.md#a-stability), with the diagonal Padé approximation to $e^z$; its stiff-limit factor is nonzero. The $s$-stage [Radau IIA method](../../../numerical-analysis.md#radau-iia-method) has order $2s-1$ and is [L-stable](../../../numerical-analysis.md#l-stability). Thus Runge-Kutta stages permit arbitrarily high [A-stable](../../../numerical-analysis.md#a-stability) order, unlike irreducible linear multistep formulas.

For a [normal matrix](../../../linear-operator-theory.md#normal-matrix), scalar amplification bounds transfer through unitary diagonalization. For a [non-normal matrix](../../../linear-operator-theory.md#non-normal-matrix), [eigenvalue](../../../linear-operator-theory.md#eigenvalue) information alone does not assert Euclidean contraction: transient growth and eigenvector conditioning can matter. Direct [energy method](../../../numerical-analysis.md#energy-method) arguments, such as the dissipative Cayley-transform proof in Question 1, use the symmetric part and are more informative in that setting.

For nonlinear dissipative vector fields, the stronger [B-stability](../../../numerical-analysis.md#b-stability) property asks that distances between two numerical solutions not increase. A standard sufficient condition for [Runge-Kutta methods](../../../numerical-analysis.md#runge-kutta-method) is [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method): $b_i\geq0$ and

$$
(b_i a_{ij}+b_j a_{ji}-b_i b_j)_{ij}
$$

is positive semidefinite. It follows from the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity) when the implicit stages exist. The three-stage Lobatto IIIA method is [A-stable](../../../numerical-analysis.md#a-stability) but has the first diagonal entry of that [matrix](../../../vector-space.md#matrix) equal to $-1/36$, so scalar [A-stability](../../../numerical-analysis.md#a-stability) should not be confused with that sufficient nonlinear condition. [Stage solvability of an implicit Runge-Kutta method](../../../numerical-analysis.md#stage-solvability-of-an-implicit-runge-kutta-method) remains a separate issue and computational cost of the implicit equations must be considered. **[A-stability](../../../numerical-analysis.md#a-stability) removes a scalar decay-mode stability restriction; order, stiff damping, nonlinear stability and solvability remain distinct properties.**

## 7

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

The [finite element method](../../../numerical-analysis.md#finite-element-method) replaces an infinite-dimensional variational problem by a finite-dimensional one, usually using functions that are polynomial on small mesh elements. [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) and [Galerkin method](../../../partial-differential-equation.md#galerkin-method) describe how the discrete equations are selected; neither intrinsically requires piecewise polynomials, though those spaces make assembly local and sparse.

For a concrete realization of the two-point problem, choose homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) at both endpoints of $(0,1)$. The differential expression alone is not a complete boundary value problem, so this boundary choice is an explicit assumption. Let $p\in W^{1,\infty}$ with $p\geq p_0>0$, $q\in L^\infty$ with $q\geq0$, and $f\in L^2$. Use the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) $V=H_0^1(0,1)$ with norm $\|v\|_V=\|v'\|_2$. By the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) this is equivalent to its full first-order Sobolev norm. Multiplying by a test function and applying [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
a(u,v)=\ell(v)\quad(v\in V),\qquad
a(u,v)=\int_0^1(pu'v'+quv)\,dx,\quad
\ell(v)=\int_0^1fv\,dx.
$$

The endpoint terms vanish by the essential boundary condition. The form is a [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form), bounded by

$$
|a(u,v)|\leq M\|u\|_V\|v\|_V,\qquad
M=\|p\|_\infty+C_P^2\|q\|_\infty,
$$

and it is a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form):

$$
a(v,v)\geq p_0\|v\|_V^2.
$$

The load is a bounded linear functional. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) gives a unique weak solution and a bound $\|u\|_V\leq\|\ell\|_{V^*}/p_0$. Under the stated coefficient regularity it solves the differential equation in the usual weak sense.

The [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) minimizes the energy

$$
J(v)=\tfrac12a(v,v)-\ell(v)
$$

over $V$, or over a conforming finite-dimensional subspace $V_h\subset V$. Its first variation is $a(v,w)-\ell(w)$; symmetry and coercivity make the functional strictly convex. In fact, if $u$ is the weak solution,

$$
J(v)-J(u)=\tfrac12a(v-u,v-u)\geq0.
$$

Thus the energy minimizer is exactly the weak solution. The [Galerkin method](../../../partial-differential-equation.md#galerkin-method) instead directly asks for $u_h\in V_h$ with $a(u_h,v_h)=\ell(v_h)$ for all $v_h\in V_h$. For this symmetric coercive problem, [Ritz-Galerkin equivalence for a symmetric coercive form](../../../numerical-analysis.md#ritz-galerkin-equivalence-for-a-symmetric-coercive-form) shows that the discrete minimizer and Galerkin solution coincide. For a nonsymmetric problem, a Galerkin formulation can still apply but the same quadratic minimization generally cannot represent its full [bilinear form](../../../linear-algebra.md#bilinear-form); appropriate coercivity or inf-sup conditions must then justify the chosen spaces.

Subtract the continuous and discrete weak equations to obtain [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality) $a(u-u_h,v_h)=0$. Since $a$ defines the [energy norm](../../../numerical-analysis.md#energy-norm) $\|v\|_a=\sqrt{a(v,v)}$, the [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2,
\qquad
\boxed{\|u-u_h\|_a=\inf_{v_h\in V_h}\|u-v_h\|_a.}
$$

In a general reference norm, the [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) yields

$$
\boxed{\|u-u_h\|_V\leq\frac{M}{p_0}
\inf_{v_h\in V_h}\|u-v_h\|_V.}
$$

The proof uses $a(e,e)=a(e,u-v_h)$ together with coercivity and continuity. Dense approximation spaces therefore imply convergence; the estimate reduces a numerical error problem to an approximation problem.

For implementation, partition the interval by nodes $0=x_0<\cdots<x_N=1$. Choose continuous piecewise-linear functions and the interior [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) $\phi_j$ as a basis, with the two boundary coefficients prescribed. Write $u_h=\sum_jU_j\phi_j$. The coefficients satisfy

$$
\boxed{KU=F,\qquad K_{ij}=\int_0^1(p\phi_j'\phi_i'+q\phi_j\phi_i)\,dx,
\quad F_i=\int_0^1f\phi_i\,dx.}
$$

The [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) is symmetric positive definite: $U^TKU=a(u_h,u_h)>0$ for nonzero interior coefficients. The local supports make it tridiagonal in this one-dimensional linear-element case.

On an element of length $h_e$, for constant element coefficients $p_e,q_e$, the two-node [matrix](../../../vector-space.md#matrix) and constant-load vector are

$$
K_e=\frac{p_e}{h_e}
\begin{pmatrix}1&-1\\-1&1\end{pmatrix}
+\frac{q_eh_e}{6}
\begin{pmatrix}2&1\\1&2\end{pmatrix},
\qquad
F_e=\frac{f_eh_e}{2}\begin{pmatrix}1\\1\end{pmatrix}.
$$

For variable coefficients, integrate $p,q,f$ against the same shape functions rather than silently replacing them by constants. Element contributions are added at shared nodes, and boundary values are eliminated or lifted into the right side. A sparse direct solve or a suitable iterative method gives the nodal coefficients. Numerical quadrature should preserve the required accuracy and, with positive coefficients and weights, the positive energy structure.

A [finite element interpolation estimate](../../../numerical-analysis.md#finite-element-interpolation-estimate) gives $\inf_{v_h}\|u-v_h\|_{H^1}\leq Ch\|u\|_{H^2}$ for these elements, where $h$ is the largest element size and the solution has the stated regularity. The [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) then gives **first-order energy error**. If the dual elliptic problem has $H^2$ regularity, the [Aubin–Nitsche duality argument](../../../numerical-analysis.md#aubin-nitsche-duality-argument) gives **second-order $L^2$ error**: for $e=u-u_h$, solve $a(v,z)=(e,v)_{L^2}$, then use $a(e,z)=a(e,z-I_hz)$ to gain one further factor of $h$. Higher-order elements improve rates when the solution is sufficiently smooth.

Nonzero Dirichlet data are handled by a boundary lifting and an affine trial space. [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) enter naturally through the integrated boundary term; Robin terms modify both the form and the load. With pure Neumann conditions and $q=0$, constants lie in the kernel: existence needs the load/flux compatibility condition, uniqueness needs a mean constraint, and the preceding Dirichlet coercivity argument cannot simply be reused. **Conforming approximation, boundary conditions and coercivity are the ingredients connecting the finite-element construction to a justified Ritz or Galerkin solution.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
