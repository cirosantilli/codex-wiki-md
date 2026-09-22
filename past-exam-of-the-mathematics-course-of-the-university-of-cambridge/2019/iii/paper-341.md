# Paper 341

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_341.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_341.pdf)

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

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Expand about $t=t_{n+2}$ and use $y''=f'(y)f(y)$ from the [chain rule](../../../calculus.md#chain-rule). The residual of the exact solution is

$$
\begin{aligned}
&y(t)-\frac87y(t-h)+\frac17y(t-2h)-\frac67hy'(t)+\frac27h^2y''(t)\\
&\qquad=\frac1{21}h^4y^{(4)}(t)+O(h^5).
\end{aligned}
$$

The coefficients through $h^3$ vanish, and the displayed fourth-order coefficient does not. Thus the [multiderivative multistep method](../../../numerical-analysis.md#multiderivative-multistep-method) has **order three**.

At $h=0$, its first characteristic polynomial is

$$
\rho(\xi)=\xi^2-\frac87\xi+\frac17=(\xi-1)(\xi-1/7).
$$

Its roots are $1$ and $1/7$, with the unit-modulus root simple, so it satisfies the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) and is [zero-stable](../../../numerical-analysis.md#zero-stability). Combining this with the defect estimate proves **convergence of order three**, assuming sufficiently smooth $f$, order-three starting values, and the nearby branch of each implicit update.

More explicitly, the right-hand side is $hF_h(y_{n+2})$, where $F_h=6f/7-2hf'f/7$ has a uniform local [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) bound for small $h$. A bounded zero-stable impulse response and the [discrete Gronwall inequality](../../../probability-and-statistics.md#discrete-gronwall-inequality) therefore control the accumulated $O(h^4)$ defects by $O(h^3)$ over fixed time intervals. This is [convergence of a zero-stable multiderivative method](../../../numerical-analysis.md#convergence-of-a-zero-stable-multiderivative-method), rather than a direct application of the first-derivative-only [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), put $z=h\lambda$. The amplification roots satisfy

$$
(7-6z+2z^2)\xi^2-8\xi+1=0.
$$

We show that no root can reach the [unit circle](../../../complex-analysis.md#complex-unit-circle) for $\operatorname{Re}z<0$. If $\xi=e^{i\theta}$, solving the quadratic in $z$ gives

$$
z=\frac32\pm\sqrt C,\qquad C=-\frac54+4e^{-i\theta}-\frac12e^{-2i\theta}.
$$

Write $c=\cos\theta$, $u=\operatorname{Re}C=-3/4+4c-c^2$, and $v=\operatorname{Im}C=(c-4)\sin\theta$. Then $u\leq9/4$ and

$$
\left(\frac92-u\right)^2-|C|^2
=\frac{81}{4}-9u-v^2
=(c-1)^2(c^2-6c+11)\geq0.
$$

Since $9/2-u>0$, this gives $|C|+u\leq9/2$. Consequently $|\operatorname{Re}\sqrt C|^2=(|C|+u)/2\leq9/4$, so both possible $z$ have nonnegative real part. Equality can occur only at $\theta=0$, which gives $z=0$ or $z=3$.

The leading coefficient has zeros $(3\pm i\sqrt5)/2$, both in the right half-plane. Hence the amplification roots vary continuously as a pair throughout the left half-plane. At $z=-1$ they are $1/3$ and $1/5$; neither can leave the [unit disk](../../../geometry-and-topology.md#unit-disk) without crossing the [unit circle](../../../complex-analysis.md#complex-unit-circle), which the preceding calculation excludes. The same conclusion extends to the imaginary axis, with strict inequality away from $z=0$. At zero the roots $1,1/7$ satisfy the simplicity requirement.

Thus the method is **[A-stable](../../../numerical-analysis.md#a-stability)**. Its third order does not contradict the usual second-order barrier, because it is a [multiderivative multistep method](../../../numerical-analysis.md#multiderivative-multistep-method).

## 2

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The tableau is the three-stage [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method). For its stage [matrix](../../../vector-space.md#matrix) $A$, weights $b$, nodes $c$ and $C=\operatorname{diag}(c)$, the [Butcher order conditions](../../../numerical-analysis.md#butcher-order-condition) through order four are

$$
\begin{gathered}
b^T\mathbf1=1,\quad b^Tc=\frac12,\quad b^Tc^{\circ2}=\frac13,\quad b^TAc=\frac16,\\
b^Tc^{\circ3}=\frac14,\quad b^TCAc=\frac18,\quad b^TAc^{\circ2}=\frac1{12},\quad b^TA^2c=\frac1{24},
\end{gathered}
$$

where $c^{\circ j}$ means coordinatewise powers. Direct substitution verifies all eight identities. Equivalently, this is a [collocation Runge-Kutta method](../../../numerical-analysis.md#collocation-runge-kutta-method) at the three [Lobatto quadrature](../../../numerical-analysis.md#lobatto-quadrature) nodes, whose weights integrate cubic [polynomials](../../../polynomial.md) exactly.

Order five would require $b^Tc^{\circ4}=1/5$, but here $b^Tc^{\circ4}=5/24$. Therefore the method has **exactly order four**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [stability function](../../../numerical-analysis.md#stability-function) of a [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) is $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$. Substitution gives

$$
\boxed{R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}.}
$$

Writing the numerator and denominator as $N(z)$ and $D(z)$,

$$
|D(z)|^2-|N(z)|^2=-2\operatorname{Re}z\left(1+\frac{|z|^2}{12}\right).
$$

The denominator has zeros $3\pm i\sqrt3$, both in the right half-plane. Therefore $|R(z)|\leq1$ throughout the closed left half-plane, with strict inequality in its interior. The method is **[A-stable](../../../numerical-analysis.md#a-stability)**. Since $R(z)\to1$ at infinity, it is not [L-stable](../../../numerical-analysis.md#l-stability).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method), the weights must be nonnegative and the real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $M=BA+A^TB-bb^T$, where $B=\operatorname{diag}(b)$, must be a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix).

The weights are positive, but $a_{11}=0$ and $b_1=1/6$, so

$$
M_{11}=2b_1a_{11}-b_1^2=-\frac1{36}<0.
$$

A [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) cannot have a negative diagonal entry, as its [quadratic form](../../../linear-algebra.md#quadratic-form) at the first [standard basis](../../../vector-space.md#standard-basis) vector would be negative. Thus this [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method) is **not [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method)**, despite its [A-stability](../../../numerical-analysis.md#a-stability).

## 3

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $h=\Delta x$ and set $u_0=u_{M+1}=0$. In the discrete [L2 norm](../../../real-analysis.md#l2-norm) $\|u\|_h^2=h\sum_{m=1}^M|u_m|^2$, the [energy method](../../../numerical-analysis.md#energy-method) gives

$$
\frac12\frac{d}{dt}\|u\|_h^2
=-\frac1h\sum_{m=0}^M|u_{m+1}-u_m|^2\leq0.
$$

To obtain this identity, shift the indices in the centered second-difference sum. The centered first-difference [matrix](../../../vector-space.md#matrix) is [skew-symmetric](../../../linear-algebra.md#skew-symmetric-matrix), so its contribution has zero real part even for complex grid values. The homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) remove the endpoint terms.

Therefore the semidiscretization is **stable for every real $\alpha$ and every positive $h$**, with the mesh-independent bound $\|u(t)\|_h\leq\|u(0)\|_h$. No restriction on $|\alpha|h$ is needed for this energy estimate.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

With $h=\Delta x$, $\tau=\Delta t$, $r=\tau/h^2$ and $c=\alpha\tau/h$, the [Forward Euler method](../../../numerical-analysis.md#euler-method) gives

$$
\boxed{u_m^{n+1}=(r-c/2)u_{m-1}^n+(1-2r)u_m^n+(r+c/2)u_{m+1}^n.}
$$

For a [Fourier mode](../../../fourier-analysis.md#fourier-mode) $e^{im\theta}$, the amplification factor is $G(\theta)=1-4r\sin^2(\theta/2)+ic\sin\theta$. Set $s=\sin^2(\theta/2)$. Then

$$
|G|^2-1=4s\{c^2-2r+(4r^2-c^2)s\}.
$$

The expression in braces is an [affine function](../../../vector-space.md#affine-function) of $s$, so it is nonpositive for all $s\in[0,1]$ precisely when its two endpoint values are nonpositive. For $\tau>0$, these conditions are $c^2\leq2r$ and $r\leq1/2$. Thus [Forward Euler stability for centered advection-diffusion](../../../finite-difference.md#forward-euler-stability-for-centered-advection-diffusion) requires exactly

$$
\boxed{\Delta t\leq\frac{(\Delta x)^2}{2},\qquad\alpha^2\Delta t\leq2.}
$$

For $\alpha=0$, only the first condition remains. If either bound fails, a band of [Fourier modes](../../../fourier-analysis.md#fourier-mode) has $|G|>1$, giving instability under [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis). At equality the amplification bound still holds, so the endpoints are included. This is discrete [L2 norm](../../../real-analysis.md#l2-norm) stability; nonnegative stencil weights would impose the additional spatial restriction $|\alpha|\Delta x\leq2$.

## 4

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Keep the [Courant number](../../../finite-difference.md#courant-number) $\mu=\Delta t/\Delta x$ fixed and write $h=\Delta x$. An exact solution of $u_t=u_x$ is $u(x,t)=g(x+t)$. Substituting it into the update gives the defect

$$
g(s+\mu h)-(1-2\mu)\{g(s)-g(s+h)\}-g(s+(1-\mu)h)
=\frac{\mu(1-\mu)(1-2\mu)}6h^3g^{(3)} + O(h^4),
$$

where $s=x+t$ and $g^{(3)}$ is evaluated at $s$. The constant, first-derivative and second-derivative terms cancel. Dividing by $\Delta t=\mu h$ gives a second-order consistency error. Hence for fixed $0<\mu<1$, $\mu\ne1/2$, the scheme has **order two**.

At the special value $\mu=1/2$, the update reduces to $u_m^{n+1}=u_{m+1}^{n-1}$. This is exactly the transport over two time steps, since $2\Delta t=\Delta x$, so the defect vanishes identically. With exact data at both starting levels it transports their values exactly; errors in those starting levels are still present, and the even and odd time subsequences evolve separately.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a [Fourier mode](../../../fourier-analysis.md#fourier-mode), the amplification polynomial is

$$
\xi^2-(1-2\mu)(1-e^{i\theta})\xi-e^{i\theta}=0.
$$

Put $a=1-2\mu$ and $\xi=e^{i\theta/2}\eta$. The roots become

$$
\eta_\pm=-ia\sin(\theta/2)\pm\sqrt{1-a^2\sin^2(\theta/2)}.
$$

If $|a|<1$, the square root is real, both roots have [modulus](../../../complex-analysis.md#modulus) one, and their separation is at least $2\sqrt{1-a^2}>0$. The companion [matrix](../../../vector-space.md#matrix) has [eigenvectors](../../../linear-operator-theory.md#eigenvector) $(\xi_\pm,1)^T$, so their uniform separation gives a mesh-independent bound on its powers. By [power boundedness of a two-level Fourier scheme](../../../finite-difference.md#power-boundedness-of-a-two-level-fourier-scheme) and the discrete [Fourier transform](../../../analysis.md#fourier-transform), this proves stability for $0<\mu<1$.

If $|a|>1$, choose $\theta=\pi$. The roots have product of [modulus](../../../complex-analysis.md#modulus) one and unequal [moduli](../../../complex-analysis.md#modulus), so one has [modulus](../../../complex-analysis.md#modulus) greater than one. The scheme is unstable.

The boundary cases require more than a root-modulus check. At $\theta=\pi$, $\mu=0$ gives $(\xi-1)^2=0$, while $\mu=1$ gives $(\xi+1)^2=0$. The companion [matrices](../../../vector-space.md#matrix) have nontrivial [Jordan blocks](../../../linear-operator-theory.md#jordan-block) and solutions of the form $(A+Bn)(\pm1)^n$. Their linear growth rules out a uniform stability bound. This mode occurs on even periodic grids, which are enough to disprove mesh-uniform stability at the endpoints.

Therefore the stable range is exactly

$$
\boxed{0<\mu<1.}
$$

Within this range, second-order convergence additionally requires two appropriately accurate starting time levels. The unit-modulus parasitic root near $\theta=0$ does not decay, so poor initialization cannot be repaired by the scheme.

## 5

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $x_m=mh$ be a uniform periodic mesh, with indices interpreted modulo the number of nodes. Write the [finite element](../../../numerical-analysis.md#finite-element) approximation as $u_h(x,t)=\sum_jU_j(t)\phi_j(x)$ using the [chapeau functions](../../../numerical-analysis.md#piecewise-linear-hat-function). The [Galerkin method](../../../partial-differential-equation.md#galerkin-method) requires

$$
\int_0^1\partial_tu_h\,\phi_m\,dx=\int_0^1\partial_xu_h\,\phi_m\,dx.
$$

The [mass matrix](../../../numerical-analysis.md#mass-matrix) has $M_{mm}=2h/3$ and $M_{m,m\pm1}=h/6$. The spatial [matrix](../../../vector-space.md#matrix) $C_{mj}=\int\phi_m\phi_j'$ has $C_{m,m+1}=1/2$ and $C_{m,m-1}=-1/2$, with zero diagonal. Therefore the semidiscrete equations are

$$
\boxed{\frac h6\left(\dot U_{m-1}+4\dot U_m+\dot U_{m+1}\right)=\frac12(U_{m+1}-U_{m-1}),}
$$

or equivalently $M\dot U=CU$. The coefficients come from integrating the products of the two overlapping [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) on each interval; periodicity supplies the wraparound entries.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [mass matrix](../../../numerical-analysis.md#mass-matrix) is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), and [integration by parts](../../../calculus.md#integration-by-parts) with periodic boundary conditions gives $C^T=-C$. Hence

$$
\frac{d}{dt}(U^TMU)=2U^TCU=0.
$$

This is [energy conservation for semidiscrete Galerkin advection](../../../numerical-analysis.md#energy-conservation-for-semidiscrete-galerkin-advection): $U^TMU=\|u_h\|_{L^2(0,1)}^2$. Thus the semidiscretization is **stable and conserves its finite element [L2 norm](../../../real-analysis.md#l2-norm)**.

For a mesh-independent comparison with the grid norm, the [Fourier symbol](../../../finite-difference.md#fourier-symbol-of-a-difference-operator) of $M$ is $h(2+\cos\theta)/3$, between $h/3$ and $h$. Consequently

$$
\frac h3\sum_m|U_m|^2\leq U^*MU\leq h\sum_m|U_m|^2.
$$

The conserved energy therefore gives a uniform bound in $\sqrt{h\sum_m|U_m|^2}$ as well. Equivalently, each [Fourier mode](../../../fourier-analysis.md#fourier-mode) evolves with the purely imaginary exponent $\sigma(\theta)=3i\sin\theta/[h(2+\cos\theta)]$. This concerns the semidiscrete method; a chosen time integrator must separately control those imaginary [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

## 6

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) with stage [matrix](../../../vector-space.md#matrix) $A$, weights $b$ and [step size](../../../convex-optimization.md#step-size) $h$ is

$$
Y_i=y_n+h\sum_j a_{ij}f(Y_j),\qquad y_{n+1}=y_n+h\sum_i b_i f(Y_i).
$$

Its order measures accuracy as $h\to0$, while stability concerns how errors or stiff components propagate. Linear [A-stability](../../../numerical-analysis.md#a-stability), strong stiff damping through [L-stability](../../../numerical-analysis.md#l-stability), and nonlinear [B-stability](../../../numerical-analysis.md#b-stability) address different questions.

For the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$, elimination of the stages gives the [stability function](../../../numerical-analysis.md#stability-function)

$$
R(z)=1+zb^T(I-zA)^{-1}\mathbf1,\qquad z=h\lambda.
$$

The [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) is $\{z:|R(z)|\leq1\}$. The method is [A-stable](../../../numerical-analysis.md#a-stability) when it contains the closed left half-plane, and [L-stable](../../../numerical-analysis.md#l-stability) when it is also true that $R(z)\to0$ as $|z|\to\infty$ there. These conditions describe, respectively, stability for every non-growing scalar linear mode and damping of very rapidly decaying modes.

The [Forward Euler method](../../../numerical-analysis.md#euler-method) has $R(z)=1+z$, so it fails [A-stability](../../../numerical-analysis.md#a-stability), for example at $z=-3$. In fact no nontrivial explicit [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) is [A-stable](../../../numerical-analysis.md#a-stability): its [stability function](../../../numerical-analysis.md#stability-function) is a nonconstant [polynomial](../../../polynomial.md), which is unbounded along the negative real axis. The [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $R(z)=1/(1-z)$. For $\operatorname{Re}z\leq0$, $|1-z|\geq1$, and the function tends to zero at infinity, proving both [A-stability](../../../numerical-analysis.md#a-stability) and [L-stability](../../../numerical-analysis.md#l-stability). The [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) has $R(z)=(1+z/2)/(1-z/2)$. The identity $|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z$ proves [A-stability](../../../numerical-analysis.md#a-stability), but its limit $-1$ rules out [L-stability](../../../numerical-analysis.md#l-stability).

For nonlinear equations, a [dissipative vector field](../../../differential-equation.md#dissipative-vector-field) satisfies $\langle f(x)-f(y),x-y\rangle\leq0$. The corresponding exact solutions contract because the time derivative of their squared distance is twice that [inner product](../../../linear-algebra.md#inner-product). A [B-stable](../../../numerical-analysis.md#b-stability) method preserves this contraction for every $h>0$, whenever its stages are well defined.

Let $d=y_n-\widetilde y_n$, $D_i=Y_i-\widetilde Y_i$, and $F_i=f(Y_i)-f(\widetilde Y_i)$. Expanding the update's squared [norm](../../../functional-analysis.md#norm), substituting $d=D_i-h\sum_j a_{ij}F_j$, and symmetrizing the double sum proves the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity)

$$
\|d_{n+1}\|^2-\|d\|^2
=2h\sum_i b_i\langle D_i,F_i\rangle-h^2\sum_{i,j}m_{ij}\langle F_i,F_j\rangle,
\quad m_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j.
$$

If $b_i\geq0$ and the [matrix](../../../vector-space.md#matrix) $M=(m_{ij})$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix), the first sum is nonpositive by dissipativity. The second double sum is nonnegative: sum the [quadratic form](../../../linear-algebra.md#quadratic-form) of $M$ over each coordinate of the $F_i$. Thus **[algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) implies [B-stability](../../../numerical-analysis.md#b-stability)**. Applied to complex scalar linear equations with the real part of the Hermitian [inner product](../../../linear-algebra.md#inner-product), the same argument also implies [A-stability](../../../numerical-analysis.md#a-stability), where the stages are defined.

The [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $b_1=a_{11}=1$, hence $M=(1)$, and is [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method). One can prove its nonlinear contraction directly: $d_{n+1}=d+h(f(y_{n+1})-f(\widetilde y_{n+1}))$ gives $\|d_{n+1}\|^2\leq\langle d,d_{n+1}\rangle\leq\|d\|\|d_{n+1}\|$. The [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) has $a_{11}=1/2$, $b_1=1$ and $M=0$, so it is [B-stable](../../../numerical-analysis.md#b-stability) even though it is not [L-stable](../../../numerical-analysis.md#l-stability).

Linear [A-stability](../../../numerical-analysis.md#a-stability) does not by itself imply nonlinear [B-stability](../../../numerical-analysis.md#b-stability). The ODE [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule) has the same [stability function](../../../numerical-analysis.md#stability-function) as the [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule), but take the dissipative scalar field $f(y)=-\max(y,0)$ and $h=6$. For any positive starting value, its trapezoidal update is $y_{n+1}=y_n+3(f(y_n)+f(y_{n+1}))=-2y_n<0$. Thus two positive starting values have their distance doubled, violating [B-stability](../../../numerical-analysis.md#b-stability). Its [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) [matrix](../../../vector-space.md#matrix) also has a negative first diagonal entry. The field is globally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity), so this is a well-defined nonlinear counterexample.

These examples distinguish accuracy, scalar stiff-mode stability, nonlinear contraction, and rapid stiff-mode damping. For implicit methods, solvability of the stage equations remains an additional requirement; a formal [stability function](../../../numerical-analysis.md#stability-function) alone does not establish it for arbitrary nonlinear problems.

## 7

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

Consider a bounded [Lipschitz domain](../../../real-analysis.md#lipschitz-domain) $\Omega$ and homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) for

$$
-\nabla\cdot(A(x)\nabla u)+c(x)u=f.
$$

Assume $A$ is a bounded real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) field with $\xi^TA(x)\xi\geq a_0|\xi|^2$ uniformly, $c\geq0$ is bounded, and $f$ defines a bounded linear functional on $V=H_0^1(\Omega)$, the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space). The [weak formulation](../../../partial-differential-equation.md#weak-formulation) is

$$
a(u,v)=\ell(v)\quad(v\in V),\qquad
 a(u,v)=\int_\Omega\nabla v^TA\nabla u+cuv,\quad\ell(v)=\langle f,v\rangle.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives continuity $|a(u,v)|\leq M\|u\|_V\|v\|_V$. Uniform ellipticity and the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) give a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form), $a(v,v)\geq\alpha\|v\|_V^2$. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) therefore supplies a unique [weak solution](../../../partial-differential-equation.md#weak-solution), with $\|u\|_V\leq\|\ell\|_{V'}/\alpha$. Its proof represents $a$ by a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) $T$ using the [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem); coercivity gives an injective operator with closed image, and a zero [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) makes that image all of $V$. This yields existence, uniqueness and the displayed estimate.

For a [conforming finite element space](../../../numerical-analysis.md#conforming-finite-element-space) $V_h\subseteq V$, the [Galerkin method](../../../partial-differential-equation.md#galerkin-method) finds $u_h\in V_h$ such that $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$. With a basis $\phi_1,\ldots,\phi_N$, this is the linear system $KU=F$, where the [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) is $K_{ij}=a(\phi_j,\phi_i)$ and $F_i=\ell(\phi_i)$. Its [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) property proves unique discrete solvability. Local support gives a [sparse matrix](../../../vector-space.md#sparse-matrix) through elementwise assembly.

For the symmetric problem, the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) minimizes $J(v)=a(v,v)/2-\ell(v)$ over $V_h$. Differentiating in every direction $v_h$ gives precisely the [Galerkin method](../../../partial-differential-equation.md#galerkin-method) equations. Conversely, if $u_h$ solves them, $J(u_h+w_h)-J(u_h)=a(w_h,w_h)/2$, proving it is the unique minimum. The same argument over $V$ gives $J(v)-J(u)=\|v-u\|_a^2/2$, where $\|v\|_a=\sqrt{a(v,v)}$ is the [energy norm](../../../numerical-analysis.md#energy-norm). Thus the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) chooses the best trial function in that norm.

Subtracting the continuous and discrete equations gives [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality), $a(u-u_h,v_h)=0$. For arbitrary $v_h\in V_h$ and $e=u-u_h$, it follows that $a(e,e)=a(e,u-v_h)$. Coercivity and continuity prove the [Céa lemma](../../../numerical-analysis.md#cea-s-lemma):

$$
\alpha\|e\|_V^2\leq M\|e\|_V\|u-v_h\|_V,
\qquad
\|u-u_h\|_V\leq\frac M\alpha\inf_{v_h\in V_h}\|u-v_h\|_V.
$$

In the symmetric [energy norm](../../../numerical-analysis.md#energy-norm), the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) improves the constant to one. Equivalently, [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality) gives the [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) $\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2$. These estimates establish stability and show that approximation properties of the trial space determine convergence.

For continuous piecewise-linear elements on a [shape-regular mesh](../../../numerical-analysis.md#shape-regular-mesh) in dimensions at most three, a [finite element interpolation estimate](../../../numerical-analysis.md#finite-element-interpolation-estimate) gives $\|u-I_hu\|_{H^1}\leq Ch\|u\|_{H^2}$ when $u\in H^2(\Omega)$. Combining it with the [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) yields $O(h)$ [energy norm](../../../numerical-analysis.md#energy-norm) error. More generally, degree-$p$ elements give $O(h^p)$ error in $H^1$ under the corresponding regularity and approximation assumptions. Mere mesh refinement cannot supply an order whose required solution regularity is absent.

An additional order in the [L2 norm](../../../real-analysis.md#l2-norm) follows under a dual [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) assumption. Solve $a(v,z)=(e,v)_{L^2}$ and assume $\|z\|_{H^2}\leq C\|e\|_{L^2}$. The [Aubin–Nitsche duality argument](../../../numerical-analysis.md#aubin-nitsche-duality-argument) uses [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality) to obtain

$$
\|e\|_{L^2}^2=a(e,z-I_hz)\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Therefore $\|e\|_{L^2}\leq Ch\|e\|_{H^1}$, giving $O(h^2)$ for the piecewise-linear case with $u\in H^2$. This improvement explicitly requires regularity of the dual problem.

As a concrete example, solve $-u''=1$ on $(0,1)$ with zero endpoint values. On a uniform mesh of spacing $h$, the [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) give $K_{jj}=2/h$, $K_{j,j\pm1}=-1/h$ and $F_j=h$. The discrete equations are $2U_j-U_{j-1}-U_{j+1}=h^2$, whose solution is $U_j=x_j(1-x_j)/2$. The exact solution is $u(x)=x(1-x)/2$, so $u_h$ is its piecewise-linear nodal interpolant. On each interval $[x_j,x_{j+1}]$,

$$
u-u_h=\frac12(x-x_j)(x_{j+1}-x).
$$

Integrating the squared error and squared derivative error gives the explicit rates

$$
\boxed{\|u-u_h\|_{H_0^1}=\frac h{\sqrt{12}},\qquad\|u-u_h\|_{L^2}=\frac{h^2}{\sqrt{120}},}
$$

where the $H_0^1$ norm here is $\|v'\|_{L^2}$.

For nonsymmetric coercive problems, the [Galerkin method](../../../partial-differential-equation.md#galerkin-method), [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality) and the [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) still apply, but the symmetric quadratic minimization interpretation of the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) generally does not. Nonconforming trial spaces, inexact integration and noncoercive equations need additional arguments beyond the conforming coercive theory proved here.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
