# Paper 341

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_341.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_341.pdf)

**Table of contents**

- [Section A](#section-a)
  - [1](#section-a/1)
    - [a](#section-a/1/a)
      - [Solution](#section-a/1/a/solution)
    - [b](#section-a/1/b)
      - [Solution](#section-a/1/b/solution)
    - [c](#section-a/1/c)
      - [Solution](#section-a/1/c/solution)
  - [2](#section-a/2)
    - [a](#section-a/2/a)
      - [Solution](#section-a/2/a/solution)
    - [b](#section-a/2/b)
      - [Solution](#section-a/2/b/solution)
    - [c](#section-a/2/c)
      - [Solution](#section-a/2/c/solution)
  - [3](#section-a/3)
    - [a](#section-a/3/a)
      - [Solution](#section-a/3/a/solution)
    - [b](#section-a/3/b)
      - [Solution](#section-a/3/b/solution)
    - [c](#section-a/3/c)
      - [Solution](#section-a/3/c/solution)
  - [4](#section-a/4)
    - [a](#section-a/4/a)
      - [Solution](#section-a/4/a/solution)
    - [b](#section-a/4/b)
      - [Solution](#section-a/4/b/solution)
    - [c](#section-a/4/c)
      - [Solution](#section-a/4/c/solution)
  - [5](#section-a/5)
    - [a](#section-a/5/a)
      - [Solution](#section-a/5/a/solution)
    - [b](#section-a/5/b)
      - [Solution](#section-a/5/b/solution)
    - [c](#section-a/5/c)
      - [Solution](#section-a/5/c/solution)
    - [d](#section-a/5/d)
      - [Solution](#section-a/5/d/solution)
- [Section B](#section-b)
  - [6](#section-b/6)
    - [Solution](#section-b/6/solution)
  - [7](#section-b/7)
    - [Solution](#section-b/7/solution)

## Section A

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="section-a/1">1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/1/a">a</h4>

↑ **Parent:** [1](#section-a/1)

<h5 id="section-a/1/a/solution">Solution</h5>

↑ **Parent:** [A](#section-a/1/a)

Substitute the exact solution and expand every value about $t_n$. The coefficient of $h^q y^{(q)}(t_n)$ in the defect is zero for $q=0,\ldots,p$ exactly when

$$
\boxed{\sum_{k=0}^s\rho_k=0,\qquad
\sum_{k=0}^sk^q\rho_k
=q\left[s^{q-1}\sigma_s+(s-1)^{q-1}\sigma_{s-1}\right]
\quad(1\leq q\leq p).}
$$

These are the [order conditions for a linear multistep method](../../../numerical-analysis.md#order-conditions-for-a-linear-multistep-method), specialized to the two nonzero derivative coefficients. The first failed identity determines the leading [local truncation error](../../../numerical-analysis.md#local-truncation-error).

<h4 id="section-a/1/b">b</h4>

↑ **Parent:** [1](#section-a/1)

<h5 id="section-a/1/b/solution">Solution</h5>

↑ **Parent:** [B](#section-a/1/b)

For $s=1$, imposing order two gives

$$
\rho_0=-1,
\qquad \sigma_0=\sigma_1=\frac12.
$$

The method is therefore the [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule)

$$
y_{n+1}-y_n=\frac h2(f_{n+1}+f_n).
$$

Its first [characteristic polynomial](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) is $\rho(\zeta)=\zeta-1$, so it satisfies the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method).

For $s=2$, the four conditions through order three give

$$
\rho_0=-\frac15,
\qquad \rho_1=-\frac45,
\qquad \sigma_1=\frac45,
\qquad \sigma_2=\frac25,
$$

and hence

$$
y_{n+2}-\frac45y_{n+1}-\frac15y_n
=h\left(\frac25f_{n+2}+\frac45f_{n+1}\right).
$$

Here

$$
\rho(\zeta)=\zeta^2-\frac45\zeta-\frac15
=(\zeta-1)\left(\zeta+\frac15\right),
$$

so the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) again holds. Both methods are consistent and zero-stable, and the [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) therefore proves that both are convergent.

<h4 id="section-a/1/c">c</h4>

↑ **Parent:** [1](#section-a/1)

<h5 id="section-a/1/c/solution">Solution</h5>

↑ **Parent:** [C](#section-a/1/c)

A highest-order method in this family has order $s+1$. The [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier) says that an irreducible [A-stable](../../../numerical-analysis.md#a-stability) multistep method has order at most two, so $s+1\leq2$ and hence $s=1$. Part b then leaves only the [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule). Its amplification factor is

$$
R(z)=\frac{1+z/2}{1-z/2},
$$

and $|R(z)|\leq1$ whenever $\operatorname{Re}z\leq0$. Thus the trapezoidal rule is the unique highest-order A-stable method of the stated form, apart from representations containing removable common factors.

<h3 id="section-a/2">2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/2/a">a</h4>

↑ **Parent:** [2](#section-a/2)

<h5 id="section-a/2/a/solution">Solution</h5>

↑ **Parent:** [A](#section-a/2/a)

For the nodes $c_1=\alpha$ and $c_2=1$, the [Lagrange basis](../../../numerical-analysis.md#lagrange-polynomial) is

$$
\ell_1(t)=\frac{1-t}{1-\alpha},
\qquad
\ell_2(t)=\frac{t-\alpha}{1-\alpha}.
$$

Direct integration gives

$$
a_{ij}=\int_0^{c_i}\ell_j(t)\,dt
$$

and therefore

$$
A=\begin{pmatrix}
\dfrac{\alpha(2-\alpha)}{2(1-\alpha)}&-\dfrac{\alpha^2}{2(1-\alpha)}\\[6pt]
\dfrac1{2(1-\alpha)}&\dfrac{1-2\alpha}{2(1-\alpha)}
\end{pmatrix}.
$$

The [collocation Runge-Kutta method](../../../numerical-analysis.md#collocation-runge-kutta-method) also requires

$$
b_j=\int_0^1\ell_j(t)\,dt,
\qquad
b^T=\left(\frac1{2(1-\alpha)},\frac{1-2\alpha}{2(1-\alpha)}\right).
$$

This exposes a sign error in the printed tableau: its lower-right entry is shown as $(-1+2\alpha)/[2(1-\alpha)]$. With $1-2\alpha$ in that position, the tableau is exactly the claimed collocation method. Taken literally, the printed weights satisfy $b^T\mathbf1=\alpha/(1-\alpha)$, so the method is not even consistent unless $\alpha=1/2$ and cannot be a collocation method for general $\alpha$.

<h4 id="section-a/2/b">b</h4>

↑ **Parent:** [2](#section-a/2)

<h5 id="section-a/2/b/solution">Solution</h5>

↑ **Parent:** [B](#section-a/2/b)

For the intended collocation weights, interpolation makes the associated [quadrature rule](../../../numerical-analysis.md#quadrature-rule) exact for every polynomial of degree at most one, so the method has order at least two. It has order at least three precisely when the node polynomial is orthogonal to constants:

$$
0=\int_0^1(t-\alpha)(t-1)\,dt
=\frac\alpha2-\frac16.
$$

Thus

$$
\boxed{p=3\text{ when }\alpha=\frac13,
\qquad p=2\text{ for every other }\alpha\ne1.}
$$

At $\alpha=1/3$ this is the two-stage [Radau IIA method](../../../numerical-analysis.md#radau-iia-method). Since one node is fixed at the endpoint, no value of $\alpha$ makes the two-node quadrature exact through degree three, so order four cannot occur.

For completeness, the tableau exactly as printed has order zero when $\alpha\ne1/2$, since $b^T\mathbf1\ne1$. At $\alpha=1/2$ the two signs coincide because the second weight vanishes, and the resulting method has order two.

<h4 id="section-a/2/c">c</h4>

↑ **Parent:** [2](#section-a/2)

<h5 id="section-a/2/c/solution">Solution</h5>

↑ **Parent:** [C](#section-a/2/c)

For [algebraic stability of a Runge-Kutta method](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method), the weights must be nonnegative and

$$
M=BA+A^TB-bb^T,
\qquad B=\operatorname{diag}(b_1,b_2),
$$

must be [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix). With the intended collocation weights,

$$
\det M=-\frac{(3\alpha-1)^2}{16(\alpha-1)^2}.
$$

Positive semidefiniteness is therefore possible only at $\alpha=1/3$; substitution gives nonnegative weights and a positive-semidefinite $M$. Hence the intended family is algebraically stable exactly when

$$
\boxed{\alpha=\frac13.}
$$

With the sign printed in the paper, one instead obtains

$$
M_{22}=-\frac{3(2\alpha-1)^2}{4(\alpha-1)^2}\leq0.
$$

Equality forces $\alpha=1/2$, where $M$ still has nonzero off-diagonal entries and is indefinite. The literal printed tableau is consequently algebraically stable for no value of $\alpha$.

<h3 id="section-a/3">3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/3/a">a</h4>

↑ **Parent:** [3](#section-a/3)

<h5 id="section-a/3/a/solution">Solution</h5>

↑ **Parent:** [A](#section-a/3/a)

Write $H=\partial_x^2-V(x)$. The real potential and [periodic boundary condition](../../../differential-equation.md#periodic-boundary-conditions) make $H$ a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) on the periodic domain. Since $u_t=-iHu$,

$$
\frac d{dt}\|u(t)\|_{L^2}^2
=2\operatorname{Re}\langle u,u_t\rangle
=2\operatorname{Re}\bigl(-i\langle u,Hu\rangle\bigr)=0,
$$

because the [inner product](../../../linear-algebra.md#inner-product) $\langle u,Hu\rangle$ is real. Thus the [Schrödinger equation](../../../physics.md#schrodinger-equation) preserves the $L^2$ norm.

<h4 id="section-a/3/b">b</h4>

↑ **Parent:** [3](#section-a/3)

<h5 id="section-a/3/b/solution">Solution</h5>

↑ **Parent:** [B](#section-a/3/b)

Let $H_h$ be the periodic centered second-difference matrix minus the real diagonal matrix containing $V(x_m)$. It is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), so the [semidiscrete system](../../../finite-difference.md#method-of-lines) is

$$
\mathbf u'=-iH_h\mathbf u
$$

with a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix) generator. Consequently

$$
\frac d{dt}\|\mathbf u(t)\|_2^2
=2\operatorname{Re}\langle\mathbf u,-iH_h\mathbf u\rangle=0.
$$

Its exact propagator $e^{-itH_h}$ is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix), and therefore the semidiscretization is stable in the discrete $2$-norm, uniformly for all times and mesh sizes.

<h4 id="section-a/3/c">c</h4>

↑ **Parent:** [3](#section-a/3)

<h5 id="section-a/3/c/solution">Solution</h5>

↑ **Parent:** [C](#section-a/3/c)

Apply the [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule), equivalently the [Crank-Nicolson method](../../../numerical-analysis.md#crank-nicolson-method), to the semidiscrete equation:

$$
i\frac{\mathbf u^{n+1}-\mathbf u^n}{\Delta t}
=H_h\frac{\mathbf u^{n+1}+\mathbf u^n}{2}.
$$

It has order two. Its amplification matrix is the [Cayley transform](../../../linear-operator-theory.md#cayley-transform-of-a-hermitian-matrix)

$$
Q=\left(I+\frac{i\Delta t}{2}H_h\right)^{-1}
\left(I-\frac{i\Delta t}{2}H_h\right).
$$

Because $H_h$ is Hermitian, $Q$ is unitary. Hence $\|\mathbf u^{n+1}\|_2=\|\mathbf u^n\|_2$ exactly.

<h3 id="section-a/4">4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/4/a">a</h4>

↑ **Parent:** [4](#section-a/4)

<h5 id="section-a/4/a/solution">Solution</h5>

↑ **Parent:** [A](#section-a/4/a)

A real [linear operator](../../../vector-space.md#linear-operator) $\mathcal L$ on an [inner product space](../../../linear-algebra.md#inner-product-space) is a [positive-definite operator](../../../linear-operator-theory.md#positive-definite-operator) when it is self-adjoint and

$$
\langle\mathcal Lu,u\rangle>0
$$

for every nonzero $u$ in its domain. In the variational setting one normally requires the stronger uniform estimate $\langle\mathcal Lu,u\rangle\geq c\|u\|_V^2$ for some $c>0$, which is [coercivity](../../../real-analysis.md#coercive-function).

<h4 id="section-a/4/b">b</h4>

↑ **Parent:** [4](#section-a/4)

<h5 id="section-a/4/b/solution">Solution</h5>

↑ **Parent:** [B](#section-a/4/b)

Choose the [Sobolev space](../../../sobolev-space.md) $V$ encoding the homogeneous essential [boundary conditions](../../../differential-equation.md#boundary-condition), set

$$
a(u,v)=\langle\mathcal Lu,v\rangle,
\qquad \ell(v)=\langle f,v\rangle,
$$

after the appropriate [integration by parts](../../../calculus.md#integration-by-parts), and define the [energy functional](../../../calculus-of-variations.md#energy-functional)

$$
J(v)=\frac12a(v,v)-\ell(v).
$$

Its first variation is $J'(u)v=a(u,v)-\ell(v)$, so its stationary points are exactly the solutions of the [weak formulation](../../../partial-differential-equation.md#weak-formulation)

$$
a(u,v)=\ell(v)\qquad(v\in V).
$$

If $a$ is bounded, symmetric, and coercive and $\ell\in V'$, the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) supplies a unique [weak solution](../../../partial-differential-equation.md#weak-solution) $u$. Moreover, for every $w\in V$,

$$
J(u+w)-J(u)
=a(u,w)-\ell(w)+\frac12a(w,w)
=\frac12a(w,w)>0
$$

unless $w=0$. Thus $J$ is [strictly convex](../../../real-analysis.md#strictly-convex-function), and $u$ is its unique global minimizer. This proves existence and uniqueness of the minimizer and of the weak solution simultaneously.

<h4 id="section-a/4/c">c</h4>

↑ **Parent:** [4](#section-a/4)

<h5 id="section-a/4/c/solution">Solution</h5>

↑ **Parent:** [C](#section-a/4/c)

Let $\Omega=(-1,1)^2$ and use the clamped energy space $V=H_0^2(\Omega)$, whose traces satisfy $u=\partial_nu=0$ on $\partial\Omega$. Two applications of [integration by parts](../../../calculus.md#integration-by-parts) give

$$
\langle\Delta^2u,u\rangle_{L^2}
=\int_\Omega(\Delta u)^2\,dx\,dy\geq0.
$$

If equality holds, then $\Delta u=0$. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) and the zero [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) imply $u=0$. The [biharmonic operator](../../../calculus.md#biharmonic-operator) is therefore positive definite. The same identity and conclusion hold for the simply supported conditions $u=\Delta u=0$; either standard interpretation of the paper's phrase “zero boundary conditions” gives the result.

<h3 id="section-a/5">5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/5/a">a</h4>

↑ **Parent:** [5](#section-a/5)

<h5 id="section-a/5/a/solution">Solution</h5>

↑ **Parent:** [A](#section-a/5/a)

Near $t=0$, take $\Omega(t)=\log F(t)$ to be the continuous local [matrix logarithm](../../../vector-space.md#matrix-logarithm) with $\Omega(0)=0$. The symmetry identity gives $F(-t)=F(t)^{-1}$, and uniqueness of this logarithm yields

$$
\Omega(-t)=\log(F(t)^{-1})=-\log F(t)=-\Omega(t).
$$

**Thus $\Omega$ is an [odd function](../../../calculus.md#odd-function). The local-logarithm qualification is necessary because the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is not globally injective; the statement is naturally understood either near $t=0$ or as an identity of formal power series.**

<h4 id="section-a/5/b">b</h4>

↑ **Parent:** [5](#section-a/5)

<h5 id="section-a/5/b/solution">Solution</h5>

↑ **Parent:** [B](#section-a/5/b)

For the [Strang splitting](../../../numerical-analysis.md#strang-splitting)

$$
F(t)=e^{tA/2}e^{tB}e^{tA/2},
$$

reversing $t$ reverses all three factors, so

$$
F(-t)=e^{-tA/2}e^{-tB}e^{-tA/2}=F(t)^{-1}.
$$

It is therefore a [time-symmetric numerical method](../../../numerical-analysis.md#time-symmetric-numerical-method). Multiplication of the three [exponential](../../../linear-operator-theory.md#matrix-exponential) series shows agreement with $e^{t(A+B)}$ through degree two. Equivalently, the [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula) gives an odd modified generator

$$
\log F(t)=t(A+B)+t^3D+O(t^5)
$$

for a matrix $D$ made from nested [commutators](../../../lie-algebra.md#commutator). Exponentiating gives

$$
\boxed{F(t)=e^{t(A+B)}+Ct^3+O(t^4)}
$$

for a matrix $C$ depending on $A$ and $B$.

<h4 id="section-a/5/c">c</h4>

↑ **Parent:** [5](#section-a/5)

<h5 id="section-a/5/c/solution">Solution</h5>

↑ **Parent:** [C](#section-a/5/c)

The three substeps have total length $2\alpha+(1-2\alpha)=1$. Their leading cubic defects add, so cancellation requires

$$
2\alpha^3+(1-2\alpha)^3=0.
$$

Taking the real cube root and solving gives

$$
\boxed{\alpha=\frac1{2-2^{1/3}}.}
$$

This is the coefficient in the [higher-order composition of a symmetric splitting](../../../numerical-analysis.md#higher-order-composition-of-a-symmetric-splitting); the middle substep $1-2\alpha$ is negative.

<h4 id="section-a/5/d">d</h4>

↑ **Parent:** [5](#section-a/5)

<h5 id="section-a/5/d/solution">Solution</h5>

↑ **Parent:** [D](#section-a/5/d)

The composition is palindromic, and hence

$$
G_\alpha(-t)=F(-\alpha t)F(-(1-2\alpha)t)F(-\alpha t)
=G_\alpha(t)^{-1}.
$$

Thus $G_\alpha$ is symmetric. Part c cancels the cubic term in its odd [formal logarithm](../../../normalization-of-an-algebraic-curve.md#formal-logarithm); symmetry forbids a fourth-degree term, so the next possible defect has degree five. Therefore

$$
\boxed{G_\alpha(t)=e^{t(A+B)}+O(t^5),}
$$

which makes the composition a fourth-order method.

## Section B

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="section-b/6">6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/6/solution">Solution</h4>

↑ **Parent:** [6](#section-b/6)

An $s$-stage [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) has stages and update

$$
Y_i=y_n+h\sum_{j=1}^sa_{ij}f(Y_j),
\qquad
y_{n+1}=y_n+h\sum_{i=1}^sb_if(Y_i).
$$

On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$, elimination of the stages gives the [stability function](../../../numerical-analysis.md#stability-function)

$$
R(z)=1+z b^T(I-zA)^{-1}\mathbf1,
\qquad z=h\lambda.
$$

The [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) is the set where $|R(z)|\leq1$. A method is [A-stable](../../../numerical-analysis.md#a-stability) when this domain contains $\operatorname{Re}z\leq0$, so every exactly decaying scalar linear mode remains bounded for every step size. It is [L-stable](../../../numerical-analysis.md#l-stability) when it is A-stable and $R(z)\to0$ as $|z|\to\infty$ in the left half-plane; this extra limit strongly damps unresolved stiff modes.

The rational function $R$ makes several useful conclusions immediate. No explicit Runge--Kutta method is A-stable because its stability function is a nonconstant [polynomial](../../../polynomial.md) and is therefore unbounded on the negative real axis. The [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) has $R(z)=(1+z/2)/(1-z/2)$ and is A-stable, but $R(z)\to-1$, so it is not L-stable. The [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $R(z)=(1-z)^{-1}$ and is L-stable. More generally, a rational $R$ with no pole in the closed left half-plane is A-stable if and only if $|R(iy)|\leq1$ for every real $y$; this follows by applying the [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) on expanding left half-disks.

Scalar linear stability does not by itself control nonlinear perturbations. Suppose the vector field is dissipative in the sense that

$$
\operatorname{Re}\langle f(u)-f(v),u-v\rangle\leq0.
$$

A method is [B-stable](../../../numerical-analysis.md#b-stability) if it preserves the resulting contractivity: two numerical solutions satisfy $\|y_{n+1}-\widetilde y_{n+1}\|\leq\|y_n-\widetilde y_n\|$. A practical sufficient condition is [algebraic stability of a Runge-Kutta method](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method): $b_i\geq0$ and

$$
M=BA+A^TB-bb^T\succeq0,
\qquad B=\operatorname{diag}(b_i).
$$

To prove the implication, let $D_i=Y_i-\widetilde Y_i$ and $F_i=f(Y_i)-f(\widetilde Y_i)$. Expanding the squared distance and substituting the stage equations gives the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity)

$$
\|y_{n+1}-\widetilde y_{n+1}\|^2
=\|y_n-\widetilde y_n\|^2
+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

The dissipativity inequalities make the middle sum nonpositive, and positive semidefiniteness of $M$ makes the final quadratic form nonnegative before its minus sign. The distance therefore cannot increase. In particular, algebraic stability implies B-stability and, by applying contractivity to the real two-dimensional form of $y'=\lambda y$, implies A-stability.

Important collocation families illustrate these notions. [Gauss methods](../../../numerical-analysis.md#gauss-legendre-method) are A-stable, symmetric, and have order $2s$, but they do not damp infinitely stiff modes. [Radau IIA methods](../../../numerical-analysis.md#radau-iia-method) have order $2s-1$, are algebraically stable, and are L-stable. These properties explain why A-stability controls unrestricted linear decay, L-stability is useful for stiff transients, and algebraic or B-stability is the stronger tool for nonlinear dissipative equations.

<h3 id="section-b/7">7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/7/solution">Solution</h4>

↑ **Parent:** [7](#section-b/7)

Consider first a scalar constant-coefficient [Cauchy problem for a partial differential equation](../../../partial-differential-equation.md#cauchy-problem) on the whole line. A translation-invariant spatial discretization is a convolution operator, so the [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform) turns it into multiplication by its Fourier symbol. This reduction is exact because Fourier modes are the simultaneous generalized eigenfunctions of every translation-invariant stencil.

For a fully discrete one-step method

$$
u^{n+1}=Q_hu^n,
$$

write $H_h(\theta)$ for its [amplification factor](../../../finite-difference.md#amplification-factor). The [Parseval identity](../../../fourier-analysis.md#parseval-identity) gives

$$
\|Q_h^nu^0\|_2^2
=\int_{-\pi}^{\pi}|H_h(\theta)|^{2n}|\widehat u^0(\theta)|^2\,d\theta.
$$

Consequently the exact necessary and sufficient condition for stability on every bounded time interval $0\leq n\Delta t\leq T$ is

$$
\boxed{\operatorname*{ess\,sup}_\theta|H_h(\theta)|
\leq e^{C\Delta t}}
$$

with $C$ independent of the mesh. Sufficiency follows directly from Parseval; necessity follows by choosing transformed initial data concentrated where the multiplier is largest. For a contractive scheme one can take $C=0$, yielding the familiar [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis) condition $|H_h(\theta)|\leq1$.

For a semidiscretization $u_t=A_hu$ with scalar symbol $a_h(\theta)$, the corresponding exact criterion is

$$
\boxed{\operatorname*{ess\,sup}_\theta\operatorname{Re}a_h(\theta)\leq C.}
$$

Indeed, the Fourier multiplier of the solution operator is $e^{ta_h(\theta)}$. For systems, eigenvalues alone cease to be sufficient when the matrix symbol is [non-normal](../../../linear-operator-theory.md#non-normal-matrix); the necessary and sufficient statement is the uniform bound $\|e^{tA_h(\theta)}\|\leq C_T$.

On the whole lattice, a finite stencil defines a [Laurent operator](../../../finite-difference.md#laurent-operator), whose operator norm is the essential supremum of its symbol. Restricting the same stencil to a half-line gives a [Toeplitz operator](../../../finite-difference.md#toeplitz-operator). The Cauchy symbol condition remains necessary for a stable initial-boundary scheme because data localized far from the boundary behave like the whole-line problem for a finite time. It is not sufficient: the boundary closure can support growing modes or amplify incoming modes even when every interior Fourier mode is stable.

Boundary stability therefore requires a uniform estimate for the forced half-line recurrence. After a Laplace transform in time and a Fourier transform in tangential variables, one solves a normal-direction recurrence. The [Uniform Kreiss--Lopatinskii condition](../../../finite-difference.md#uniform-kreiss-lopatinskii-condition) requires the boundary equations to determine its decaying roots with a uniformly bounded inverse. In practical terms, one imposes one independent boundary condition for each incoming characteristic or numerical mode and none for outgoing modes. The [group velocity](../../../wave-equation.md#group-velocity) $d\omega/dk$ identifies the direction in which a narrow [wave packet](../../../wave-equation.md#wave-packet) carries energy, so its sign helps determine which boundary is inflow and explains why a numerically generated high-frequency branch can require a boundary condition different from that suggested by its phase velocity.

For a two-step method, the Fourier substitution produces an [amplification polynomial of a multilevel finite difference scheme](../../../finite-difference.md#amplification-polynomial-of-a-multilevel-finite-difference-scheme). Every root must lie in the closed unit disk, and unit-modulus roots must be simple, uniformly in the wavenumber. For example, leapfrog differencing of $u_t+cu_x=0$ gives

$$
u_j^{n+1}=u_j^{n-1}-\nu(u_{j+1}^n-u_{j-1}^n),
\qquad \nu=\frac{c\Delta t}{\Delta x},
$$

and hence

$$
G^2+2i\nu\sin\theta\,G-1=0.
$$

The roots have unit modulus when $|\nu\sin\theta|\leq1$, giving the usual [Courant](../../../finite-difference.md#courant-number) restriction $|\nu|\leq1$. At the endpoint, a wavenumber with $|\nu\sin\theta|=1$ produces a repeated unit root and violates the uniform root condition; strict $|\nu|<1$ avoids this marginal linear growth. The second root is the familiar oscillatory computational mode, illustrating why a multilevel scheme requires its full amplification polynomial rather than a single multiplier.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
