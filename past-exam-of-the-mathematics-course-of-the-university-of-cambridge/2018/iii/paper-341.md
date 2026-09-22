# Paper 341

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_341.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_341.pdf)

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

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a fixed-step [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) with a nonzero leading coefficient, applied to an [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) with a locally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) vector field, the [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) states that

$$
\boxed{\text{convergence}\ \Longleftrightarrow\
\text{consistency and zero-stability}.}
$$

Here convergence is uniform on each fixed finite time interval as the [step size](../../../convex-optimization.md#step-size) tends to zero, for every set of starting values tending to the corresponding exact values. [Consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) means that the normalized local defect tends to zero; for the [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) it gives $\rho(1)=0$ and $\rho'(1)=\sigma(1)$. [Zero-stability](../../../numerical-analysis.md#zero-stability) is equivalent to the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method): every [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) $\xi$ of $\rho$ satisfies $|\xi|\leq1$, and roots with $|\xi|=1$ are simple. Order $p\geq1$, together with [zero-stability](../../../numerical-analysis.md#zero-stability) and starting errors $O(h^p)$, gives [global error](../../../numerical-analysis.md#global-discretization-error) $O(h^p)$ under the usual smoothness assumptions.

To prove the [necessity of the root condition for multistep convergence](../../../numerical-analysis.md#necessity-of-the-root-condition-for-multistep-convergence), use the test problem $y'=0$, $y(0)=0$. Its discrete error satisfies $\rho(E)e_n=0$, where $Ee_n=e_{n+1}$. Set $h=T/N$. If $|\xi|>1$, the exact recurrence solution

$$
e_n=|\xi|^{-N}\xi^n
$$

has starting errors tending to zero at every fixed starting index, but $|e_N|=1$. Thus convergence fails.

If a unit-modulus root has multiplicity $m\geq2$, the recurrence instead admits

$$
e_n=N^{-(m-1)}n^{m-1}\xi^n.
$$

Again every fixed starting error tends to zero while $|e_N|=1$. These polynomial-times-exponential solutions follow from the repeated factor $(E-\xi)^m$. Complex modes can be interpreted as a real two-component system, or their real and imaginary parts can be used. Therefore **convergence requires precisely the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method)**. Repeated roots strictly inside the unit disk are allowed, since their polynomial factors are dominated by exponential decay.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Factor the first [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) as

$$
\rho(w)=(w-1)(w^2-2\alpha w+1).
$$

The other two [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) have product one. If $-1<\alpha<1$, they are $\alpha\pm i\sqrt{1-\alpha^2}$: distinct unit-modulus roots, both different from one. At $\alpha=-1$, the root $-1$ is double; at $\alpha=1$, the root one is triple. Outside $[-1,1]$, one of the reciprocal real roots has modulus greater than one. Thus the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) holds exactly for $-1<\alpha<1$.

For the [order conditions for a linear multistep method](../../../numerical-analysis.md#order-conditions-for-a-linear-multistep-method), expand the exponential defect:

$$
\rho(e^z)-z\sigma(e^z)
=\frac{11-5\alpha}{6}z^3+\frac{13-7\alpha}{4}z^4+O(z^5).
$$

The constant, linear and quadratic coefficients vanish for every $\alpha$. The cubic coefficient vanishes only at $\alpha=11/5$, where the quartic coefficient is $-3/5\neq0$. Consequently the formal order is

$$
\boxed{p=\begin{cases}3,&\alpha=11/5,\\2,&\alpha\neq11/5.\end{cases}}
$$

For all parameters satisfying the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method), $\rho'(1)=\sigma(1)=2(1-\alpha)\neq0$, so this formal calculation gives ordinary second-order [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method). The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) therefore yields

$$
\boxed{\text{the method is convergent exactly when }-1<\alpha<1.}
$$

The exceptional third-order formula is not [zero-stable](../../../numerical-analysis.md#zero-stability). At $\alpha=1$, $\sigma\equiv0$ and $\rho=(w-1)^3$: the recurrence contains no vector-field evaluations. It satisfies the displayed Taylor identities only formally and is **a degenerate, nonconvergent formula**, not a usable second-order ODE solver. This distinction avoids interpreting formal cancellation as convergence.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Only $-1<\alpha<1$ needs consideration. On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), the [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) is $P_z(w)=\rho(w)-z\sigma(w)$, where $z=h\lambda$. [A-stability](../../../numerical-analysis.md#a-stability) requires all amplification roots to have modulus at most one for every $\operatorname{Re}z\leq0$, with simple unit-modulus roots.

Choose the negative real value $z=-2/(1-\alpha)$. The leading coefficient of $P_z$ is

$$
1-z(\alpha-1)=-1,
$$

whereas $P_z(1)=-z\sigma(1)=4>0$. Hence $P_z(w)\to-\infty$ as real $w\to+\infty$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) supplies a real amplification root $w>1$, so this negative test value is unstable. Therefore

$$
\boxed{\text{no parameter makes the method both convergent and A-stable}.}
$$

