# Paper 72

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper72.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper72.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Multiply by a [test function](../../../distribution-theory.md#test-function) vanishing at the endpoints and apply [integration by parts](../../../calculus.md#integration-by-parts). The positive operator is $-u''+xu$, so the forcing changes sign. The [weak formulation](../../../partial-differential-equation.md#weak-formulation) of this [forced Airy boundary-value problem](../../../differential-equation.md#forced-airy-boundary-value-problem) is: find $u\in V=H_0^1(0,1)$ such that

$$
\boxed{a(u,v)=\ell(v)\quad(v\in V),\qquad
a(u,v)=\int_0^1(u'v'+xuv)\,dx,\quad
\ell(v)=-\int_0^1v\,dx.}
$$

Here $V$ is the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) and can be equipped with $\|v\|_V=\|v'\|_{L^2}$. The interval [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) states $\|v\|_{L^2}\leq\pi^{-1}\|v'\|_{L^2}$, so this [norm](../../../functional-analysis.md#norm) makes $V$ a [Hilbert space](../../../hilbert-space.md) and is equivalent to its usual $H^1$ [Sobolev norm](../../../sobolev-space.md#sobolev-norm). The form is symmetric and satisfies

$$
|a(u,v)|\leq(1+\pi^{-2})\|u\|_V\|v\|_V,\qquad
a(v,v)\geq\|v\|_V^2,\qquad
|\ell(v)|\leq\pi^{-1}\|v\|_V.
$$

The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) says that a bounded [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form) on a [Hilbert space](../../../hilbert-space.md) and a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) determine exactly one weak solution. All its hypotheses have just been verified. Moreover, $u''=xu+1\in L^2$ gives $u\in H^2$ on the interval; the right-hand side is then continuous, so this weak solution is the classical solution with the prescribed endpoint values.

Since the form is symmetric, the equivalent [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) minimizes

