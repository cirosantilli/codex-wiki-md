# Paper 341

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_341.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_341.pdf)

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

## 1

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Along an exact autonomous-ODE solution, $f(y)=y'$ and

$$
g(y)=f'(y)f(y)=y''.
$$

Move every term to the left and substitute the [Taylor expansions](../../../calculus.md#taylor-expansion) about $t_n$. The coefficients of $h^jy^{(j)}(t_n)$ vanish for $0\leq j\leq4$, while the first nonzero coefficient is

$$
\frac{2}{165}h^5y^{(5)}(t_n).
$$

Thus the local defect is $O(h^5)$. At $h=0$ the first characteristic polynomial is

$$
\rho(\xi)=\xi^2-\frac{16}{11}\xi+\frac5{11}
=(\xi-1)\left(\xi-\frac5{11}\right),
$$

which satisfies the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method). The method is therefore zero-stable and has

$$
\boxed{\text{order }4}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Apply the method to the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation) $y'=\lambda y$ and set $z=h\lambda$. Its amplification roots satisfy

$$
\left(1-\frac8{11}z+\frac2{11}z^2\right)\xi^2
-\frac{16}{11}\xi+\frac5{11}+\frac2{11}z=0.
$$

At $z=0$ the roots are $1$ and $5/11$. A root can leave the unit disk only through $\xi=e^{i\varphi}$. Substitution gives the boundary equation

$$
2\xi^2z^2+(2-8\xi^2)z+11\xi^2-16\xi+5=0.
$$