This is a direct [absolute stability](../../../numerical-analysis.md#linear-stability-domain) obstruction, independent of the [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier), which by itself would not rule out the convergent second-order members.

## 2

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The nodes $0,1/2,1$ have [Lagrange interpolation polynomials](../../../numerical-analysis.md#lagrange-polynomial)

$$
\ell_1(s)=2s^2-3s+1,\quad
\ell_2(s)=4s-4s^2,\quad
\ell_3(s)=2s^2-s.
$$

The coefficients obtained from $a_{ij}=\int_0^{c_i}\ell_j(s)\,ds$ and $b_j=\int_0^1\ell_j(s)\,ds$ reproduce the given [Butcher tableau](../../../numerical-analysis.md#butcher-tableau). In particular, the second row's last entry is $-1/24$, which is missing from the TeX transcription. Thus this is the three-stage [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method).

One applicable collocation theorem is that $s$-stage Lobatto IIIA collocation has order $2s-2$. Alternatively, the [fourth-order conditions for a Runge-Kutta method](../../../numerical-analysis.md#fourth-order-conditions-for-a-runge-kutta-method) give a direct verification. With $e=(1,1,1)^T$, $c=Ae$ and $C=\operatorname{diag}(c)$, the eight required [Butcher order conditions](../../../numerical-analysis.md#butcher-order-condition) are

$$
\begin{gathered}
b^Te=1,\quad b^Tc=\tfrac12,\quad b^Tc^2=\tfrac13,\quad b^TAc=\tfrac16,\\
b^Tc^3=\tfrac14,\quad b^TCAc=\tfrac18,\quad
b^TAc^2=\tfrac1{12},\quad b^TA^2c=\tfrac1{24}.
\end{gathered}
$$

Powers of $c$ here are componentwise. Substitution satisfies all eight. The [stability function](../../../numerical-analysis.md#stability-function) computed from the stages is

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}.
$$

Its expansion satisfies $R(z)-e^z=-z^5/720+O(z^6)$, so even the scalar linear problem fails the fifth-order condition. Hence

$$
\boxed{p=4.}
$$

The [Butcher order condition](../../../numerical-analysis.md#butcher-order-condition) theorem equates order $p$ with all conditions for [rooted trees](../../../combinatorics.md#rooted-tree) through order $p$; the displayed conditions are its complete specialization through order four.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the [stability function](../../../numerical-analysis.md#stability-function) $R(z)=(z^2+6z+12)/(z^2-6z+12)$. Its denominator vanishes only at $3\pm i\sqrt3$, both in the open right half-plane. For $z=x+iy$,

$$
|z^2-6z+12|^2-|z^2+6z+12|^2
=-24x(|z|^2+12).
$$

This is nonnegative whenever $x\leq0$, so $|R(z)|\leq1$ throughout the closed left half-plane. The internal stage equations are also solvable there, since $\det(I-zA)=1-z/2+z^2/12$. Therefore **the method is [A-stable](../../../numerical-analysis.md#a-stability)**.

The inequality is strict in the open left half-plane, while $|R(iy)|=1$. Moreover $R(z)\to1$ as $|z|\to\infty$, so the method is **not [L-stable](../../../numerical-analysis.md#l-stability)**. These conclusions follow directly from the definitions of [A-stability](../../../numerical-analysis.md#a-stability) and [L-stability](../../../numerical-analysis.md#l-stability), rather than from the order of the method.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For [algebraic stability of a Runge-Kutta method](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method), the weights must be nonnegative and

$$
M=BA+A^TB-bb^T,\qquad B=\operatorname{diag}(b),
$$

must be a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). Here all weights are positive, but direct calculation gives

$$
M=\frac1{36}\begin{pmatrix}-1&1&0\\1&0&-1\\0&-1&1\end{pmatrix}.
$$

In particular $e_1^TMe_1=-1/36<0$; equivalently, its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $0,\pm\sqrt3/36$. Therefore **the method is not [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method)**. This does not contradict its [A-stability](../../../numerical-analysis.md#a-stability): [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) is a stronger condition designed to guarantee nonlinear [B-stability](../../../numerical-analysis.md#b-stability) through the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity).

## 3

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The original PDF puts both neighbouring values at time $n+1$. Thus the actual scheme is [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) in time with a centered three-point approximation to the second spatial derivative. The old-time neighbours in the TeX transcription describe a different method.

Let $h=\Delta x$ and $k=\Delta t$. Insert a sufficiently smooth exact solution and divide by $k$. Expanding at $(x_m,t_{n+1})$ gives

$$
\frac{u(x_m,t_{n+1})-u(x_m,t_n)}k
-\frac{u(x_m-h,t_{n+1})-2u(x_m,t_{n+1})+u(x_m+h,t_{n+1})}{h^2}
=-\frac{k}{2}u_{tt}-\frac{h^2}{12}u_{xxxx}+O(k^2+h^4).
$$

The PDE cancels the $u_t-u_{xx}$ term. Therefore the normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) is $O(k+h^2)$ and

$$
\boxed{\text{first order in time and second order in space}.}
$$

For compatible smooth data with exact nodal initialization, the [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) established below gives [global error](../../../numerical-analysis.md#global-discretization-error) $O(k+h^2)$ on fixed time intervals, by summing the one-step defects with the contraction bound. Thus no relation between $k$ and $h$ is needed for stability; choosing $k=O(h^2)$ makes both consistency contributions $O(h^2)$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $T$ be the $M\times M$ [tridiagonal matrix](../../../vector-space.md#tridiagonal-matrix) with diagonal two and adjacent entries minus one, incorporating zero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition). The actual PDF scheme is

$$
U^{n+1}=G_\mu U^n,\qquad G_\mu=(I+\mu T)^{-1}.
$$

An [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector) of $T$ has components $\sqrt{2/(M+1)}\sin(jm\pi/(M+1))$, and substitution gives

$$
\lambda_j=2-2\cos\frac{j\pi}{M+1}
=4\sin^2\frac{j\pi}{2(M+1)}>0,\qquad 1\leq j\leq M.
$$

They form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) by the [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices). Hence $I+\mu T$ is invertible for every $\mu>0$, and the amplification [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $g_j=(1+\mu\lambda_j)^{-1}\in(0,1)$. For the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm) $\|U\|_h^2=h\sum_m|U_m|^2$,

$$
\boxed{\|G_\mu^n U\|_h\leq\|U\|_h\quad\text{for all }n\geq0,\ \mu>0.}
$$

This bound has constant one independent of time step and mesh, which is the required [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method). Therefore **every positive [Courant number](../../../finite-difference.md#courant-number) is stable**. If a forcing or local-defect sequence is added, the discrete [variation-of-constants formula](../../../functional-analysis.md#variation-of-constants-formula) gives a bound by the initial [norm](../../../functional-analysis.md#norm) plus the sum of those perturbation [norms](../../../functional-analysis.md#norm); this also justifies the [global error](../../../numerical-analysis.md#global-discretization-error) conclusion in part (a).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use $N$ distinct periodic grid points $x_m=m/N$, $0\leq m<N$, and $h=1/N$. Values at the two ends of the interval represent the same point, so the endpoint must not be stored twice. With indices interpreted modulo $N$, set

$$
\boxed{(1+2\mu)U_m^{n+1}
-\mu(U_{m-1}^{n+1}+U_{m+1}^{n+1})=U_m^n.}
$$

This replaces the Dirichlet matrix by the periodic discrete Laplacian. The normalized [Fourier modes](../../../fourier-analysis.md#fourier-mode) $N^{-1/2}e^{2\pi ijm/N}$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) and have amplification factors

$$
\boxed{g_j=\frac1{1+4\mu\sin^2(\pi j/N)},\qquad 0\leq j<N.}
$$

Each satisfies $0<g_j\leq1$ for every $\mu>0$. The [Parseval identity](../../../fourier-analysis.md#parseval-identity) therefore gives $\|U^{n+1}\|_h\leq\|U^n\|_h$ in the [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm), uniformly in the grid and time step. Thus **all positive [Courant numbers](../../../finite-difference.md#courant-number) remain stable**. The constant mode has $g_0=1$, expressing preservation of the spatial mean; all nonconstant modes decay. The formula with modulo indices also handles small grids, where two neighbours can coincide.

## 4

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a sufficiently regular solution with zero [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), differentiate its squared [L2 norm](../../../real-analysis.md#l2-norm). Since $u_t=-i(\Delta u-Vu)$,

$$
\frac{d}{dt}\|u(t)\|_{L^2}^2
=2\operatorname{Re}\int_\Omega\overline u\,u_t
=2\operatorname{Re}\left[-i\left(\int_\Omega\overline u\,\Delta u
-\int_\Omega V|u|^2\right)\right].
$$

[Integration by parts](../../../calculus.md#integration-by-parts) and the zero boundary trace give $\int\overline u\Delta u=-\int|\nabla u|^2$. The potential contribution is real because $V$ is real. The quantity in parentheses is consequently real, and its product with $-i$ has zero real part. Hence

$$
\boxed{\|u(t)\|_{L^2(\Omega)}=\|u(0)\|_{L^2(\Omega)}.}
$$

This is the [energy method](../../../numerical-analysis.md#energy-method) for a [skew-adjoint](../../../functional-analysis.md#skew-adjoint-generator) evolution. For general [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) data, the same result follows from the [strongly continuous unitary group](../../../functional-analysis.md#strongly-continuous-unitary-group) generated by a self-adjoint realization of $\Delta-V$. A sufficient assumption is a bounded real potential with the Dirichlet Laplacian; arbitrary real potentials require appropriate domain and self-adjointness assumptions. The differentiated proof presumes the regularity needed for the displayed integrals, rather than asserting it for every pointwise real function $V$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Arrange the interior values into a vector $U$. Represent the [five-point Dirichlet Laplacian as a Kronecker sum](../../../finite-difference.md#five-point-dirichlet-laplacian-as-a-kronecker-sum) $L_h=h^{-2}(D\otimes I+I\otimes D)$, where $D$ is the [tridiagonal matrix](../../../vector-space.md#tridiagonal-matrix) with diagonal $-2$ and adjacent entries one. This [Kronecker sum](../../../vector-space.md#kronecker-sum) is real symmetric; the real sampled potential has a real diagonal matrix $D_V$. Thus

$$
iU'=H_hU,\qquad H_h=L_h-D_V=H_h^*.
$$

The generator $-iH_h$ is a [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix). Consequently

$$
\frac{d}{dt}(U^*U)
=2\operatorname{Re}(-iU^*H_hU)=0,
\qquad U(t)=e^{-itH_h}U(0).
$$

The [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is a [unitary matrix](../../../linear-operator-theory.md#unitary-matrix), either by differentiating its product with its adjoint or by [unitary diagonalization of a normal matrix](../../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix). For the two-dimensional [discrete L2 norm](../../../functional-analysis.md#discrete-l2-norm) $\|U\|_h^2=h^2\sum_{m,n}|U_{m,n}|^2$, this gives

$$
\boxed{\|U(t)-\widetilde U(t)\|_h
=\|U(0)-\widetilde U(0)\|_h\quad(t\geq0).}
$$

Applying the same equation to a difference proves [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) with a mesh-independent constant one. This is [norm conservation of a semidiscrete Schrödinger equation](../../../finite-difference.md#norm-conservation-of-a-semidiscrete-schrodinger-equation). It concerns continuous time after spatial discretization; an arbitrary subsequent time integrator need not preserve this stability.

**The printed coordinates do not discretize the stated square.** For $[-1,1]^2$ with $M$ interior points in each direction, use $h=2/(M+1)$, $x_m=-1+mh$, $y_n=-1+nh$, and sample $V$ there. The printed $h=1/(M+1)$ and unshifted coordinates instead describe a grid on $[0,1]^2$. The matrix proof is valid for either geometry with its corresponding boundary values, so this transcription-independent statement flaw does not alter the stability conclusion.

## 5

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Work in the real [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) $X=H_0^1(0,1)$, whose members have square-integrable [weak derivatives](../../../distribution-theory.md#weak-derivative) and zero endpoint trace. Define the [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form) and [linear functional](../../../linear-algebra.md#linear-functional)

$$
a(u,v)=\int_0^1(u'v'+uv)\,dx,\qquad
\ell(v)=\int_0^1xv\,dx.
$$

The [weak formulation](../../../partial-differential-equation.md#weak-formulation) is to find $u\in X$ with $a(u,v)=\ell(v)$ for every $v\in X$. [Integration by parts](../../../calculus.md#integration-by-parts) recovers the differential equation for a smooth solution; conversely, this identity is the definition of its [weak solution](../../../partial-differential-equation.md#weak-solution).

Use the full $H^1$ [norm](../../../functional-analysis.md#norm). The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $|a(u,v)|\leq\|u\|_{H^1}\|v\|_{H^1}$ and $|\ell(v)|\leq\|v\|_{H^1}/\sqrt3$. Also $a(v,v)=\|v\|_{H^1}^2$, so $a$ is a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form) with constant one. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) states that a bounded, coercive bilinear form on a real [Hilbert space](../../../hilbert-space.md) determines a unique weak solution for every bounded linear functional. It therefore applies here.

The equivalent minimization problem is

$$
\boxed{\min_{v\in H_0^1(0,1)}\mathcal E(v),\qquad
\mathcal E(v)=\frac12\int_0^1\bigl((v')^2+v^2\bigr)\,dx-\int_0^1xv\,dx.}
$$

If $u$ is the weak solution, symmetry and $a(u,v-u)=\ell(v-u)$ give

$$
\mathcal E(v)-\mathcal E(u)=\frac12a(v-u,v-u).
$$

This is positive unless $v=u$, proving a unique [global minimizer](../../../analysis.md#global-minimizer). Conversely, differentiating $\mathcal E(u+tv)$ at $t=0$ gives the weak identity. Thus **the unique energy minimizer is exactly the unique [weak solution](../../../partial-differential-equation.md#weak-solution)**. As a check, the classical representative is

$$
\boxed{u(x)=x-\frac{\sinh x}{\sinh1}.}
$$

It satisfies both endpoint conditions and $-u''+u=x$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

**The trial space must be a subspace of $H_0^1(0,1)$, not merely of $L^2(0,1)$.** The printed assumptions on the basis do not ensure square-integrable weak derivatives, and boundary traces are not defined for arbitrary [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) functions. For example, $\varphi(x)=x^{1/4}(1-x)$ is continuous, vanishes at both endpoints and belongs to $L^2$, but $|\varphi'(x)|^2\sim x^{-3/2}/16$ is not integrable at zero. Assume the basis belongs to the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space), as it does for the hat functions in part (c).

Write $u_H=\sum_{j=1}^M c_j\varphi_j$. Differentiating the restricted energy with respect to $c_i$, or imposing the [Galerkin method](../../../partial-differential-equation.md#galerkin-method) with test function $\varphi_i$, gives

$$
\boxed{\sum_{j=1}^M A_{ij}c_j=F_i,\qquad
A_{ij}=\int_0^1(\varphi_j'\varphi_i'+\varphi_j\varphi_i)\,dx,\qquad
F_i=\int_0^1x\varphi_i\,dx.}
$$

The derivative term is the usual diffusion [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) and the second is the [mass matrix](../../../numerical-analysis.md#mass-matrix). The full matrix is real symmetric, and for every nonzero coefficient vector $c$,

$$
c^TAc=\int_0^1\left[\left(\sum_jc_j\varphi_j'\right)^2
+\left(\sum_jc_j\varphi_j\right)^2\right]dx>0,
$$

because a basis is [linearly independent](../../../vector-space.md#linear-independence). Thus it is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), so the restricted [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) has a unique solution and minimum.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) have disjoint supports unless their nodes coincide or are neighbours. Direct integration on the two adjacent intervals gives

$$
\int\varphi_i'^2=\frac2h,\quad
\int\varphi_i^2=\frac{2h}3,\quad
\int\varphi_i'\varphi_{i+1}'=-\frac1h,\quad
\int\varphi_i\varphi_{i+1}=\frac h6.
$$

Since $x=x_i+(x-x_i)$ and the hat is symmetric about $x_i=ih$, its load is $F_i=x_i\int\varphi_i=x_i h=ih^2$. Thus the [reaction-diffusion finite element matrix](../../../numerical-analysis.md#reaction-diffusion-finite-element-matrix) gives the explicit equations

$$
\boxed{\left(\frac2h+\frac{2h}3\right)c_i
+\left(-\frac1h+\frac h6\right)(c_{i-1}+c_{i+1})=ih^2,
\quad 1\leq i\leq M,\quad c_0=c_{M+1}=0.}
$$

The coefficient matrix is a [tridiagonal matrix](../../../vector-space.md#tridiagonal-matrix) and a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) by the energy identity in part (b), hence **nonsingular**. A separate spectral verification uses the sine basis with $\theta_j=j\pi/(M+1)$ and gives

$$
\lambda_j=\frac{2(1-\cos\theta_j)}h
+\frac h3(2+\cos\theta_j)>0.
$$

Both terms are positive for the Dirichlet modes. This also identifies precisely how the diffusion [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) and reaction [mass matrix](../../../numerical-analysis.md#mass-matrix) combine.

## 6

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The starting point of a conforming [finite element method](../../../numerical-analysis.md#finite-element-method) is a [weak formulation](../../../partial-differential-equation.md#weak-formulation) in a [Hilbert space](../../../hilbert-space.md) $X$. For example, a homogeneous [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) on a bounded [Lipschitz domain](../../../real-analysis.md#lipschitz-domain) gives $X=H_0^1(\Omega)$. One seeks

$$
a(u,v)=\ell(v)\qquad(v\in X),
$$

where $a$ is a [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form), $|a(w,v)|\leq L\|w\|_X\|v\|_X$, and $\ell\in X^*$ is a bounded [linear functional](../../../linear-algebra.md#linear-functional). A [conforming finite element space](../../../numerical-analysis.md#conforming-finite-element-space) $X_h\subset X$ is finite dimensional and is typically built from functions that are polynomial on each element of a [finite element mesh](../../../numerical-analysis.md#finite-element-mesh). With a basis $\varphi_j$, the [Galerkin method](../../../partial-differential-equation.md#galerkin-method) imposes the same identity only for $v_h\in X_h$, giving

$$
\boxed{Kc=F,\qquad K_{ij}=a(\varphi_j,\varphi_i),\quad F_i=\ell(\varphi_i).}
$$

The [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) is sparse when basis supports overlap only locally. Local element integrals assemble its entries; the [mass matrix](../../../numerical-analysis.md#mass-matrix) represents an $L^2$ term. This separates the choice of trial functions from the variational principle determining their coefficients.

The fundamental well-posedness theorem is the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem): if $a(v,v)\geq\gamma\|v\|_X^2$ for some $\gamma>0$, there is a unique solution for each $\ell\in X^*$, with $\|u\|_X\leq\|\ell\|_{X^*}/\gamma$. The same theorem on $X_h$ gives a unique discrete solution. The constants must be independent of the mesh for uniform [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method). Boundary conditions are built into the trial space when they are essential constraints; flux conditions arise through boundary terms in [integration by parts](../../../calculus.md#integration-by-parts) and are natural constraints in the [weak formulation](../../../partial-differential-equation.md#weak-formulation).

When $a$ is symmetric and a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form), the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) minimizes

$$
\mathcal E(v)=\tfrac12a(v,v)-\ell(v)
$$

over $X_h$. Its first variation is exactly the [Galerkin method](../../../partial-differential-equation.md#galerkin-method), so **Ritz minimization and Galerkin testing coincide for symmetric coercive problems**. The [energy norm](../../../numerical-analysis.md#energy-norm) $\|v\|_a=\sqrt{a(v,v)}$ turns the approximation into an [orthogonal projection](../../../hilbert-space.md#orthogonal-projection). Indeed, subtracting the exact and discrete weak equations gives [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality), $a(u-u_h,v_h)=0$. For every $v_h\in X_h$ the [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) becomes

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2,
$$

so

$$
\boxed{\|u-u_h\|_a=\inf_{v_h\in X_h}\|u-v_h\|_a.}
$$

This exact best-approximation property is the central advantage of the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method).

Symmetry is unnecessary for the [Galerkin method](../../../partial-differential-equation.md#galerkin-method). For any bounded, coercive form, the [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) gives

$$
\boxed{\|u-u_h\|_X\leq\frac L\gamma
\inf_{v_h\in X_h}\|u-v_h\|_X.}
$$

To prove it, put $e=u-u_h$. [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality) yields $a(e,e)=a(e,u-v_h)$, so coercivity and boundedness give $\gamma\|e\|_X^2\leq L\|e\|_X\|u-v_h\|_X$. Divide when $e\neq0$ and take the [infimum](../../../real-analysis.md#infimum). Thus approximation capability plus uniform coercivity gives convergence. In contrast, minimizing $\tfrac12a(v,v)-\ell(v)$ for a nonsymmetric form differentiates its symmetric part and generally does not solve the original weak equation.

A concrete symmetric example is the one-dimensional reaction-diffusion problem from Question 5. Continuous [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) give the diffusion [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) $S$ with diagonal $2/h$ and neighbouring entries $-1/h$, and the [mass matrix](../../../numerical-analysis.md#mass-matrix) $M$ with diagonal $2h/3$ and neighbouring entries $h/6$. Therefore $K=S+M$ and $F_i=ih^2$. Its [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) is the coordinate form of the continuous energy. The exact smooth solution $u(x)=x-\sinh(x)/\sinh1$ makes this an explicit test of the method, not just an abstract existence result.

For a nonsymmetric example, take positive $\varepsilon$, constant real $\beta$, and

$$
-\varepsilon u''+\beta u'+u=f,\qquad u(0)=u(1)=0.
$$

Its form is $a(u,v)=\varepsilon\int u'v'+\beta\int u'v+\int uv$. Since $\int v'v=0$, it has coercivity constant $\min(\varepsilon,1)$ in the full $H^1$ norm, although it is not symmetric when $\beta\neq0$. The [Galerkin method](../../../partial-differential-equation.md#galerkin-method) remains well posed. On the uniform hat basis, $K=\varepsilon S+\beta C+M$, where $C_{i,i+1}=1/2$, $C_{i,i-1}=-1/2$ and $C_{ii}=0$. The [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) $C$ cancels from $c^TKc$, proving nonsingularity. A Ritz energy would omit precisely this advection contribution. Small $\varepsilon$ may nevertheless make the approximation constant large and produce poorly resolved layers; algebraic solvability is not an accuracy guarantee.

Quantitative convergence uses a [finite element interpolation estimate](../../../numerical-analysis.md#finite-element-interpolation-estimate). On a [shape-regular mesh](../../../numerical-analysis.md#shape-regular-mesh), for piecewise-linear conforming elements and $u\in H^2(\Omega)$ in the usual low-dimensional setting,

$$
\|u-I_hu\|_{H^1}\leq Ch\|u\|_{H^2},\qquad
\|u-I_hu\|_{L^2}\leq Ch^2\|u\|_{H^2}.
$$

The [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) therefore gives an $O(h)$ energy error. The [Aubin–Nitsche duality argument](../../../numerical-analysis.md#aubin-nitsche-duality-argument) improves the [L2 norm](../../../real-analysis.md#l2-norm) error when the dual elliptic problem has $H^2$ regularity: solve $a(v,z)=(e,v)_{L^2}$ and use

$$
\|e\|_{L^2}^2=a(e,z-I_hz)
\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Consequently

$$
\boxed{\|u-u_h\|_{H^1}=O(h),\qquad
\|u-u_h\|_{L^2}=O(h^2),}
$$

with constants depending on the solution and regularity bounds. The second estimate is conditional on dual regularity; corners or insufficient data regularity can reduce the rate.

The same [Galerkin method](../../../partial-differential-equation.md#galerkin-method) handles evolution equations. For the homogeneous [heat equation](../../../diffusion-equation.md#heat-equation), the [semidiscrete finite element heat equation](../../../numerical-analysis.md#semidiscrete-finite-element-heat-equation) is $M\dot c+Sc=0$. Because $M$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) and $S$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix),

$$
\frac{d}{dt}(c^TMc)=-2c^TSc\leq0.
$$

The decreasing [quadratic form](../../../linear-algebra.md#quadratic-form) is exactly the [L2 norm](../../../real-analysis.md#l2-norm) squared of the finite-element function. This separates spatial [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) from the subsequent time integrator, just as in the [Schrödinger equation](../../../physics.md#schrodinger-equation) example. **Conformity, coercivity and approximation estimates together explain convergence.**

## 7

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

An $s$-stage [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) for $y'=f(t,y)$ is defined by

$$
Y_i=y_n+h\sum_{j=1}^sa_{ij}f(t_n+c_jh,Y_j),\qquad
y_{n+1}=y_n+h\sum_{i=1}^sb_if(t_n+c_ih,Y_i).
$$

The [Butcher tableau](../../../numerical-analysis.md#butcher-tableau) records $A=(a_{ij})$, $b$ and $c$; internal consistency usually sets $c=Ae$, and first-order consistency requires $b^Te=1$. A strictly lower triangular $A$ gives an explicit method, while other stage dependencies generally require an [implicit Runge-Kutta method](../../../numerical-analysis.md#implicit-runge-kutta-method). The [stage solvability of an implicit Runge-Kutta method](../../../numerical-analysis.md#stage-solvability-of-an-implicit-runge-kutta-method) must be checked separately: if $f$ is globally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) in $y$ with constant $L$, the stage fixed-point map is a contraction in the maximum stage norm whenever $hL\max_i\sum_j|a_{ij}|<1$. This is a sufficient small-step condition, not a restriction intrinsic to the definitions of [A-stability](../../../numerical-analysis.md#a-stability) or [B-stability](../../../numerical-analysis.md#b-stability).

Linear stability begins with the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$. Solving the stages gives

$$
\boxed{y_{n+1}=R(z)y_n,\qquad
R(z)=1+zb^T(I-zA)^{-1}e,\qquad z=h\lambda.}
$$

The [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) consists of test values for which the stage system is well defined and $|R(z)|\leq1$. [A-stability](../../../numerical-analysis.md#a-stability) means this includes the closed left half-plane. For $\operatorname{Re}\lambda<0$, this gives stability with no scalar decay-mode step restriction. For a [normal matrix](../../../linear-operator-theory.md#normal-matrix) $L$ in $y'=Ly$, [unitary diagonalization of a normal matrix](../../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix) reduces the [norm](../../../functional-analysis.md#norm) estimate to these scalar factors. For a [non-normal matrix](../../../linear-operator-theory.md#non-normal-matrix), eigenvalues alone do not establish a uniform [norm](../../../functional-analysis.md#norm) bound: eigenvector conditioning and transient amplification matter. Mesh-uniform estimates for discretized PDEs must control operator powers, not only their spectra.

Every consistent explicit [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) has a nonconstant polynomial [stability function](../../../numerical-analysis.md#stability-function) and therefore cannot be [A-stable](../../../numerical-analysis.md#a-stability), since that polynomial is unbounded on the negative real axis. For example, [Forward Euler method](../../../numerical-analysis.md#euler-method) has $R(z)=1+z$, stability disk $|1+z|\leq1$, and restriction $0\leq hq\leq2$ for $\lambda=-q<0$. For a pure imaginary mode $\lambda=i\omega\neq0$, $|1+ih\omega|>1$, so it is unstable for every positive step. The [classical fourth-order Runge-Kutta method](../../../numerical-analysis.md#classical-fourth-order-runge-kutta-method) instead has

$$
R(z)=1+z+\tfrac12z^2+\tfrac16z^3+\tfrac1{24}z^4,
\qquad |R(iq)|^2=1-\frac{q^6}{72}+\frac{q^8}{576}.
$$

It is stable on the imaginary axis exactly for $|q|\leq2\sqrt2$, an illustrative conditional stability range for oscillatory evolution.

[Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $R(z)=(1-z)^{-1}$ and is [A-stable](../../../numerical-analysis.md#a-stability). [L-stability](../../../numerical-analysis.md#l-stability) adds $R(z)\to0$ as $|z|\to\infty$ in the left half-plane; backward Euler satisfies this and strongly damps unresolved rapidly decaying modes in a [stiff differential equation](../../../numerical-analysis.md#stiff-equation). The [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) and the [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule) both have $R(z)=(1+z/2)/(1-z/2)$, so they are [A-stable](../../../numerical-analysis.md#a-stability) but not [L-stable](../../../numerical-analysis.md#l-stability). They preserve the modulus of a pure imaginary test mode, but their stiff-decay limit is $-1$, leaving oscillatory numerical remnants. The three-stage [Lobatto IIIA method](../../../numerical-analysis.md#lobatto-iiia-method) has the fourth-order rational function found in Question 2 and likewise lacks [L-stability](../../../numerical-analysis.md#l-stability). Thus high order and [A-stability](../../../numerical-analysis.md#a-stability) do not themselves imply efficient stiff damping.

Nonlinear stability measures differences between solutions of the same equation. A [one-sided Lipschitz condition](../../../real-analysis.md#one-sided-lipschitz-condition) is

$$
\operatorname{Re}\langle f(t,y)-f(t,\widetilde y),y-\widetilde y\rangle
\leq\nu\|y-\widetilde y\|^2.
$$

Differentiating the squared difference and applying the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives $\|y(t)-\widetilde y(t)\|\leq e^{\nu(t-t_0)}\|y(t_0)-\widetilde y(t_0)\|$. A [dissipative vector field](../../../differential-equation.md#dissipative-vector-field) has $\nu\leq0$ and is contractive. A [B-stable](../../../numerical-analysis.md#b-stability) method preserves this property for every positive step size for which the stages are well defined:

$$
\boxed{\|y_{n+1}-\widetilde y_{n+1}\|\leq\|y_n-\widetilde y_n\|.}
$$

This includes time-dependent vector fields when dissipativity holds at each common time argument. Applying it to scalar linear dissipative fields shows that [B-stability](../../../numerical-analysis.md#b-stability) implies [A-stability](../../../numerical-analysis.md#a-stability) when the linear stages are well defined; the converse fails.

The standard sufficient theorem is **[algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) implies [B-stability](../../../numerical-analysis.md#b-stability)**, subject to stage solvability. Define $B=\operatorname{diag}(b)$ and $M=BA+A^TB-bb^T$. [Algebraic stability of a Runge-Kutta method](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) means $b_i\geq0$ and $M$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix). To prove the theorem, set $d=y_n-\widetilde y_n$, $D_i=Y_i-\widetilde Y_i$ and $F_i=f(t_n+c_ih,Y_i)-f(t_n+c_ih,\widetilde Y_i)$. Expanding the output difference and using $D_i=d+h\sum_ja_{ij}F_j$ yields the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity)

$$
\|d_{n+1}\|^2=\|d\|^2
+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

Dissipativity makes the first sum nonpositive, while positive semidefiniteness makes the last [quadratic form](../../../linear-algebra.md#quadratic-form) nonnegative. The latter follows by factoring $M=Q^TQ$ and writing it as a sum of squared [norms](../../../functional-analysis.md#norm) of linear combinations of the $F_i$. This proves the claimed contraction. It is a sufficient theorem; absence of [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) is not, by itself, a proof of failure of [B-stability](../../../numerical-analysis.md#b-stability) for every representation.

Several examples make the distinctions concrete. For backward Euler, $b=1$, $A=(1)$, so $M=(1)$: it is both [L-stable](../../../numerical-analysis.md#l-stability) and [B-stable](../../../numerical-analysis.md#b-stability). For implicit midpoint, $b=1$, $A=(1/2)$, so $M=(0)$: it is [B-stable](../../../numerical-analysis.md#b-stability) and preserves squared [norms](../../../functional-analysis.md#norm) for a skew-Hermitian linear equation, but lacks stiff damping. For the two-stage [Gauss--Legendre Runge-Kutta method](../../../numerical-analysis.md#gauss-legendre-method),

$$
A=\begin{pmatrix}1/4&1/4-\sqrt3/6\\1/4+\sqrt3/6&1/4\end{pmatrix},
\qquad b=(1/2,1/2)^T,
$$

the matrix $M$ vanishes as well. The collocation theorem gives order four, and its [stability function](../../../numerical-analysis.md#stability-function) is exactly the same as the three-stage Lobatto IIIA function. Yet the Gauss method is [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method), whereas that Lobatto method is not. Identical scalar linear stability functions need not imply identical nonlinear stability properties.

An example combining stiff damping and nonlinear contraction is the two-stage [Radau IIA method](../../../numerical-analysis.md#radau-iia-method), with

$$
A=\begin{pmatrix}5/12&-1/12\\3/4&1/4\end{pmatrix},\quad
b=(3/4,1/4)^T,\quad
M=\frac1{16}\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\quad
R(z)=\frac{1+z/3}{1-2z/3+z^2/6}.
$$

Its positive weights and positive semidefinite $M$ prove [B-stability](../../../numerical-analysis.md#b-stability); its rational function has denominator roots $2\pm i\sqrt2$ and, for $z=x+iy$, satisfies

$$
|1-2z/3+z^2/6|^2-|1+z/3|^2
=\frac{|z|^4-8x|z|^2+24x^2-72x}{36}\geq0\quad(x\leq0).
$$

Thus it is [A-stable](../../../numerical-analysis.md#a-stability); the limit $R(z)\to0$ then proves [L-stability](../../../numerical-analysis.md#l-stability). The standard Radau IIA collocation theorem gives order $2s-1$, here three. These properties explain its usefulness for stiff nonlinear equations.

Finally, **[A-stability](../../../numerical-analysis.md#a-stability) alone does not imply [B-stability](../../../numerical-analysis.md#b-stability)**. The [trapezoidal rule fails B-stability](../../../numerical-analysis.md#trapezoidal-rule-fails-b-stability) even for the scalar dissipative equation $y'=-y^3$. With $h=1$, its step map $T$ is uniquely defined by

$$
T(y)+\tfrac12T(y)^3=y-\tfrac12y^3.
$$

At $y=\sqrt2$, $T(y)=0$. Implicit differentiation gives

$$
T'(y)=\frac{1-\tfrac32y^2}{1+\tfrac32T(y)^2},\qquad T'(\sqrt2)=-2.
$$

Thus nearby starting values are separated by approximately twice their original distance after one step, although the exact flow is contractive. This example and the contractivity theorem show why scalar linear analysis, stiff damping and genuinely nonlinear [norm](../../../functional-analysis.md#norm) estimates answer different stability questions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