$$
\boxed{J(v)=\frac12\int_0^1[(v')^2+xv^2]\,dx+\int_0^1v\,dx
\quad\text{over }H_0^1(0,1).}
$$

Indeed, stationarity gives the weak equation and

$$
J(v)-J(u)=\tfrac12a(v-u,v-u)\geq0,
$$

with equality only at $u$. This proves the minimization equivalence, including the sign of the linear term.

Restricting to a [conforming finite element space](../../../numerical-analysis.md#conforming-finite-element-space) $V_h\subset V$ gives a unique discrete solution and [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality), $a(u-u_h,v_h)=0$ for every $v_h\in V_h$. The [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) states that if the continuity and coercivity constants are $M$ and $\alpha$, then $\|u-u_h\|_V\leq(M/\alpha)\inf_{v_h\in V_h}\|u-v_h\|_V$. For this symmetric problem the exact best-approximation constant in the [energy norm](../../../numerical-analysis.md#energy-norm) is one. The piecewise-linear [finite element interpolation estimate](../../../numerical-analysis.md#finite-element-interpolation-estimate) $\|u-I_hu\|_{H^1}\leq Ch\|u\|_{H^2}$ on regular [finite element meshes](../../../numerical-analysis.md#finite-element-mesh) therefore gives [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) of the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method), with first-order error in the [energy norm](../../../numerical-analysis.md#energy-norm).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Take a uniform [finite element mesh](../../../numerical-analysis.md#finite-element-mesh) $x_i=ih$, $0\leq i\leq J$, $h=1/J$, and interior [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) $\phi_i$. Write $u_h=\sum_{i=1}^{J-1}U_i\phi_i$. The [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) gives $KU=F$ with

$$
K_{ij}=\int_0^1\phi_i'\phi_j'\,dx+\int_0^1x\phi_i\phi_j\,dx,
\qquad F_i=-\int_0^1\phi_i\,dx=-h.
$$

The derivative part has diagonal $2/h$, neighboring entries $-1/h$ and zero other entries. For the [affine-weighted hat mass matrix](../../../numerical-analysis.md#affine-weighted-hat-mass-matrix), symmetry around $x_i$ gives

$$
\int x\phi_i^2\,dx=\frac{2h}{3}x_i.
$$

On $[x_i,x_{i+1}]$, the product of the two hats is symmetric about the midpoint, integrates to $h/6$, and therefore has weighted integral

$$
\int x\phi_i\phi_{i+1}\,dx=\frac h{12}(x_i+x_{i+1}).
$$

Consequently the explicit [tridiagonal](../../../vector-space.md#tridiagonal-matrix) equations are

$$
\boxed{\left[-\frac1h+\frac h{12}(x_{i-1}+x_i)\right]U_{i-1}
+\left[\frac2h+\frac{2h}3x_i\right]U_i
+\left[-\frac1h+\frac h{12}(x_i+x_{i+1})\right]U_{i+1}=-h,}
$$

for $1\leq i\leq J-1$, with $U_0=U_J=0$. The reaction coefficient has been integrated exactly; replacing it by an unweighted constant [mass matrix](../../../numerical-analysis.md#mass-matrix) would give a different system. For a nonzero coefficient [vector](../../../vector-space.md#vector), the represented function is nonzero and $U^TKU=a(u_h,u_h)>0$, so the [matrix](../../../vector-space.md#matrix) is symmetric [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) and the algebraic solution is unique.

Uniform spacing is a choice, not a requirement of the method. On a general [finite element mesh](../../../numerical-analysis.md#finite-element-mesh) with $h_i=x_i-x_{i-1}$, the corresponding entries are

$$
K_{ii}=\frac1{h_i}+\frac1{h_{i+1}}
+\frac{h_i}{12}(x_{i-1}+3x_i)
+\frac{h_{i+1}}{12}(3x_i+x_{i+1}),
$$



$$
K_{i,i+1}=-\frac1{h_{i+1}}+
\frac{h_{i+1}}{12}(x_i+x_{i+1}),\qquad
F_i=-\frac{h_i+h_{i+1}}2,
$$

with symmetric lower entries. These reduce to the displayed uniform-grid system.

## 2

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For this [two-step family with a third-order member](../../../numerical-analysis.md#two-step-family-with-a-third-order-member), use the [exponential-symbol order criterion for a multistep method](../../../numerical-analysis.md#exponential-symbol-order-criterion-for-a-multistep-method). Expanding the exact-solution residual symbol gives

$$
\rho(e^z)-z\sigma(e^z)
=-\frac{1+5a}{12}z^3-\frac{3+11a}{24}z^4+O(z^5).
$$

The constant, linear and quadratic coefficients vanish for every parameter. Thus

$$
\boxed{p=2\text{ for }a\ne-1/5,\qquad p=3\text{ for }a=-1/5.}
$$

At the exceptional value the fourth-degree coefficient is $-1/30$, so there is no further increase. This means an unscaled exact-solution residual of order $h^{p+1}$, or a residual divided by the step of order $h^p$.

The first characteristic [polynomial](../../../polynomial.md) factors as $\rho(w)=(w-1)(w-a)$. The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) requires every root to have modulus at most one and each unit-modulus root to be simple. The root $a=-1$ is allowed because it is distinct from the simple root one; $a=1$ is not, since it makes one a double root. Hence [zero-stability](../../../numerical-analysis.md#zero-stability) holds exactly for

$$
\boxed{-1\leq a<1.}
$$

On this interval, $\rho(1)=0$ and $\rho'(1)=\sigma(1)=1-a\ne0$ establish [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method). The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem), for a fixed-step consistent [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) applied to an [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) with a [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) right-hand side with convergent starting values and well-defined small-step updates, says that [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) is equivalent to [zero-stability](../../../numerical-analysis.md#zero-stability). Therefore the same interval is exactly the [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) range. With sufficiently accurate starting values the convergent members have the orders just computed.

At $a=1$ the [Taylor expansion](../../../calculus.md#taylor-expansion) still gives a formal order-two residual, but $\rho'(1)=\sigma(1)=0$ and the double root prevents a convergent method. Canceling the common factor $w-1$ produces the [common-factor cancellation defect in a multistep recurrence](../../../numerical-analysis.md#common-factor-cancellation-defect-in-a-multistep-recurrence) and changes the starting relations and cannot repair [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) of the original recurrence. At $a=0$, cancellation of a zero root instead reveals the ordinary [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule); it is consistent with the order-two result.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Apply the method to the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), put $z=h\lambda$, and retain every root of its [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method):

$$
P_z(w)=\left[1-\frac{1+a}{2}z\right]w^2
-\left[1+a+\frac{1-3a}{2}z\right]w+a.
$$

An [A-stable](../../../numerical-analysis.md#a-stability) convergent method must satisfy the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) for every $\operatorname{Re}z\leq0$.

First take $-1<a<0$. As negative real $z$ tends to minus infinity, one root tends to the nonzero root of $\sigma$,

$$
w_\infty=\frac{3a-1}{1+a},\qquad |w_\infty|>1.
$$

It follows by root continuity that some sufficiently negative finite $z$ is unstable. At $a=-1$, the recurrence has [polynomial](../../../polynomial.md) $w^2-2zw-1$; for any negative real $z$, its root $z-\sqrt{z^2+1}$ is below $-1$. Thus all negative convergent parameters are excluded.

For $0\leq a<1$, use the [boundary-locus test for multistep A-stability](../../../numerical-analysis.md#boundary-locus-test-for-multistep-a-stability). A unit root $w=e^{i\theta}$ with $\sigma(w)\ne0$ would require $z=\rho(w)/\sigma(w)$. Direct multiplication by the conjugate denominator gives

$$
\operatorname{Re}\frac{\rho(e^{i\theta})}{\sigma(e^{i\theta})}
=\frac{a(1+a)(1-\cos\theta)^2}{|\sigma(e^{i\theta})|^2}\geq0.
$$

There is therefore no unit-root crossing in the open left half-plane. The leading coefficient of $P_z$ never vanishes there, since its only zero is the positive real value $2/(1+a)$. For a small negative real $z$, the simple root initially at one moves to $1+z+O(z^2)$, inside the disk, and the other root is close to $a$, also inside. Continuity of [polynomial](../../../polynomial.md) roots and connectedness of the open left half-plane then keep both roots strictly inside throughout that half-plane. Possible zeros of $\sigma$ cause no omitted crossing: for $a>0$ its other root lies strictly inside the [unit disk](../../../geometry-and-topology.md#unit-disk), while at $a=0$ its unit-circle zero $w=-1$ has $\rho(-1)\ne0$.

On the imaginary axis, if $a>0$ the displayed real part vanishes only at $w=1$, which corresponds to $z=0$ and is simple. Other imaginary-axis parameters retain strictly interior roots. If $a=0$, the two roots are zero and the [stability function](../../../numerical-analysis.md#stability-function) $(1+z/2)/(1-z/2)$, whose modulus is one on that axis; the unit root is simple. Thus the required boundary [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) holds as well.

Combining necessity and sufficiency gives

$$
\boxed{\text{The convergent A-stable members are exactly }0\leq a<1.}
$$

In particular, the third-order member $a=-1/5$ is convergent but not [A-stable](../../../numerical-analysis.md#a-stability), in agreement with the [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier).

## 3

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $h=\Delta x$, $k=\Delta t$ and $\mu=k/h$. For the exact solution $u(x,t)=F(x+t)$ of the [advection equation](../../../partial-differential-equation.md#transport-equation), the three left-hand samples are translations by $(\mu-1)h$, $\mu h$ and $(\mu+1)h$ relative to $(x_m,t_n)$; the right-hand samples are translations by zero and $h$.

Denote their coefficients by $a=\mu(1+\mu)/6$, $b=(2-\mu)(1+\mu)/3$, $c=(2-\mu)(1-\mu)/6$, $d=(2-\mu)/3$ and $e=(1+\mu)/3$. [Taylor expansion](../../../calculus.md#taylor-expansion) compares moments

$$
M_j=a(\mu-1)^j+b\mu^j+c(\mu+1)^j-d\,0^j-e,
$$

where $0^0=1$ in the zeroth moment. Direct calculation gives

$$
M_0=M_1=M_2=M_3=0,\qquad
M_4=\frac{\mu(\mu-2)(\mu-1)(\mu+1)}3.
$$

Thus the unscaled exact-solution residual is

$$
\mathcal R_h=\frac{h^4}{72}\mu(\mu-2)(\mu-1)(\mu+1)u_{xxxx}+O(h^5).
$$

For fixed nonzero $\mu$, dividing by the time step yields

$$
\boxed{\frac{\mathcal R_h}{k}
=\frac{h^3}{72}(\mu-2)(\mu-1)(\mu+1)u_{xxxx}+O(h^4).}
$$

The scheme is therefore **third order under fixed-Courant refinement**, with an unscaled one-step defect of order four. Stability then gives third-order accumulated error for smooth data with [periodic boundary conditions](../../../differential-equation.md#periodic-boundary-conditions). Calling the unscaled defect fourth order is a different convention, not fourth-order approximation of the differential equation.

At $\mu=-1,1,2$, the amplification factor in (b) becomes exactly $e^{i\mu\theta}$: the numerical step translates the grid data by that integer number of cells and is exact for this constant-speed [advection equation](../../../partial-differential-equation.md#transport-equation). At $\mu=0$ it is the identity, a zero-time-step limit. These are exact special shifts, rather than merely a cancellation of one term of the [Taylor expansion](../../../calculus.md#taylor-expansion). This is the [implicit advection scheme with exact integer shifts](../../../finite-difference.md#implicit-advection-scheme-with-exact-integer-shifts).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose a spatial interval with [periodic boundary conditions](../../../differential-equation.md#periodic-boundary-conditions) and a uniform grid, so no separate inflow [boundary closure of a difference scheme](../../../finite-difference.md#boundary-closure-of-a-difference-scheme) is required. The [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform) is a [unitary operator](../../../vector-space.md#unitary-operator) in the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm). Every circulant stencil is diagonal in that transform, and a one-step [Fourier multiplier](../../../analysis.md#fourier-multiplier) is a contraction exactly when its modulus is at most one for every grid frequency. For a mesh-uniform statement, use all $\theta\in[-\pi,\pi]$, the limiting frequency range.

A [Fourier mode](../../../fourier-analysis.md#fourier-mode) $e^{im\theta}$ gives

$$
G(\theta)=\frac{N(\theta)}{D(\theta)},\qquad
N=d+ee^{i\theta},\qquad D=ae^{-i\theta}+b+ce^{i\theta},
$$

with the coefficients from (a). Squaring moduli and putting $v=\cos\theta$ yields

$$
\boxed{|D|^2-|N|^2
=\frac{\mu(\mu-2)(\mu-1)(\mu+1)}9(1-\cos\theta)^2.}
$$

This has the required nonnegative sign for every frequency exactly when

$$
\boxed{\mu\in(-\infty,-1]\cup[0,1]\cup[2,\infty).}
$$

One must also check that the implicit equation is solvable, rather than divide by a vanishing symbol. Here

$$
\operatorname{Im}D=\frac{1-2\mu}{3}\sin\theta,\qquad D(0)=1,
\qquad D(\pi)=\frac{1+2\mu-2\mu^2}{3}.
$$

For $\mu\ne1/2$, a zero would have to occur at zero or $\pi$; the latter occurs only at $(1\pm\sqrt3)/2$, both outside the displayed stable intervals. At $\mu=1/2$, $D=3/4+(1/4)\cos\theta\geq1/2$. Thus there is no denominator zero in the stable range. For fixed such $\mu$, continuity on the compact frequency interval gives a uniformly bounded inverse, and $|G|\leq1$ proves $\|U^n\|_{2,h}\leq\|U^0\|_{2,h}$ for all steps.

Outside these intervals the displayed difference is negative at every nonzero frequency where $D\ne0$, so $|G|>1$. On periodic refining meshes there are frequencies approaching any selected such value. Their amplification is bounded away from one and is repeated $O(h^{-1})$ times over a fixed physical interval when $k=\mu h$, violating a mesh-uniform stability bound. At the two singular parameters the implicit operator itself fails on meshes containing the Nyquist mode. These observations prove necessity as well as sufficiency.

For the physical convention $k>0$, $h>0$, the result is **$0<\mu\leq1$ or $\mu\geq2$**, with zero admitted as the identity limit. The negative intervals describe the algebraic contraction result for signed [Courant numbers](../../../finite-difference.md#courant-number). In particular, the additional large positive interval must not be discarded by imposing the usual explicit-scheme [Courant–Friedrichs–Lewy condition](../../../finite-difference.md#courant-friedrichs-lewy-condition): this scheme is implicit. Stability at large fixed [Courant number](../../../finite-difference.md#courant-number) is not a guarantee of a small error constant.

## 4

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For an $s$-stage [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) with coefficient [matrix](../../../vector-space.md#matrix) $A=(a_{ij})$ and weights $b=(b_i)$, put $B=\operatorname{diag}(b_i)$. It is [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) when

$$
\boxed{b_i\geq0\quad\text{for every }i,\qquad
M=BA+A^TB-bb^T\succeq0.}
$$

Equivalently, $m_{ij}=b_ia_{ij}+b_ja_{ji}-b_ib_j$ defines a [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix) symmetric [matrix](../../../vector-space.md#matrix). The condition concerns the full coefficient tableau and nonlinear contractivity, not merely the scalar [stability function](../../../numerical-analysis.md#stability-function). It is normally used with a consistent [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) and stage equations satisfying the necessary [stage solvability of an implicit Runge-Kutta method](../../../numerical-analysis.md#stage-solvability-of-an-implicit-runge-kutta-method).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Butcher contractivity theorem](../../../numerical-analysis.md#butcher-contractivity-theorem) states that an [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) is [B-stable](../../../numerical-analysis.md#b-stability): for a [dissipative vector field](../../../differential-equation.md#dissipative-vector-field) and any positive step for which the stage problems are solved, its step does not increase the distance between two numerical solutions. The required condition on the [dissipative vector field](../../../differential-equation.md#dissipative-vector-field) is

$$
\operatorname{Re}\langle f(t,u)-f(t,v),u-v\rangle\leq0
$$

for all compared states at each common time. The [inner product](../../../linear-algebra.md#inner-product) can be real Euclidean or complex Hermitian. The [stage solvability of an implicit Runge-Kutta method](../../../numerical-analysis.md#stage-solvability-of-an-implicit-runge-kutta-method) is assumed in this comparison, not a conclusion from a distance estimate alone.

Let $d$ be the difference of starting values, $D_i$ the differences of corresponding stages and $F_i$ the differences of their vector-field values. Then

$$
D_i=d+h\sum_ja_{ij}F_j,\qquad
 d_+=d+h\sum_i b_iF_i.
$$

Expanding the squared [norm](../../../functional-analysis.md#norm) of the update gives

$$
\|d_+\|^2=\|d\|^2+2h\sum_i b_i\operatorname{Re}\langle d,F_i\rangle
+h^2\sum_{i,j}b_ib_j\operatorname{Re}\langle F_i,F_j\rangle.
$$

Substitute $d=D_i-h\sum_ja_{ij}F_j$ in the linear term. Symmetrizing the double sum proves the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity)

$$
\boxed{\|d_+\|^2=\|d\|^2
+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.}
$$

Each [inner product](../../../linear-algebra.md#inner-product) in the first sum is nonpositive by the defining inequality for a [dissipative vector field](../../../differential-equation.md#dissipative-vector-field), and its weight is nonnegative. The final [quadratic form](../../../linear-algebra.md#quadratic-form) is nonnegative: resolve the [vectors](../../../vector-space.md#vector) $F_i$ into components and apply [positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix) of $M$ to each component [vector](../../../vector-space.md#vector). Hence $\boxed{\|d_+\|\leq\|d\|}$, which is exactly [B-stability](../../../numerical-analysis.md#b-stability). No [linearization](../../../algebra.md#linearization) of the [vector field](../../../calculus.md#vector-field) has been used.

For the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$ with $\operatorname{Re}\lambda\leq0$, this also bounds the amplification factor by one wherever the stages are well defined. With strictly positive weights, no stage pole can occur in the open left half-plane. Indeed, if $(I-zA)v=0$ for nonzero $v$, then

$$
v^*Mv=2\operatorname{Re}(1/z)v^*Bv-|b^Tv|^2<0
$$

when $\operatorname{Re}z<0$, contradicting $M\succeq0$. This proves the usual [A-stability](../../../numerical-analysis.md#a-stability) corollary for the scalar [stability function](../../../numerical-analysis.md#stability-function); boundedness from the open half-plane makes any boundary pole in that [rational function](../../../isolated-singularity.md#rational-function) removable. Zero-weight redundant stages require their own solvability treatment. The nonlinear [B-stability](../../../numerical-analysis.md#b-stability) statement is stronger than [A-stability](../../../numerical-analysis.md#a-stability), and the two notions should not be conflated.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For the first [Butcher tableau](../../../numerical-analysis.md#butcher-tableau), $b=(1/2,1/2)^T$ and the off-diagonal entries sum to $1/2$, while each diagonal entry is $1/4$. Thus

$$
BA+A^TB-bb^T=\begin{pmatrix}0&0\\0&0\end{pmatrix}.
$$

The positive weights and zero [matrix](../../../vector-space.md#matrix) prove that **method 1 is [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method)**. It is the two-stage [Gauss collocation method](../../../numerical-analysis.md#gauss-legendre-method).

The second method is explicit and has $b=(1/4,3/8,3/8)^T$. Its first diagonal algebraic-stability entry is

$$
m_{11}=2b_1a_{11}-b_1^2=-\frac1{16}<0.
$$

A [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix) [matrix](../../../vector-space.md#matrix) cannot have a negative diagonal [quadratic form](../../../linear-algebra.md#quadratic-form), so **method 2 is not [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method)**. The negative value supplies a direct test; its order is irrelevant to this conclusion.

For the third method, $A=\begin{pmatrix}1/4&-1/4\\1/4&5/12\end{pmatrix}$ and $b=(1/4,3/4)^T$. Direct computation gives

$$
M=\frac1{16}\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\qquad
v^TMv=\frac1{16}(v_1-v_2)^2\geq0.
$$

Both weights are positive, so **method 3 is [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method)**.

## 5

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Interpret the square as $[0,1]^2$, use equal spacing $h=1/J$ in both directions and retain interior indices $1\leq m,n\leq J-1$. Boundary values contribute to the right-hand side and do not change the interior coefficient [matrix](../../../vector-space.md#matrix). Products of the one-dimensional sine modes used in the [discrete sine transform](../../../numerical-analysis.md#discrete-sine-transform)

$$
v_{pq}(m,n)=\sin(p\pi m/J)\sin(q\pi n/J)
$$

form a [basis](../../../vector-space.md#basis), and substitution into the [five-point Laplacian](../../../finite-difference.md#five-point-laplacian) gives

$$
\Delta_hv_{pq}=-\Lambda_{pq}v_{pq},\qquad
\Lambda_{pq}=\frac4{h^2}\left[
\sin^2\left(\frac{p\pi}{2J}\right)+
\sin^2\left(\frac{q\pi}{2J}\right)\right].
$$

The interior [matrix](../../../vector-space.md#matrix) is $\Delta_h+\lambda I$, so it is nonsingular exactly when

$$
\boxed{\lambda\notin\{\Lambda_{pq}:1\leq p,q\leq J-1\}.}
$$

These are the [discrete Helmholtz resonance](../../../partial-differential-equation.md#discrete-helmholtz-resonance) values, including their possible multiplicities. A sufficient condition is $\lambda<\Lambda_{11}=8h^{-2}\sin^2(\pi/(2J))$, so in particular every nonpositive $\lambda$ is allowed. That is not a necessary restriction: positive values between, or above, the finitely many discrete [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are nonsingular as well. With homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) a nonresonant system has only the zero solution; at a resonance the corresponding modes of the [discrete sine transform](../../../numerical-analysis.md#discrete-sine-transform) give nonzero homogeneous solutions.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For a sufficiently smooth function, [Taylor expansion](../../../calculus.md#taylor-expansion) of the four neighboring values gives

$$
\Delta_hu=\Delta u+\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).
$$

The reaction term $\lambda u$ is sampled exactly at the grid point. On an exact solution, therefore,

$$
\boxed{(\Delta_h+\lambda)u
=\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).}
$$

The method has **second-order local accuracy for the [partial differential equation](../../../partial-differential-equation.md)**. The original printed equations multiply this expression by $h^2$, so their unscaled residual is $O(h^4)$; that scaling does not make the [Laplacian](../../../calculus.md#laplacian) approximation fourth order. Resonance and inverse-matrix bounds are separate issues from this local truncation calculation.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let $S_1u$ be the sum of the four axial neighbors and $S_2u$ the sum of the four diagonal neighbors. The two PDF stencils define

$$
\Gamma_9u=\frac23S_1u+\frac16S_2u-\frac{10}3u,
\qquad M_hu=\frac23u+\frac1{12}S_1u.
$$

The reaction stencil has four axial weights $1/12$ and center weight $2/3$, so its weights sum to one. [Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
h^{-2}\Gamma_9u=\Delta u+\frac{h^2}{12}\Delta^2u+O(h^4),\qquad
M_hu=u+\frac{h^2}{12}\Delta u+O(h^4).
$$

For example, the diagonal neighbors supply the $u_{xxyy}$ term needed to turn the fourth derivatives into the full squared [Laplacian](../../../calculus.md#laplacian). Adding the reaction contribution produces

$$
h^{-2}\Gamma_9u+\lambda M_hu
=(\Delta+\lambda)u+\frac{h^2}{12}\Delta(\Delta+\lambda)u+O(h^4).
$$

On a smooth solution of the constant-coefficient equation, both displayed leading terms vanish. Thus the [compact fourth-order Helmholtz stencil](../../../finite-difference.md#compact-fourth-order-helmholtz-stencil) has

$$
\boxed{\text{fourth-order normalized local accuracy,}\qquad
\Gamma_9u+\lambda h^2M_hu=O(h^6).}
$$

The cancellation uses the differential equation and constant $\lambda$; the [nine-point finite-difference stencil](../../../finite-difference.md#nine-point-finite-difference-stencil) alone still has an $O(h^2)$ operator error on an arbitrary smooth function. It also does not establish a uniform global fourth-order error without an appropriate inverse bound and compatible treatment of boundaries and resonances.

## 6

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [eigenvalue stability analysis of a finite difference method](../../../finite-difference.md#eigenvalue-stability-analysis-of-a-finite-difference-method) reduces a linear evolution discretization to its modal behavior, but it must retain the [norm](../../../functional-analysis.md#norm) and the dependence on the mesh. For a homogeneous system obtained by the [method of lines](../../../finite-difference.md#method-of-lines), $U'=A_hU$, the solution is $e^{tA_h}U(0)$. A one-step time discretization gives $U^{n+1}=G_{h,k}U^n$; for a [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method), where its stage [matrices](../../../vector-space.md#matrix) are invertible, $G_{h,k}=R(kA_h)$. With a [multistep method](../../../numerical-analysis.md#linear-multistep-method) one instead uses an amplification [matrix](../../../vector-space.md#matrix) on the augmented [vector](../../../vector-space.md#vector) of several time levels.

The relevant finite-time stability estimate is

$$
\boxed{\|G_{h,k}^n\|_h\leq C_T\quad\text{whenever }0\leq nk\leq T,}
$$

with $C_T$ independent of the refining spatial mesh and allowed time steps. Similarly, semidiscrete stability requires $\|e^{tA_h}\|_h\leq C_T$ for $0\leq t\leq T$. The [norm](../../../functional-analysis.md#norm) should represent the continuum problem, such as the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm) $\|U\|_{2,h}^2=h\sum_j|U_j|^2$ in one dimension. A fixed finite [matrix](../../../vector-space.md#matrix) having decaying solutions as $t\to\infty$ is not by itself a mesh-uniform result for the [partial differential equation](../../../partial-differential-equation.md).

If $G=X\Lambda X^{-1}$, then

$$
\|G^n\|\leq\|X\|\|X^{-1}\|\max_j|\lambda_j|^n.
$$

Thus [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of modulus at most one give a uniform bound when the diagonalizing [bases](../../../vector-space.md#basis) have uniformly bounded [condition numbers](../../../linear-algebra.md#condition-number). For a [normal matrix](../../../linear-operator-theory.md#normal-matrix) in the chosen [inner product](../../../linear-algebra.md#inner-product), the [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators) supplies an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), so the [condition number](../../../linear-algebra.md#condition-number) is one and the [norm](../../../functional-analysis.md#norm) of $G^n$ is exactly $\max_j|\lambda_j|^n$. For a [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) or [skew-adjoint](../../../functional-analysis.md#skew-adjoint-generator) spatial [matrix](../../../vector-space.md#matrix), applying a scalar [stability function](../../../numerical-analysis.md#stability-function) preserves this favorable modal structure. This is the setting where [eigenvalue](../../../linear-operator-theory.md#eigenvalue) calculations provide especially clean, reliable step restrictions.

A precise fixed-matrix statement is also useful: a [matrix](../../../vector-space.md#matrix) is power bounded for all nonnegative integers $n$ if and only if all its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) lie in the closed [unit disk](../../../geometry-and-topology.md#unit-disk) and every [Jordan block](../../../linear-operator-theory.md#jordan-block) at a unit-modulus [eigenvalue](../../../linear-operator-theory.md#eigenvalue) has size one. Indeed, powers of an interior [Jordan block](../../../linear-operator-theory.md#jordan-block) contain a [polynomial](../../../polynomial.md) in $n$ times a decaying geometric factor and are bounded; a larger block on the unit circle produces unbounded [polynomial](../../../polynomial.md) growth. For a family of [matrices](../../../vector-space.md#matrix), the resulting bounds must still be uniform. Moreover, [finite-time stability versus power boundedness](../../../finite-difference.md#finite-time-stability-versus-power-boundedness) distinguishes this all-time condition from the physical-time estimate above. For example $G_k=I+kN$, $N^2=0$, has $G_k^n=I+nkN$, bounded for $nk\leq T$ despite a nontrivial [Jordan block](../../../linear-operator-theory.md#jordan-block) at one. Even the scalar update $1+k$ is stable on fixed intervals, since $(1+k)^n\leq e^T$, although it represents a growing equation rather than a contraction.

For a constant-coefficient periodic difference operator, [Fourier modes](../../../fourier-analysis.md#fourier-mode) diagonalize the spatial [matrix](../../../vector-space.md#matrix). The [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform) is a [unitary operator](../../../vector-space.md#unitary-operator), so [Parseval's identity](../../../fourier-analysis.md#parseval-identity) identifies its modal maximum with the [operator norm](../../../continuous-dual-space.md#operator-norm). The [eigenvalue stability analysis of a finite difference method](../../../finite-difference.md#eigenvalue-stability-analysis-of-a-finite-difference-method) then becomes [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis). For the [Dirichlet discrete Laplacian](../../../finite-difference.md#dirichlet-discrete-laplacian), a [discrete sine transform](../../../numerical-analysis.md#discrete-sine-transform) plays the same role. These facts explain its advantages: a large [matrix](../../../vector-space.md#matrix) calculation becomes a scalar symbol or a known spectral interval, and the extremal [eigenvalue](../../../linear-operator-theory.md#eigenvalue) directly determines a safe time step.

As a first example, centered space discretization of the [heat equation](../../../diffusion-equation.md#heat-equation) $u_t=u_{xx}$ has [eigenvalues](../../../linear-operator-theory.md#eigenvalue)

$$
\lambda(\theta)=-\frac4{h^2}\sin^2(\theta/2).
$$

[Forward Euler method](../../../numerical-analysis.md#euler-method) gives $R(k\lambda)=1-4r\sin^2(\theta/2)$ with $r=k/h^2$. Requiring all factors in $[-1,1]$ yields $0\leq r\leq1/2$ for all periodic meshes. In two dimensions the corresponding uniform bound is $r\leq1/4$. Because these are [normal matrices](../../../linear-operator-theory.md#normal-matrix), these scalar bounds prove contraction rather than merely suggest it.

[Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $R(z)=1/(1-z)$, so the centered discretization of the [heat equation](../../../diffusion-equation.md#heat-equation) is contractive for every $k>0$. The [Crank-Nicolson method](../../../numerical-analysis.md#crank-nicolson-method) has $R(z)=(1+z/2)/(1-z/2)$ and is likewise contractive for these negative real modes. However, its factor tends to $-1$ for very stiff modes, leaving high-frequency oscillations weakly damped; [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) tends to zero. The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) therefore expose the presence of [stiff differential equations](../../../numerical-analysis.md#stiff-equation) and damping as well as binary stability. Unconditional stability does not remove accuracy requirements.

For an [advection equation](../../../partial-differential-equation.md#transport-equation) example, the [upwind finite difference scheme](../../../finite-difference.md#upwind-finite-difference-scheme) for $u_t+c u_x=0$, $c>0$, has factor $G=1-\nu+\nu e^{-i\theta}$, with $\nu=ck/h$. Since

$$
|G|^2=1-2\nu(1-\nu)(1-\cos\theta),
$$

it is a contraction in the periodic [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm) exactly for $0\leq\nu\leq1$. In contrast, [Forward Euler method](../../../numerical-analysis.md#euler-method) with centered advection has factor $1-i\nu\sin\theta$. Its modulus exceeds one at nonzero active frequencies, and repeated amplification makes it unstable under fixed nonzero Courant refinement. A much smaller scaling $k=O(h^2)$ can bound its finite-time growth, demonstrating again that exact contraction and the most general stability estimate are different claims.

The major limitation is the possible presence of a [nonnormal matrix](../../../linear-operator-theory.md#non-normal-matrix). For example,

$$
A_h=\begin{pmatrix}-1&h^{-1}\\0&-1\end{pmatrix},\qquad
e^{tA_h}=e^{-t}\begin{pmatrix}1&t/h\\0&1\end{pmatrix}.
$$

Both [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are negative, yet at $t=1$ the second unit [vector](../../../vector-space.md#vector) is amplified by at least $1/(eh)$. This proves that [negative spectra do not imply uniform semidiscrete stability](../../../finite-difference.md#negative-spectra-do-not-imply-uniform-semidiscrete-stability). Ill-conditioned [eigenvectors](../../../linear-operator-theory.md#eigenvector), [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) and transient amplification can invalidate a spectral-only argument. Direct [energy estimates](../../../partial-differential-equation.md#energy-estimate) or estimates for the [resolvent](../../../functional-analysis.md#resolvent-of-an-operator) can supply the missing [norm](../../../functional-analysis.md#norm) control.

[Boundary conditions](../../../differential-equation.md#boundary-condition) are another limitation. A periodic symbol proves a periodic or whole-line result, not an arbitrary initial-boundary-value problem. [Boundary closure of a difference scheme](../../../finite-difference.md#boundary-closure-of-a-difference-scheme) can introduce growing modes or mesh-dependent amplification. A spatial operator with variable coefficients can still be studied through its assembled [matrix](../../../vector-space.md#matrix), but then whether it is a [normal matrix](../../../linear-operator-theory.md#normal-matrix), its [condition number](../../../linear-algebra.md#condition-number) and the physical [inner product](../../../linear-algebra.md#inner-product) must be checked rather than borrowed from a [Fourier stability analysis](../../../finite-difference.md#fourier-stability-analysis). For the [finite element method](../../../numerical-analysis.md#finite-element-method) the natural [mass matrix](../../../numerical-analysis.md#mass-matrix) [inner product](../../../linear-algebra.md#inner-product) often turns a [generalized eigenvalue problem](../../../linear-operator-theory.md#generalized-eigenvalue-problem) into a [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) one.

For time-dependent or split updates, separate spectra are insufficient to control products. For instance, $G_1=\begin{pmatrix}0&K\\0&0\end{pmatrix}$ and $G_2=\begin{pmatrix}0&0\\K&0\end{pmatrix}$ each have only zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue), while $G_2G_1$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $K^2$. For $K>1$, alternating the two is unstable. A common contractive [norm](../../../functional-analysis.md#norm) would control the products, but their individual [eigenvalues](../../../linear-operator-theory.md#eigenvalue) do not.

Finally, stability and [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) have different roles. The [Lax equivalence theorem](../../../finite-difference.md#lax-equivalence-theorem) states that, for a well-posed linear initial-value problem and a consistent [finite difference method](../../../finite-difference.md#finite-difference-method) on compatible grid spaces, stability on every fixed time interval is equivalent to [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) as the admissible meshes refine. Bounded grid representation and the correct initial and boundary setup are part of that framework. An [eigenvalue](../../../linear-operator-theory.md#eigenvalue) estimate can establish its stability hypothesis in the favorable settings described above; it neither proves [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) nor bypasses its uniformity requirements. The method is therefore a powerful modal tool, provided its spectral calculation is connected to a genuine [norm](../../../functional-analysis.md#norm) estimate.

## 7

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

A fixed-step [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) for $y'=f(t,y)$ uses several previous solution and derivative values:

$$
\sum_{j=0}^s\alpha_jy_{n+j}
=k\sum_{j=0}^s\beta_jf(t_{n+j},y_{n+j}),\qquad \alpha_s\ne0.
$$

The coefficients are fixed independently of the step size. It is explicit when $\beta_s=0$ and implicit otherwise. Its [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) are $\rho(w)=\sum_j\alpha_jw^j$ and $\sigma(w)=\sum_j\beta_jw^j$. The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) gives a uniquely solvable implicit step under a [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) bound $L$ whenever $k|\beta_s|L<|\alpha_s|$, by contraction of the new-value equation on the appropriate solution region. A suitable starting procedure must supply the first $s$ values; the method alone does not determine them.

Order is defined by inserting a smooth exact solution into the recurrence. If the residual is $O(k^{p+1})$ and its first nonzero coefficient occurs at that degree, the method has order $p$; dividing the residual by $k$ gives an $O(k^p)$ [local truncation error](../../../numerical-analysis.md#local-truncation-error). [Taylor expansion](../../../calculus.md#taylor-expansion) gives the exact [order conditions for a linear multistep method](../../../numerical-analysis.md#order-conditions-for-a-linear-multistep-method)

$$
\sum_j\alpha_jj^q=q\sum_j\beta_jj^{q-1}\quad(0\leq q\leq p),
$$

with the right side interpreted as zero at $q=0$, and failure at $q=p+1$ for exact order. Equivalently,

$$
\rho(e^z)-z\sigma(e^z)=O(z^{p+1}).
$$

The basic [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) conditions are $\rho(1)=0$, $\rho'(1)=\sigma(1)$; for the ordinary nondegenerate consistent formulation this common value is nonzero. Exactness on constants and linear functions does not control propagation of numerical perturbations.

That propagation is the role of [zero-stability](../../../numerical-analysis.md#zero-stability). On $y'=0$ the homogeneous recurrence is $\rho(E)y_n=0$. Its modes are $n^r\xi^n$, with powers of $n$ determined by root multiplicities. The theorem on the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) states that [zero-stability](../../../numerical-analysis.md#zero-stability) is equivalent to every root of $\rho$ having modulus at most one, with every unit-modulus root simple. Interior repeated roots are permitted, since geometric decay dominates their [polynomial](../../../polynomial.md) factors. An exterior root amplifies perturbations geometrically; a repeated unit root amplifies them polynomially and violates a step-independent perturbation bound.

The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) states that a fixed-step consistent [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) is convergent exactly when it is [zero-stable](../../../numerical-analysis.md#zero-stability). This concerns [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) with a uniformly [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) right-hand side on the solution region over a fixed finite interval, convergent starting values, and the well-defined nearby branch of each small-step implicit solve. For order $p$ [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method), the solution must have the required smoothness and the starting errors must be $O(k^p)$.

The mechanism can be sketched explicitly. The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) bounds the recurrence's discrete [Green function](../../../analysis.md#green-s-function). For an order-$p$ exact-solution defect $d_n=O(k^{p+1})$, the [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) error equation then gives an estimate of the form

$$
E_n\leq C\left(E_{\mathrm{start}}+\sum_{j<n}\|d_j\|\right)
+Ck\sum_{j\leq n}E_j.
$$

The current-step term can be absorbed for small $k$. The [discrete Gronwall inequality](../../../probability-and-statistics.md#discrete-gronwall-inequality) says that a bound $E_n\leq A+Bk\sum_{j<n}E_j$ implies $E_n\leq A(1+Bk)^n\leq Ae^{Bt_n}$. There are $O(k^{-1})$ defects on a fixed interval, so their sum is $O(k^p)$ and this yields the claimed global order. Conversely, testing $y'=0$ with vanishing starting perturbations in exterior-root or repeated-unit-root modes proves that [convergence of a numerical method](../../../numerical-analysis.md#convergence-of-a-numerical-method) fails without the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method).

For example, the two-step [Adams-Bashforth method](../../../numerical-analysis.md#adams-bashforth-method) has

$$
y_{n+2}-y_{n+1}=k(3f_{n+1}-f_n)/2,
\qquad \rho=w(w-1),\quad\sigma=(3w-1)/2.
$$

It is explicit, order two and [zero-stable](../../../numerical-analysis.md#zero-stability), hence convergent with order-two starting values. By contrast, a recurrence with $\rho=(w-1)^2$ has solutions $y_n=y_0+n(y_1-y_0)$ on the zero differential equation. Starting differences $\sqrt k$ tend to zero yet become unbounded at a fixed positive time, since $n$ is of order $1/k$. A small local defect or formal high order cannot rescue this mode. Canceling a common factor may remove it only by changing the allowed starting relations, as the parameter endpoint in Question 2 illustrates.

[Absolute stability](../../../numerical-analysis.md#linear-stability-domain) addresses a different limit: apply the method to the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$ and put $z=k\lambda$. The amplification roots satisfy

$$
P_z(w)=\rho(w)-z\sigma(w)=0.
$$

All roots must satisfy the disk condition, with unit roots simple; one cannot inspect only the root that tends to one as $z\to0$. The degree and solvability of the recurrence must also be preserved. The resulting set of $z$ is the domain of [absolute stability](../../../numerical-analysis.md#linear-stability-domain). [A-stability](../../../numerical-analysis.md#a-stability) means that it includes the whole closed left half-plane, so the numerical solutions of every [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) with $\operatorname{Re}\lambda\leq0$ are stable for every positive step size. It is a linear test-equation property, not a proof of arbitrary nonlinear contractivity or high accuracy at large steps.

[Forward Euler method](../../../numerical-analysis.md#euler-method) has order one and factor $1+z$, so its stability region is the disk $|1+z|\leq1$. [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has factor $(1-z)^{-1}$ and is [A-stable](../../../numerical-analysis.md#a-stability). The [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule) is order two with factor $(1+z/2)/(1-z/2)$; its modulus is at most one throughout the left half-plane. These one-step methods are included as the simplest multistep examples. For the two-step [Adams-Bashforth method](../../../numerical-analysis.md#adams-bashforth-method), the negative-real stability interval is $-1\leq z\leq0$: its [polynomial](../../../polynomial.md) is $w^2-(1+3z/2)w+z/2$, and the root reaches $-1$ at $z=-1$. It therefore imposes a step restriction when applied to strongly decaying modes.

The genuinely two-step [BDF2 method](../../../numerical-analysis.md#second-order-backward-differentiation-formula) is

$$
3y_{n+2}-4y_{n+1}+y_n=2k f_{n+2}.
$$

It has order two, roots $1,1/3$ at zero step and is [A-stable](../../../numerical-analysis.md#a-stability). For its normalized [polynomials](../../../polynomial.md) $\rho=3w^2/2-2w+1/2$, $\sigma=w^2$, the unit-circle boundary locus has

$$
\operatorname{Re}\frac{\rho(e^{i\theta})}{\sigma(e^{i\theta})}
=(1-\cos\theta)^2\geq0.
$$

The leading coefficient has no zero in the left half-plane, and the roots at a small negative $z$ are both inside the disk. Root continuity then proves open-half-plane stability; on the imaginary boundary the only possible unit root is the simple root one at $z=0$. This gives a direct proof of the stated [A-stability](../../../numerical-analysis.md#a-stability) rather than relying on a boundary plot.

Two sharp order barriers explain the tradeoff. The [first Dahlquist barrier](../../../numerical-analysis.md#first-dahlquist-barrier) states that a consistent [zero-stable](../../../numerical-analysis.md#zero-stability) real linear $s$-step method using only first derivatives has order at most $s+1$ for odd $s$ and $s+2$ for even $s$; an explicit method has order at most $s$. The [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier) states that an irreducible [A-stable](../../../numerical-analysis.md#a-stability) real [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) has order at most two. These statements concern fixed constant coefficients and the ordinary first-derivative multistep class, not multiderivative methods or arbitrary variable-step formulations. Thus higher order alone is not a route to unconditional stiff stability. Question 2 provides a concrete illustration: its third-order member is [zero-stable](../../../numerical-analysis.md#zero-stability) but not [A-stable](../../../numerical-analysis.md#a-stability).

No nontrivial consistent explicit [multistep method](../../../numerical-analysis.md#linear-multistep-method) is [A-stable](../../../numerical-analysis.md#a-stability). Its [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) has a fixed highest coefficient, while at least one lower coefficient grows without bound as real $z\to-\infty$. Were all roots uniformly in the [unit disk](../../../geometry-and-topology.md#unit-disk), their [elementary symmetric polynomials](../../../polynomial.md#elementary-symmetric-polynomial) would keep all the monic coefficients bounded, a contradiction. This is the coefficient argument behind [explicit multistep methods cannot be A-stable](../../../numerical-analysis.md#explicit-multistep-methods-cannot-be-a-stable).

In practice, selecting a method therefore involves accuracy, startup, the presence of a [stiff differential equation](../../../numerical-analysis.md#stiff-equation), implicit-solve cost and step-size control. [Zero-stability](../../../numerical-analysis.md#zero-stability) handles propagation as the step tends to zero; [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) supplies a vanishing defect; [A-stability](../../../numerical-analysis.md#a-stability) handles the numerical solutions of all decaying [Dahlquist test equations](../../../numerical-analysis.md#dahlquist-test-equation) at finite steps. None substitutes for the others, and variable steps or PDE discretizations require additional uniform stability arguments appropriate to their setting.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