Direct separation into real and imaginary parts shows that both branches satisfy $\operatorname{Re}z\geq0$; equality occurs on the branch through $z=0$. Hence no root crosses the unit circle in $\operatorname{Re}z<0$. Moreover both roots tend to zero as $z\to\infty$ in the left half-plane. Consequently the method is [A-stable](../../../numerical-analysis.md#a-stability), and it also strongly damps the infinitely stiff limit.

## 2

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $A=(a_{ij})$, $b=(b_i)$, $\mathbf1=(1,1,1)^T$, and $c=A\mathbf1$. From the displayed tableau,

$$
c=\left(0,\frac35-\frac{\sqrt6}{10},
\frac35+\frac{\sqrt6}{10}\right)^T.
$$

The quadrature moments satisfy

$$
b^Tc^q=\frac1{q+1},\qquad q=0,1,2,3,4.
$$

Direct substitution into the remaining [Butcher order conditions](../../../numerical-analysis.md#butcher-order-condition) gives, for example,

$$
b^TAc=\frac16,\quad
b^T(c\circ Ac)=\frac18,\quad
b^TA(c\circ c)=\frac1{12},\quad
b^TA^2c=\frac1{24},
$$

and all rooted-tree conditions of orders at most five are satisfied. The order-six moment already fails:

$$
b^Tc^5=\frac{33}{200}\ne\frac16.
$$

The [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) therefore has

$$
\boxed{\text{order }5}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[Algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) requires $b_i\geq0$ and positive semidefiniteness of

$$
\mathcal M=BA+A^TB-bb^T,\qquad B=\operatorname{diag}(b).
$$

The three weights are positive, but direct calculation gives

$$
\mathcal M_{11}=2b_1a_{11}-b_1^2=-\frac1{81}<0.
$$

A positive-semidefinite matrix cannot have a negative diagonal entry. Hence

$$
\boxed{\text{the method is not algebraically stable}.}
$$

## 3

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The equation can be written

$$
u_t=iu_{xx}-iVu.
$$

For the squared [L2 norm](../../../real-analysis.md#l2-norm), periodic [integration by parts](../../../calculus.md#integration-by-parts) and the reality of $V$ give

$$
\frac d{dt}\int_{-1}^1|u|^2\,dx
=2\operatorname{Re}\int_{-1}^1
\left(iu_{xx}-iVu\right)\overline u\,dx
=2\operatorname{Re}\left[
-i\int_{-1}^1|u_x|^2\,dx
-i\int_{-1}^1V|u|^2\,dx
\right]=0.
$$

**Thus the [Schrödinger equation](../../../physics.md#schrodinger-equation) generates a unitary flow and $\|u(\cdot,t)\|_2$ is constant.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Here $\Delta x=1/M$ and periodic indexing is taken modulo $2M$. The [second-order central difference](../../../finite-difference.md#second-order-central-difference) matrix is the real symmetric circulant matrix

$$
A=M^2
\begin{pmatrix}
-2&1&0&\cdots&0&1\\
1&-2&1&\ddots&&0\\
0&1&-2&\ddots&\ddots&\vdots\\
\vdots&\ddots&\ddots&\ddots&1&0\\
0&&\ddots&1&-2&1\\
1&0&\cdots&0&1&-2
\end{pmatrix}.
$$

Since $V$ is real diagonal, $H=A-V$ is [Hermitian](../../../hilbert-space.md#hermitian-operator). Therefore $iH$ is [skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix), and

$$
\boxed{\frac d{dt}\|\mathbf u\|_2^2
=\mathbf u^*(iH)\mathbf u+
\mathbf u^*(-iH)\mathbf u=0.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Split the generator as $iA-iV$. One [Strang splitting](../../../numerical-analysis.md#strang-splitting) step is

$$
\boxed{
\mathbf u^{n+1}
=e^{-ihV/2}e^{ihA}e^{-ihV/2}\mathbf u^n
}.
$$

The two potential half-steps are componentwise multiplications. The circulant matrix $A$ is diagonalized by the [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform); its eigenvalues are

$$
\lambda_j=-4M^2\sin^2\left(\frac{\pi j}{2M}\right),
\qquad j=0,\ldots,2M-1.
$$

Thus the middle step consists of a [Fast Fourier transform](../../../numerical-analysis.md#cooley-tukey-fft-algorithm), multiplication of Fourier coefficient $j$ by $e^{ih\lambda_j}$, and an inverse transform. Its cost is $O(M\log M)$ and every factor is unitary, so the implementation preserves the discrete norm exactly up to roundoff.

## 4

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $L_h=D_{xx}+\alpha D_x$, where the centered second-difference matrix $D_{xx}$ is real symmetric negative definite under homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), and the centered first-difference matrix $D_x$ is real skew-symmetric. Hence

$$
\operatorname{Re}\langle\mathbf u,L_h\mathbf u\rangle
=\langle\mathbf u,D_{xx}\mathbf u\rangle\leq0.
$$

The semidiscrete [energy method](../../../numerical-analysis.md#energy-method) gives $\|\mathbf u(t)\|_2\leq\|\mathbf u(0)\|_2$ for every real $\alpha$, so the scheme is stable.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For the Cauchy problem, insert the [Fourier mode](../../../fourier-analysis.md#fourier-mode) $u_m=e^{im\vartheta}$. The spatial symbol is

$$
\lambda_h(\vartheta)
=-\frac4{\Delta x^2}\sin^2\frac\vartheta2
+i\frac{\alpha}{\Delta x}\sin\vartheta.
$$

Its real part is nonpositive for every $\vartheta$, so each mode has modulus $e^{t\operatorname{Re}\lambda_h}\leq1$. By the discrete [Fourier transform](../../../analysis.md#fourier-transform) and [Parseval identity](../../../fourier-analysis.md#parseval-identity), the scheme is stable in the discrete $L^2$ norm.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

[Forward Euler method](../../../numerical-analysis.md#euler-method) gives

$$
u_m^{n+1}=u_m^n
+r(u_{m-1}^n-2u_m^n+u_{m+1}^n)
+s(u_{m+1}^n-u_{m-1}^n),
$$

where

$$
r=\frac{\Delta t}{\Delta x^2},
\qquad
s=\frac{\alpha\Delta t}{2\Delta x}.
$$

Its [amplification factor](../../../finite-difference.md#amplification-factor) is

$$
G(\vartheta)=1-4r\sin^2\frac\vartheta2
+i\frac{\alpha\Delta t}{\Delta x}\sin\vartheta.
$$

Writing $X=\sin^2(\vartheta/2)$, the condition $|G|^2\leq1$ for every $0\leq X\leq1$ is equivalent to

$$
r\leq\frac12,
\qquad
\left(\frac{\alpha\Delta t}{\Delta x}\right)^2\leq2r.
$$

Therefore

$$
\boxed{
0\leq\Delta t\leq
\min\left\{\frac{\Delta x^2}{2},\frac2{\alpha^2}\right\}
}
$$

with the second bound omitted when $\alpha=0$.

## 5

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write the operator in [Sturm-Liouville form](../../../analysis.md#sturm-liouville-form):

$$
Lu=-\bigl((1+x^2)u'\bigr)'+x^2u.
$$

The natural solution space is the [Sobolev space](../../../sobolev-space.md) $H_0^1(0,1)$. Multiplication by a test function $v\in H_0^1(0,1)$ and integration by parts gives the symmetric bilinear form

$$
a(u,v)=\int_0^1
\left[(1+x^2)u'v'+x^2uv\right]dx.
$$

It is bounded and

$$
a(u,u)\geq\int_0^1|u'|^2dx
\geq C\|u\|_{H^1}^2
$$

by the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality). Thus $L$ is positive definite and $a$ is coercive. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) gives a unique weak solution of the variational problem

$$
\boxed{
\text{find }u\in H_0^1(0,1)
\text{ such that }
a(u,v)=\int_0^1fv\,dx
\quad\text{for every }v\in H_0^1(0,1).
}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $\{\phi_j\}_{j=1}^{N-1}$ be the [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) on a mesh, and put

$$
u_h=\sum_{j=1}^{N-1}U_j\phi_j.
$$

The [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) requires

$$
\sum_{j=1}^{N-1}K_{ij}U_j=F_i,
\qquad i=1,\ldots,N-1,
$$

where, for $f\equiv1$,

$$
\boxed{
K_{ij}=\int_0^1
\left[(1+x^2)\phi_j'\phi_i'
+x^2\phi_j\phi_i\right]dx,
\qquad
F_i=\int_0^1\phi_i\,dx.
}
$$

Local support makes $K$ symmetric tridiagonal, and coercivity makes it positive definite.

## 6

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Stability asks whether perturbations already present in data, arithmetic, or an earlier numerical step remain controlled under subsequent evolution. It complements [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method): consistency says that an exact smooth solution nearly satisfies one numerical step, while stability prevents the accumulated local defects from being amplified without bound. For a well-posed differential equation these two properties are what make convergence possible.

For a [linear multistep method](../../../numerical-analysis.md#linear-multistep-method), zero-stability concerns the limit $h\to0$. The roots of its first characteristic polynomial must lie in the closed unit disk, and every root on the unit circle must be simple. The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) states that a consistent linear multistep method converges precisely when it is zero-stable. The parasitic root $5/11$ in Question 1 decays, whereas a repeated root at $1$ would turn small defects into secular growth.

Absolute stability instead fixes $z=h\lambda$ for the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation). A one-step method has amplification factor $R(z)$ and absolute-stability region

$$
\mathcal S=\{z:|R(z)|\leq1\}.
$$

A-stability means that $\mathcal S$ contains the entire closed left half-plane, matching every decaying scalar linear problem. [L-stability](../../../numerical-analysis.md#l-stability) additionally requires $R(z)\to0$ as $z\to-\infty$, which suppresses unresolved fast transients in a [stiff differential equation](../../../numerical-analysis.md#stiff-equation). Backward Euler is L-stable; the trapezoidal rule is A-stable but approaches $-1$ and can retain stiff oscillations; forward Euler is stable only in the disk $|1+z|\leq1$.

For nonlinear dissipative systems, scalar absolute stability can be insufficient. B-stability controls distances between numerical solutions of contractive differential equations. For Runge–Kutta methods, algebraic stability—nonnegative weights and positive semidefiniteness of $BA+A^TB-bb^T$—is a useful sufficient condition for B-stability. Question 2 shows how a single negative diagonal entry disproves it.

After spatial discretization of a partial differential equation, stability can be studied through the semidiscrete matrix. If its Hermitian part is nonpositive, the [energy method](../../../numerical-analysis.md#energy-method) proves contractivity without diagonalizing it. A skew-Hermitian generator instead conserves norm, as in the discrete Schrodinger problem of Question 3. Eigenvalues alone can be misleading for a [non-normal matrix](../../../linear-operator-theory.md#non-normal-matrix): transient growth may be large even when every eigenvalue lies in the left half-plane, so matrix norms, logarithmic norms, resolvent bounds, or a [pseudospectrum](../../../banach-algebra.md#pseudospectrum) may be needed.

For constant-coefficient Cauchy problems, [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis) inserts Fourier modes and bounds their amplification factors. Question 4 gives a typical result: centered diffusion contributes a negative real symbol and centered advection an imaginary symbol. Semidiscrete evolution is stable, yet forward Euler imposes both the parabolic restriction $\Delta t=O(\Delta x^2)$ and an advection-diffusion restriction. This illustrates a [Courant–Friedrichs–Lewy condition](../../../finite-difference.md#courant-friedrichs-lewy-condition): a stable spatial approximation need not remain stable under an arbitrary time stepper.

For a well-posed linear initial-value problem and a consistent finite-difference approximation, the [Lax equivalence theorem](../../../finite-difference.md#lax-equivalence-theorem) identifies stability with convergence. Its hypotheses matter: it does not by itself cover nonlinear equations, inconsistent boundary closures, changing norms, or non-smooth solutions. Boundaries also defeat a naive whole-line Fourier argument; an energy estimate, normal-mode boundary analysis, or a discrete semigroup bound must include the boundary treatment.

Practical stability analysis therefore starts from the structure of the differential equation. Conservation laws favor unitary or symplectic methods, diffusion favors A- or L-stable implicit methods, monotone transport may require strong-stability-preserving time stepping and upwind fluxes, and stiff splitting requires attention to both the factors and their commutators. Stability does not guarantee accuracy: a heavily damped method may be stable while erasing the solution, and a stable computation with $h\lambda$ near the edge of its stability region may have an unacceptable phase error.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
