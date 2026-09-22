# Paper 341

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_341.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_341.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
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
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Lagrange interpolation polynomials](../../../numerical-analysis.md#lagrange-polynomial) at $c_1=1/3$ and $c_2=1$ are

$$
\ell_1(s)=\frac32(1-s),\qquad \ell_2(s)=\frac32s-\frac12.
$$

Their [integrals](../../../calculus.md#integral) give

$$
\left(\int_0^{c_i}\ell_j(s)\,ds\right)_{ij}
=\begin{pmatrix}5/12&-1/12\\3/4&1/4\end{pmatrix},
\qquad
\left(\int_0^1\ell_j(s)\,ds\right)_j=(3/4,1/4).
$$

Thus the coefficients are exactly those of a [collocation Runge-Kutta method](../../../numerical-analysis.md#collocation-runge-kutta-method). More explicitly, with stage slopes $F_j=f(t_n+c_jh,Y_j)$, the degree-two [polynomial](../../../polynomial.md)

$$
p(t_n+sh)=y_n+h\sum_{j=1}^2F_j\int_0^s\ell_j(r)\,dr
$$

satisfies $p(t_n)=y_n$, $p(t_n+c_ih)=Y_i$, and $p'(t_n+c_ih)=F_i$. These are the [collocation Runge-Kutta method](../../../numerical-analysis.md#collocation-runge-kutta-method) equations, and $y_{n+1}=p(t_n+h)$. For an [implicit Runge-Kutta method](../../../numerical-analysis.md#implicit-runge-kutta-method), the nearby stages exist uniquely for sufficiently small $h$ under [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity); see [stage solvability of an implicit Runge-Kutta method](../../../numerical-analysis.md#stage-solvability-of-an-implicit-runge-kutta-method).

Write $e=(1,1)^T$, $c=Ae$, and interpret powers of $c$ componentwise. The [Butcher order conditions](../../../numerical-analysis.md#butcher-order-condition) through degree three are verified directly:

$$
b^Te=1,\qquad b^Tc=\frac12,\qquad b^Tc^2=\frac13,\qquad b^TAc=\frac16.
$$

For the last equality, $Ac=(1/18,1/2)^T$. However, the necessary degree-four [Butcher order condition](../../../numerical-analysis.md#butcher-order-condition) fails:

$$
b^Tc^3=\frac{5}{18}\ne\frac14.
$$

Consequently, for sufficiently smooth [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation), the [local truncation error](../../../numerical-analysis.md#local-truncation-error) is $O(h^4)$ and the [order of a Runge-Kutta method](../../../numerical-analysis.md#order-of-a-runge-kutta-method) is exactly

$$
\boxed{p=3}.
$$

This is the two-stage [Radau IIA method](../../../numerical-analysis.md#radau-iia-method); the conclusion follows from the explicit calculations rather than its name.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), put $z=h\lambda$. Eliminating the stages of the [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) gives the [stability function](../../../numerical-analysis.md#stability-function)

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\boxed{\frac{1+z/3}{1-2z/3+z^2/6}}.
$$

Its poles are $2\pm i\sqrt2$, strictly in the right half-plane. To prove [A-stability](../../../numerical-analysis.md#a-stability) directly, write $z=-r+iy$ with $r\geq0$. With $D(z)=1-2z/3+z^2/6$ and $N(z)=1+z/3$, elementary expansion gives

$$
|D(z)|^2-|N(z)|^2
=2r+\frac23r^2+\frac29r^3+\frac1{36}r^4
+\frac29ry^2+\frac1{18}r^2y^2+\frac1{36}y^4\geq0.
$$

Therefore $|R(z)|\leq1$ throughout the closed left half-plane; the inequality is strict except at $z=0$. **The method is [A-stable](../../../numerical-analysis.md#a-stability).** Moreover $R(z)\to0$ as $|z|\to\infty$, so the [Radau IIA method](../../../numerical-analysis.md#radau-iia-method) is also [L-stable](../../../numerical-analysis.md#l-stability).

## 2

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Insert an exact smooth [solution of a differential equation](../../../differential-equation.md#solution-of-a-differential-equation) and expand about $t=t_{n+2}$. The unscaled [local truncation error](../../../numerical-analysis.md#local-truncation-error), with every term moved to the left, is

$$
d_h(t)=\frac{1-7\alpha}{6}h^3y^{(3)}(t)
+\frac{15\alpha-1}{24}h^4y^{(4)}(t)+O(h^5).
$$

Here the constant, first-[derivative](../../../calculus.md#derivative), and second-[derivative](../../../calculus.md#derivative) terms all cancel, using the [chain rule](../../../calculus.md#chain-rule) identity $y''=f'(y)f(y)$. Hence the formal defect convention $d_h=O(h^{p+1})$ gives

$$
\boxed{p=3\quad(\alpha=1/7),\qquad p=2\quad(\alpha\ne1/7)}.
$$

At $\alpha=1/7$, the coefficient of $h^4y^{(4)}$ is $1/21$, so there is no further cancellation. At any other $\alpha$, the cubic coefficient is nonzero.

There is a degeneracy at $\alpha=1$: both the first-[derivative](../../../calculus.md#derivative) coefficient and $\rho'(1)$ vanish. The raw defect still has the displayed formal order two, but it cannot be normalized by $(1-\alpha)h$ into an ordinary first-order [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) test. Thus a convention requiring this nondegenerate normalization would leave the ODE order undefined at $\alpha=1$. In either convention, it is not a convergent approximation to arbitrary initial-value data; the next part explains why.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The first [characteristic polynomials of a linear multistep method](../../../numerical-analysis.md#characteristic-polynomials-of-a-linear-multistep-method) is

$$
\rho(\zeta)=\zeta^2-(1+\alpha)\zeta+\alpha=(\zeta-1)(\zeta-\alpha).
$$

The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) requires $|\alpha|\leq1$ and excludes $\alpha=1$, where the [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) at one is double. At $\alpha=-1$, the two unit-modulus [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) are distinct, so [zero-stability](../../../numerical-analysis.md#zero-stability) holds. For $\alpha\ne1$, the first-order [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) identity is $\rho'(1)=1-\alpha$, equal to the coefficient of $hf$.

Using the permitted [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) in this [multiderivative multistep method](../../../numerical-analysis.md#multiderivative-multistep-method) setting gives

$$
\boxed{-1\leq\alpha<1}.
$$

This means convergence on every fixed finite time interval where the smooth exact [solution of a differential equation](../../../differential-equation.md#solution-of-a-differential-equation) exists, with consistent starting values and the nearby branch of each implicit solve. More specifically, the [convergence of a zero-stable multiderivative method](../../../numerical-analysis.md#convergence-of-a-zero-stable-multiderivative-method) gives order $p$ when the starting errors are $O(h^p)$ and both $f$ and $f'f$ are locally uniformly [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) on the relevant region.

The exclusions are genuine. For $y'=0$ and $|\alpha|>1$, an arbitrarily small parasitic starting error is amplified as $\alpha^n$. At $\alpha=1$, take $y_0=0$, $y_1=h$, also for $y'=0$. The exact solution is zero, but the numerical recurrence gives $y_n=nh$, an error of order one at fixed positive time. This proves failure even though the starting values converge.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

On the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), $g(y)=\lambda^2y$, so the [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) becomes

$$
\left[1-(1-\alpha)z+\frac{1-3\alpha}{2}z^2\right]\xi^2
-(1+\alpha)\xi+\alpha=0,\qquad z=h\lambda.
$$

Both [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), including the parasitic one, must satisfy the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method).

For $\alpha=1/7$, multiply by seven and set $a=7-6z+2z^2$. The [polynomial](../../../polynomial.md) is $a\xi^2-8\xi+1$. The [complex quadratic Schur criterion](../../../numerical-analysis.md#complex-quadratic-schur-criterion) says that its [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) are strictly in the [unit disk](../../../geometry-and-topology.md#unit-disk) if

$$
|a|>1,\qquad |a|^2-1>8|a-1|.
$$

Here is a direct verification on the entire left half-plane. Put $z=-r+iy$, $r\geq0$, $t=y^2$, and $a_0=7+6r+2r^2$. Then

$$
q=|a|^2=a_0^2+8(r^2+3r+1)t+4t^2\geq49,
$$

and expansion of the squared inequality gives

$$
\begin{aligned}
(q-1)^2-64|a-1|^2={}&16t^4+64(r^2+3r+1)t^3\\
&+32(r^2+3r+3)(3r^2+9r+2)t^2\\
&+64r(r+3)(r^4+6r^3+17r^2+24r+11)t\\
&+16r(r+3)(r^2+3r+3)^2(r^2+3r+8).
\end{aligned}
$$

Every term is nonnegative, and at least one is positive unless $z=0$. Since $q-1>0$, taking square roots proves the strict [complex quadratic Schur criterion](../../../numerical-analysis.md#complex-quadratic-schur-criterion) for $z\ne0$. At $z=0$, the [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) are the simple values $1$ and $1/7$. The leading coefficient cannot vanish because $|a|^2\geq49$. Thus **the method at $\alpha=1/7$ is [A-stable](../../../numerical-analysis.md#a-stability)**. Its order three is compatible with the [Second Dahlquist barrier](../../../numerical-analysis.md#second-dahlquist-barrier): that barrier concerns first-[derivative](../../../calculus.md#derivative) [linear multistep methods](../../../numerical-analysis.md#linear-multistep-method), whereas this method uses a second [derivative](../../../calculus.md#derivative).

For $\alpha=1/2$, choose $z=-4$, strictly in the left half-plane. The [amplification polynomial of a multistep method](../../../numerical-analysis.md#amplification-polynomial-of-a-multistep-method) reduces to

$$
-\xi^2-\frac32\xi+\frac12=0,\qquad
\xi=\frac{-3\pm\sqrt{17}}4.
$$

One [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) has [modulus](../../../complex-analysis.md#modulus) $(3+\sqrt{17})/4>1$. Thus **the method at $\alpha=1/2$ is not [A-stable](../../../numerical-analysis.md#a-stability)**.

## 3

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [Dirichlet Laplacian eigenfunctions](../../../partial-differential-equation.md#dirichlet-laplacian-eigenfunction) and positive [Dirichlet Laplacian eigenvalues](../../../partial-differential-equation.md#dirichlet-laplacian-eigenvalue) on the interval of length two are

$$
\phi_j(x)=\sin\frac{j\pi(x+1)}2,\qquad
\lambda_j=\left(\frac{j\pi}{2}\right)^2,\qquad j\geq1.
$$

A [Sturm-Liouville eigenfunction expansion](../../../analysis.md#sturm-liouville-eigenfunction-expansion) gives $u=\sum_jq_j(t)\phi_j$, with $q_j''+(\lambda_j-\alpha)q_j=0$. Thus all [normal modes](../../../wave-equation.md#normal-mode) oscillate precisely when $\alpha<\lambda_1$.

To justify a spatially uniform bound for arbitrary appropriate data, assume the usual [wave equation](../../../wave-equation.md) energy class $u(0)\in H_0^1(-1,1)$ and $u_t(0)\in L^2(-1,1)$, or smoother compatible data. The [energy method](../../../numerical-analysis.md#energy-method) conserves

$$
E=\frac12\left(\|u_t\|_{L^2}^2+\|u_x\|_{L^2}^2-\alpha\|u\|_{L^2}^2\right).
$$

The sharp [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) is $\|u\|_{L^2}^2\leq\lambda_1^{-1}\|u_x\|_{L^2}^2$. For $0\leq\alpha<\lambda_1$, this makes $E$ coercive with constant $1-\alpha/\lambda_1$; for $\alpha<0$, [coercivity](../../../real-analysis.md#coercive-function) is immediate. The [one-dimensional Sobolev representative](../../../sobolev-space.md#one-dimensional-sobolev-representative) satisfies $|u(x,t)|\leq\sqrt2\,\|u_x(t)\|_{L^2}$ by the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Hence the conserved [energy](../../../classical-mechanics.md#energy) bounds $u$ uniformly in both variables.

At $\alpha=\lambda_1$, the smooth solution $u=t\phi_1$ is unbounded. At $\alpha>\lambda_1$, $u=e^{\sqrt{\alpha-\lambda_1}t}\phi_1$ is unbounded. Therefore

$$
\boxed{\alpha<\frac{\pi^2}{4}}.
$$

The bound depends on the initial data; it is not a single bound for all arbitrarily rescaled solutions. The energy-class hypothesis supplies pointwise meaning and excludes undefined rough-data interpretations.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

**The printed formula is not a consistent spatial discretization of the stated PDE.** The original PDF genuinely has $1/\Delta x$, rather than $1/(\Delta x)^2$. Writing $h=\Delta x$, the [Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
h^{-1}\bigl(u(x-h)-2u(x)+u(x+h)\bigr)=h\,u_{xx}(x)+O(h^3),
$$

so it approximates a diffusion coefficient tending to zero. Moreover, $m=1,\ldots,M$ and $h=1/(M+1)$ cover $(0,1)$, whereas the given [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) belong to $(-1,1)$. No value at the interior location $x=0$ was prescribed. These are actual source defects, not repairs justified by the TeX conversion.

A conditional analysis of the literal [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) system is still possible. If it is closed by imposing $u_0=u_{M+1}=0$ on the displayed grid, the negative [Dirichlet discrete Laplacian](../../../finite-difference.md#dirichlet-discrete-laplacian) has positive frequencies squared

$$
\kappa_j(h)=\frac4h\sin^2\frac{j\pi}{2(M+1)},\qquad j=1,\ldots,M,
$$

and each [normal mode](../../../wave-equation.md#normal-mode) obeys $q_j''=(\alpha-\kappa_j)q_j$. For a fixed mesh, every solution is bounded for all time exactly when

$$
\boxed{\alpha<\kappa_1(h)=\frac4h\sin^2\frac{\pi h}{2}}.
$$

Equality produces a linearly growing [normal mode](../../../wave-equation.md#normal-mode) for nonzero modal initial velocity; above the threshold there is an exponentially growing [normal mode](../../../wave-equation.md#normal-mode). Since $\kappa_1(h)\sim\pi^2h\to0$, any $0<\alpha<\pi^2/4$ gives bounded continuous solutions but unbounded literal discrete solutions on sufficiently fine meshes. For example, $\alpha=1$, $M=99$ gives $\kappa_1<1$, and a growing first sine [normal mode](../../../wave-equation.md#normal-mode). At $\alpha=0$, every fixed mesh is bounded for all time, but unit first-mode initial velocity has maximal displacement $1/\sqrt{\kappa_1(h)}$, which diverges on mesh refinement. For uniform-in-mesh, all-time displacement bounds for arbitrary bounded displacement/velocity data in the mesh-weighted [L2 norm](../../../real-analysis.md#l2-norm), the literal closed system therefore requires $\alpha<0$.

This differs from finite-time [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method), governed here by [displacement stability of a symmetric semidiscrete wave equation](../../../finite-difference.md#displacement-stability-of-a-symmetric-semidiscrete-wave-equation). For the conditional closure above, [diagonalization of a matrix](../../../linear-operator-theory.md#diagonalization-of-a-matrix) gives, with $\alpha_+=\max(\alpha,0)$,

$$
\|U(t)\|_h\leq e^{\sqrt{\alpha_+}t}
\bigl(\|U(0)\|_h+t\|U'(0)\|_h\bigr),\qquad
\|U\|_h^2=h\sum_m|U_m|^2.
$$

Oscillatory modes use $|\sin(\omega t)/\omega|\leq t$, including its value $t$ at $\omega=0$; growing modes use $\sinh(\beta t)/\beta\leq t e^{\beta t}$. Thus the displacement map is mesh-uniformly bounded on each fixed finite time interval for every fixed real $\alpha$. This is a legitimate finite-time displacement [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) estimate, but neither [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) nor the all-time conclusion of part (i). It does not assert a velocity bound in the unweighted displacement norm.

If the intended method instead uses $h^{-2}$ and the full interval, take interior indices $m=-M,\ldots,M$, $h=1/(M+1)$, with zeros at $m=\pm(M+1)$. Its first positive discrete [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is

$$
\lambda_{1,h}=\frac4{h^2}\sin^2\frac{\pi h}{4}<\frac{\pi^2}{4},
\qquad \lambda_{1,h}\longrightarrow\frac{\pi^2}{4}.
$$

The corrected, fixed-mesh all-time condition is $\alpha<\lambda_{1,h}$, with the same strictness at equality. For every fixed $\alpha<\pi^2/4$, this holds on all sufficiently fine meshes. This corrected interpretation is stated separately rather than silently replacing the PDF.

## 4

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

**The original PDF has a spatial shift $u_{m+2}^{n+2}$, so the printed scheme is not the usual second-order BDF discretization.** The PDF does have $-2u_m^{n+2}$ on the right; the TeX aid loses that factor two, and that transcription must not be used.

Let $h=\Delta x$, $k=\Delta t$, and expand an exact smooth [heat equation](../../../diffusion-equation.md#heat-equation) solution about $(x_m,t_{n+2})$. Relative to the standard unshifted [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula), the printed newest value adds

$$
u(x_m+2h,t)-u(x_m,t)=2hu_x+2h^2u_{xx}+O(h^3).
$$

Dividing the raw residual by $2k/3$, its expansion is

$$
u_t-u_{xx}+\frac{3h}{k}u_x+\frac{3h^2}{k}u_{xx}
-\frac{k^2}{3}u_{ttt}-\frac{h^2}{12}u_{xxxx}
+O(k^3+h^4+h^3/k).
$$

In particular, for the usual refinement $k=\mu h^2$ with fixed $\mu>0$, the term $3u_x/(\mu h)$ generally diverges. A concrete smooth counterexample is $u=e^{-\pi^2t/4}\cos(\pi x/2)$, which satisfies the [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) and has $u_x\ne0$ at $x=1/2$. Thus **the printed scheme has no consistent order under fixed-$\mu$ refinement**. Its normalized shift error is $O(h/k)$, so one could only investigate a special coupled limit such as $h=o(k)$ after specifying a valid boundary closure; it has no standard joint second-order accuracy.

For the likely intended correction $u_m^{n+2}$, the extra shift terms disappear. The normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) is

$$
-\frac{k^2}{3}u_{ttt}-\frac{h^2}{12}u_{xxxx}+O(k^3+h^4).
$$

With a stable, suitably accurate starter, the corrected [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula) combined with the [second-order central difference](../../../finite-difference.md#second-order-central-difference) therefore has

$$
\boxed{\text{order two in time and order two in space}}.
$$

This is a correction to the printed method, not a claim about it.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The spatial shift in the PDF also requires a boundary value beyond the supplied right endpoint: if $m$ is the last interior index, the newest $m+2$ value is outside the interval. Thus **the printed Dirichlet method has no specified boundary closure, and no unique stability range can be assigned to it as stated**.

For completeness, the literal interior formula has an exact [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis) on an infinite or periodic grid. Substitution of a [Fourier mode](../../../fourier-analysis.md#fourier-mode) $U_m^n=\xi^ne^{im\theta}$ gives

$$
A(\theta)\xi^2-4\xi+1=0,\qquad
A(\theta)=3e^{2i\theta}+8\mu\sin^2(\theta/2).
$$

For the [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) tending to one as $\theta\to0$, expansion gives

$$
\xi=1-3i\theta-(\mu+3/2)\theta^2+O(\theta^3),
\qquad
|\xi|^2=1+(6-2\mu)\theta^2+O(\theta^4).
$$

Consequently $\mu<3$ is unstable: sufficiently small nonzero frequencies have a [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) of [modulus](../../../complex-analysis.md#modulus) greater than one, and arbitrarily fine periodic grids contain such frequencies.

Conversely, if $\mu\geq3$ and $s=\cos\theta$, then

$$
\operatorname{Re}A-3
=6(s-1)^2+4(\mu-3)(1-s)\geq0.
$$

For $A=u+iv$ with $u\geq3$,

$$
(|A|^2-1)^2-16|A-1|^2
=(u-1)^2(u-3)(u+5)+2(u^2-9)v^2+v^4\geq0.
$$

Since $|A|\geq3$, the [complex quadratic Schur criterion](../../../numerical-analysis.md#complex-quadratic-schur-criterion) yields both [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) in the [unit disk](../../../geometry-and-topology.md#unit-disk), strictly inside except at $\theta=0$, where they are $1$ and $1/3$. Uniform [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) follows directly from the [BDF2 discrete energy identity](../../../numerical-analysis.md#bdf2-discrete-energy-identity): the modal recurrence is $3v^{n+2}-4v^{n+1}+v^n=-(A-3)v^{n+2}$, whose [energy](../../../classical-mechanics.md#energy) decreases because $\operatorname{Re}(A-3)\geq0$. Summing the modal energies proves a bound independent of the grid and even of $\mu\geq3$; no eigenvector-separation assumption is needed. This is the [stability of a spatially shifted BDF2 stencil](../../../finite-difference.md#stability-of-a-spatially-shifted-bdf2-stencil). Thus the literal periodic-grid result is

$$
\boxed{\mu\geq3\quad\text{for the printed shifted stencil on a periodic grid}}.
$$

This cannot establish stability of an unspecified [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) closure. It also does not restore [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method).

For the intended unshifted [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula), a spatial [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-\beta\leq0$ gives

$$
(3+2k\beta)\xi^2-4\xi+1=0.
$$

The [Schur stability criterion](../../../numerical-analysis.md#schur-stability-criterion) gives the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) for every $k\beta\geq0$, with strict inequalities for $\beta>0$. A useful uniform [energy method](../../../numerical-analysis.md#energy-method) proof, including the repeated interior roots that a bare separation argument would miss, is the [BDF2 discrete energy identity](../../../numerical-analysis.md#bdf2-discrete-energy-identity). With $\delta^2U=U^{n+2}-2U^{n+1}+U^n$ and

$$
\mathcal E_n=\|U^{n+1}\|_h^2+\|2U^{n+1}-U^n\|_h^2,
$$

the corrected [Dirichlet discrete Laplacian](../../../finite-difference.md#dirichlet-discrete-laplacian) scheme satisfies

$$
\mathcal E_{n+1}-\mathcal E_n+\|\delta^2U\|_h^2
+4k\|D_+U^{n+2}\|_h^2=0.
$$

This follows by taking the [inner product](../../../linear-algebra.md#inner-product) of $3U^{n+2}-4U^{n+1}+U^n=2kL_hU^{n+2}$ with $U^{n+2}$ and using [summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula). It controls both time levels uniformly, regardless of the mesh ratio. Hence the corrected method is stable for

$$
\boxed{\text{every }\mu>0}.
$$

## 5

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Use the real [Hilbert space](../../../hilbert-space.md) $V=H_0^1(0,1)$, the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space), with [norm](../../../functional-analysis.md#norm) $\|v\|_V=\|v'\|_{L^2}$. The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) makes this equivalent to its usual [Sobolev space](../../../sobolev-space.md) norm. Define the symmetric [bilinear form](../../../linear-algebra.md#bilinear-form) and continuous [linear functional](../../../linear-algebra.md#linear-functional)

$$
a(u,v)=\int_0^1\bigl(u'v'+xuv\bigr)\,dx,\qquad
\ell(v)=\int_0^1fv\,dx.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the sharp interval [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) imply

$$
|a(u,v)|\leq(1+\pi^{-2})\|u\|_V\|v\|_V,\qquad
a(v,v)\geq\|v\|_V^2,\qquad
|\ell(v)|\leq\pi^{-1}\|f\|_{L^2}\|v\|_V.
$$

Thus $a$ is a [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form) and a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form), and $\ell$ is bounded because $f$ is [square-integrable](../../../measure-theory.md#square-integrable-function). The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) supplies a unique [weak solution](../../../partial-differential-equation.md#weak-solution):

$$
\boxed{y\in H_0^1(0,1),\qquad a(y,v)=\ell(v)\quad\text{for every }v\in H_0^1(0,1)}.
$$

This is obtained from the differential equation by [integration by parts](../../../calculus.md#integration-by-parts); the test functions have zero boundary trace. Conversely, the [weak solution](../../../partial-differential-equation.md#weak-solution) satisfies $y''=xy-f$ in the sense of [distributions](../../../distribution-theory.md#distribution-mathematical-analysis). Since $xy-f\in L^2$, it belongs to $H^2(0,1)\cap H_0^1(0,1)$ and solves the equation [almost everywhere](../../../measure-theory.md#almost-everywhere).

Equivalently, the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) minimizes

$$
J(v)=\frac12\int_0^1\bigl((v')^2+xv^2\bigr)\,dx-\int_0^1fv\,dx
$$

over $V$. Indeed $J(y+w)-J(y)=a(w,w)/2$, since the mixed term is $a(y,w)-\ell(w)=0$. This proves existence and uniqueness of the minimizer directly from the [weak solution](../../../partial-differential-equation.md#weak-solution), as well as its equivalence to the [variational problem](../../../calculus-of-variations.md#variational-problem).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Choose a [basis](../../../vector-space.md#basis) $\phi_1,\ldots,\phi_N$ of a [conforming finite element space](../../../numerical-analysis.md#conforming-finite-element-space) $V_N\subset H_0^1(0,1)$ and write $y_N=\sum_jc_j\phi_j$. Testing the [variational problem](../../../calculus-of-variations.md#variational-problem) with each [basis](../../../vector-space.md#basis) function gives

$$
\boxed{\sum_{j=1}^N A_{ij}c_j=b_i,\qquad
A_{ij}=\int_0^1(\phi_j'\phi_i'+x\phi_j\phi_i)\,dx,\qquad
b_i=\int_0^1f\phi_i\,dx}.
$$

These are also the equations $\partial J(y_N)/\partial c_i=0$ for the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method). The [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) is symmetric and a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix): for a nonzero coefficient [vector](../../../vector-space.md#vector) $c$, [linear independence](../../../vector-space.md#linear-independence) gives $v_N=\sum c_j\phi_j\ne0$, and

$$
c^TAc=a(v_N,v_N)\geq\|v_N'\|_{L^2}^2>0.
$$

Thus there is a unique coefficient [vector](../../../vector-space.md#vector).

Subtracting the exact and discrete [variational problems](../../../calculus-of-variations.md#variational-problem) proves [Galerkin orthogonality](../../../numerical-analysis.md#galerkin-orthogonality), $a(y-y_N,v_N)=0$ for every $v_N\in V_N$. In the [energy norm](../../../numerical-analysis.md#energy-norm) $\|v\|_a=\sqrt{a(v,v)}$, the [Pythagorean identity](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) yields

$$
\|y-v_N\|_a^2=\|y-y_N\|_a^2+\|y_N-v_N\|_a^2.
$$

Therefore the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) is the best approximation in the [energy norm](../../../numerical-analysis.md#energy-norm). The [Céa lemma](../../../numerical-analysis.md#cea-s-lemma) also gives $\|y-y_N\|_V\leq(1+\pi^{-2})\inf_{v_N\in V_N}\|y-v_N\|_V$, so any dense sequence of conforming trial spaces converges.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Put $h=1/(N+1)$ and $x_i=ih$. The interior [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) are

$$
\phi_i(x)=
\begin{cases}
(x-x_{i-1})/h,&x_{i-1}\leq x\leq x_i,\\
(x_{i+1}-x)/h,&x_i\leq x\leq x_{i+1},\\
0,&\text{otherwise}.
\end{cases}
$$

They are a [basis](../../../vector-space.md#basis) of the continuous piecewise-affine functions vanishing at both endpoints. The [support of a function](../../../function.md#support) for each hat only overlaps those of neighbouring hats, so the [stiffness matrix](../../../numerical-analysis.md#stiffness-matrix) is a [tridiagonal matrix](../../../vector-space.md#tridiagonal-matrix). Direct [integration](../../../calculus.md#integral) gives the [derivative](../../../calculus.md#derivative) contribution $2/h$ on the diagonal and $-1/h$ on adjacent diagonals.

For the potential contribution, symmetry about $x_i$ gives $\int x\phi_i^2\,dx=x_i\int\phi_i^2\,dx=2hx_i/3$. On the overlap of $\phi_i$ and $\phi_{i+1}$, their product is symmetric about $(x_i+x_{i+1})/2$, and its [integral](../../../calculus.md#integral) is $h/6$. This is the [affine-weighted hat mass matrix](../../../numerical-analysis.md#affine-weighted-hat-mass-matrix) calculation. Consequently,

$$
\boxed{
A_{ii}=\frac2h+\frac{2hx_i}{3},\qquad
A_{i,i+1}=A_{i+1,i}=-\frac1h+\frac{h(x_i+x_{i+1})}{12}
}
$$

and all other entries vanish. The exact right-hand side is

$$
b_i=\frac1h\int_{x_{i-1}}^{x_i}(x-x_{i-1})f(x)\,dx
+\frac1h\int_{x_i}^{x_{i+1}}(x_{i+1}-x)f(x)\,dx.
$$

Thus, with $c_0=c_{N+1}=0$, the requested scalar equations are

$$
\begin{aligned}
\left(-\frac1h+\frac{h(x_{i-1}+x_i)}{12}\right)c_{i-1}
+\left(\frac2h+\frac{2hx_i}{3}\right)c_i
+\left(-\frac1h+\frac{h(x_i+x_{i+1})}{12}\right)c_{i+1}
=b_i,\quad 1\leq i\leq N.
\end{aligned}
$$

At the endpoints the coefficient multiplying the zero boundary value is simply omitted. Since $f\in L^2$, its point values are not even well defined; replacing $b_i$ by $hf(x_i)$ would require an additional [quadrature rule](../../../numerical-analysis.md#quadrature-rule) convention and regularity hypothesis, not present here. The exact [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) uses the displayed [integrals](../../../calculus.md#integral). The [finite element interpolation estimate](../../../numerical-analysis.md#finite-element-interpolation-estimate) and [Céa lemma](../../../numerical-analysis.md#cea-s-lemma), using $y\in H^2$, give an $O(h)$ [energy norm](../../../numerical-analysis.md#energy-norm) error; the [Aubin–Nitsche duality argument](../../../numerical-analysis.md#aubin-nitsche-duality-argument) gives $O(h^2)$ in the [L2 norm](../../../real-analysis.md#l2-norm) on this interval.

## 6

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) advances $y'=f(t,y)$ through stages

$$
Y_i=y_n+h\sum_j a_{ij}F_j,\qquad
F_j=f(t_n+c_jh,Y_j),\qquad
y_{n+1}=y_n+h\sum_i b_iF_i.
$$

The [Butcher tableau](../../../numerical-analysis.md#butcher-tableau) records $A,b,c$, normally with $c=Ae$. Linear [absolute stability](../../../numerical-analysis.md#linear-stability-domain) tests the amplification of a linear decay mode; nonlinear [B-stability](../../../numerical-analysis.md#b-stability) compares distances between two solutions of a [dissipative vector field](../../../differential-equation.md#dissipative-vector-field). Both describe propagation of perturbations, but they impose different conditions.

For the [Dahlquist test equation](../../../numerical-analysis.md#dahlquist-test-equation), elimination of stages gives

$$
R(z)=1+zb^T(I-zA)^{-1}e,\qquad z=h\lambda.
$$

The [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) consists of $z$ for which the step is defined and $|R(z)|\leq1$. Poles or singular stage systems must be excluded, even if an output formula has a formal cancellation. For a scalar test equation, the proof is $y_n=R(z)^ny_0$: the powers are bounded exactly when $|R(z)|\leq1$. For $y'=Ly$, the update is $R(hL)$. If $L$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix), [unitary diagonalization of a normal matrix](../../../linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix) makes the [operator norm](../../../continuous-dual-space.md#operator-norm) equal to the largest scalar amplification [modulus](../../../complex-analysis.md#modulus). For a diagonalizable [matrix](../../../vector-space.md#matrix), powers are bounded by the [condition number](../../../linear-algebra.md#condition-number) of the [eigenvector](../../../linear-operator-theory.md#eigenvector) matrix times the maximal scalar power. These constants must remain uniform for mesh-dependent systems. A defective unit-modulus [eigenvalue](../../../linear-operator-theory.md#eigenvalue) can instead produce a growing [Jordan block](../../../linear-operator-theory.md#jordan-block); the scalar spectral test alone does not control a general [matrix](../../../vector-space.md#matrix).

An [A-stable](../../../numerical-analysis.md#a-stability) method accepts the entire closed left half-plane. The [Explicit Euler method](../../../numerical-analysis.md#euler-method) has $R(z)=1+z$ and a disk of stability $|1+z|\leq1$, so it is not [A-stable](../../../numerical-analysis.md#a-stability). No nonconstant [polynomial](../../../polynomial.md) [stability function](../../../numerical-analysis.md#stability-function) can be [A-stable](../../../numerical-analysis.md#a-stability), since it is unbounded on the negative real axis; this excludes all consistent explicit [Runge-Kutta methods](../../../numerical-analysis.md#runge-kutta-method). The [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $R(z)=1/(1-z)$, and $|1-z|\geq1$ when $\operatorname{Re}z\leq0$, proving [A-stability](../../../numerical-analysis.md#a-stability). It is also [L-stable](../../../numerical-analysis.md#l-stability), because $R(z)\to0$ for large left-half-plane $z$.

The [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) and the [trapezoidal rule](../../../numerical-analysis.md#trapezoidal-rule) have the same scalar [stability function](../../../numerical-analysis.md#stability-function),

$$
R(z)=\frac{1+z/2}{1-z/2}.
$$

The identity $|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z$ proves [A-stability](../../../numerical-analysis.md#a-stability). On the imaginary axis their amplification has unit [modulus](../../../complex-analysis.md#modulus), and along the negative real axis it tends to $-1$. Thus neither is [L-stable](../../../numerical-analysis.md#l-stability); very stiff decay can persist as alternating numerical values. In contrast, the two-stage [Radau IIA method](../../../numerical-analysis.md#radau-iia-method) has $R(z)=(1+z/3)/(1-2z/3+z^2/6)$, with the explicit nonnegative modulus-gap proof in question 1, and is [L-stable](../../../numerical-analysis.md#l-stability). This illustrates why [L-stability](../../../numerical-analysis.md#l-stability) matters beyond [A-stability](../../../numerical-analysis.md#a-stability) for a [stiff differential equation](../../../numerical-analysis.md#stiff-equation).

For nonlinear problems, assume a real or complex Euclidean [inner product](../../../linear-algebra.md#inner-product) and the dissipativity hypothesis

$$
\operatorname{Re}\langle f(t,u)-f(t,v),u-v\rangle\leq0
$$

for all relevant states at each common time. Exact solutions satisfy

$$
\frac{d}{dt}\|u-v\|^2
=2\operatorname{Re}\langle f(t,u)-f(t,v),u-v\rangle\leq0.
$$

A [B-stable](../../../numerical-analysis.md#b-stability) [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) reproduces this nonexpansion of distances whenever its stages exist. Put $d=y_n-\widetilde y_n$, $D_i=Y_i-\widetilde Y_i$, and $G_i=f(t_n+c_ih,Y_i)-f(t_n+c_ih,\widetilde Y_i)$. Then $D_i=d+h\sum_j a_{ij}G_j$. Expansion of the output squared [norm](../../../functional-analysis.md#norm), followed by substituting $d=D_i-h\sum_j a_{ij}G_j$ in its linear terms, proves the [Runge-Kutta contractivity identity](../../../numerical-analysis.md#runge-kutta-contractivity-identity)

$$
\|d_{\mathrm{new}}\|^2-\|d\|^2
=2h\sum_i b_i\operatorname{Re}\langle D_i,G_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle G_i,G_j\rangle,
\quad
m_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j.
$$

If $b_i\geq0$ and $M=(m_{ij})$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix), the first sum is nonpositive by dissipativity, and the second is nonnegative: expand each coordinate of the stage [vectors](../../../vector-space.md#vector) to express it as a sum of nonnegative [quadratic forms](../../../linear-algebra.md#quadratic-form). These are exactly the conditions for [algebraic stability of a Runge-Kutta method](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method). Hence **[algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) implies [B-stability](../../../numerical-analysis.md#b-stability)**. Applying [B-stability](../../../numerical-analysis.md#b-stability) to the linear dissipative problem $y'=\lambda y$, or its two-dimensional real form, also proves [A-stability](../../../numerical-analysis.md#a-stability) whenever stages are well defined.

The [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) has $b=A=1$, hence $M=1$; the [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule) has $b=1$, $A=1/2$, hence $M=0$. Both are [algebraically stable](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) and [B-stable](../../../numerical-analysis.md#b-stability). For the two-stage [Radau IIA method](../../../numerical-analysis.md#radau-iia-method),

$$
M=\frac1{16}\begin{pmatrix}1&-1\\-1&1\end{pmatrix},
$$

a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix), while both weights are positive. It therefore combines third-order accuracy, [B-stability](../../../numerical-analysis.md#b-stability), and [L-stability](../../../numerical-analysis.md#l-stability). The distinction between stability and solvability is essential: for [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) $f$, the stage map is a contraction when $hL\max_i\sum_j|a_{ij}|<1$, so the [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) proves small-step unique solvability. The preceding [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) proof is an estimate for existing stages; it is not a theorem asserting stage existence for arbitrary step sizes and domains.

Linear [A-stability](../../../numerical-analysis.md#a-stability) is insufficient for nonlinear [B-stability](../../../numerical-analysis.md#b-stability). The [trapezoidal rule fails B-stability](../../../numerical-analysis.md#trapezoidal-rule-fails-b-stability), even though its scalar [stability function](../../../numerical-analysis.md#stability-function) is identical to that of the [B-stable](../../../numerical-analysis.md#b-stability) [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule). Its [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) coefficients are

$$
A=\begin{pmatrix}0&0\\1/2&1/2\end{pmatrix},\qquad
b=(1/2,1/2)^T,\qquad
M=\begin{pmatrix}-1/4&0\\0&1/4\end{pmatrix}.
$$

Failure of this sufficient [algebraic stability](../../../numerical-analysis.md#algebraic-stability-of-a-runge-kutta-method) test alone would not prove failure of [B-stability](../../../numerical-analysis.md#b-stability). An actual counterexample does: take $f(y)=-y^3$ and $h=2$. Dissipativity follows from

$$
(f(u)-f(v))(u-v)=-(u-v)^2(u^2+uv+v^2)\leq0.
$$

The unique step map $T$ obeys $T+T^3=y-y^3$, because the left-hand side is strictly increasing and onto. At $y=1$, $T=0$, and implicit [differentiation](../../../calculus.md#differentiation) gives

$$
T'(1)=\frac{1-3(1)^2}{1+3T(1)^2}=-2.
$$

Nearby initial states expand in distance. This proves a true nonlinear failure rather than merely failure of a coefficient criterion.

Finally, [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) on finite intervals connects these contractivity properties to accuracy. If a one-step map is nonexpansive and its exact one-step defect has [norm](../../../functional-analysis.md#norm) at most $Ch^{p+1}$, then the error satisfies $\|e_{n+1}\|\leq\|e_n\|+Ch^{p+1}$, hence $\|e_n\|\leq\|e_0\|+CT h^p$ for $nh\leq T$. A Lipschitz step bound $1+Kh$ gives the same order using the [discrete Gronwall inequality](../../../probability-and-statistics.md#discrete-gronwall-inequality). For a [stiff differential equation](../../../numerical-analysis.md#stiff-equation), the value of [B-stability](../../../numerical-analysis.md#b-stability) is that the propagation estimate need not grow with a large negative dissipative rate. The accuracy constant still needs appropriate smoothness and uniform [derivative](../../../calculus.md#derivative) bounds; stability alone does not establish a mesh-uniform error order.

## 7

↑ **Parent:** [Paper 341](paper-341.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

For a fully discrete linear [partial differential equation](../../../partial-differential-equation.md) evolution, write $U^{n+1}=C_{h,k}U^n$ in a specified discrete [norm](../../../functional-analysis.md#norm). Finite-time [stability of a numerical method](../../../numerical-analysis.md#stability-of-a-numerical-method) means

$$
\boxed{\|C_{h,k}^{\,n}\|\leq C_T\quad\text{whenever }nk\leq T},
$$

with $C_T$ independent of the allowed meshes. For a [multistep method](../../../numerical-analysis.md#linear-multistep-method), augment the state with its time-history values and include a stable starter. Bounds may grow as $e^{\omega T}$ when the continuous problem has growth; demanding decay for all time would be a stronger assertion. The treatment of initial data, forcing, [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), and the [norm](../../../functional-analysis.md#norm) is part of the hypothesis, not a detail supplied by an interior calculation.

For constant coefficients on an infinite or periodic uniform grid, [von Neumann stability analysis](../../../finite-difference.md#von-neumann-stability-analysis) substitutes the [Fourier mode](../../../fourier-analysis.md#fourier-mode) $U_j^n=G(\theta)^ne^{ij\theta}$. The [discrete Fourier transform](../../../numerical-analysis.md#discrete-fourier-transform) and the [Parseval identity](../../../fourier-analysis.md#parseval-identity) turn a uniform multiplier estimate into a discrete [L2 norm](../../../real-analysis.md#l2-norm) estimate. In a one-step scalar scheme, $|G(\theta)|\leq1$ proves contractivity, while $|G(\theta)|\leq1+\omega k$ gives finite-time [stability](../../../numerical-analysis.md#stability-of-a-numerical-method). In a multilevel scheme, every [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) in its [amplification polynomial of a multilevel finite difference scheme](../../../finite-difference.md#amplification-polynomial-of-a-multilevel-finite-difference-scheme) matters, as does uniform control of the associated companion [matrix](../../../vector-space.md#matrix).

For the [Forward Euler diffusion scheme](../../../finite-difference.md#forward-euler-diffusion-scheme) with $\mu=k/h^2$,

$$
G(\theta)=1-4\mu\sin^2(\theta/2).
$$

Thus $|G|\leq1$ for all frequencies exactly when

$$
\boxed{0\leq\mu\leq\frac12}.
$$

Sufficiency follows since $G\in[-1,1]$; necessity follows from the highest-frequency mode $\theta=\pi$ on even periodic grids. This gives the usual parabolic mesh restriction $k\leq h^2/2$. For the [Backward Euler diffusion scheme](../../../finite-difference.md#backward-euler-diffusion-scheme),

$$
G(\theta)=\frac1{1+4\mu\sin^2(\theta/2)},
$$

so every $\mu\geq0$ is stable. The [Crank-Nicolson method](../../../numerical-analysis.md#crank-nicolson-method) has

$$
G(\theta)=\frac{1-2\mu\sin^2(\theta/2)}{1+2\mu\sin^2(\theta/2)},
$$

again of [modulus](../../../complex-analysis.md#modulus) at most one for all $\mu\geq0$, but stiff modes approach $-1$ rather than zero. These are PDE manifestations of the [A-stability](../../../numerical-analysis.md#a-stability) and [L-stability](../../../numerical-analysis.md#l-stability) distinctions for time integration.

For advection $u_t+a u_x=0$, assume $a>0$ and set $\nu=ak/h$. The [upwind finite difference scheme](../../../finite-difference.md#upwind-finite-difference-scheme) is $U_j^{n+1}=(1-\nu)U_j^n+\nu U_{j-1}^n$, with

$$
|G(\theta)|^2=1-2\nu(1-\nu)(1-\cos\theta).
$$

It is contractive when $0\leq\nu\leq1$. This also has a direct maximum-norm proof: each newest value is a [convex combination](../../../mathematical-optimization.md#convex-combination) of two old values. The resulting [Courant–Friedrichs–Lewy condition](../../../finite-difference.md#courant-friedrichs-lewy-condition) expresses that the numerical [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence) covers the physical one. For negative $a$, the upwind direction must be reversed. By contrast, [Forward Euler method](../../../numerical-analysis.md#euler-method) time stepping with the centered first [finite difference](../../../finite-difference.md) has $G=1-i\nu\sin\theta$ and $|G|>1$ for nonzero $\nu\sin\theta$. Under fixed nonzero $\nu$ refinement it is unstable, since a fixed nontrivial mode grows geometrically over $T/k$ steps. This is not a claim of instability under every imaginable mesh coupling: $k=O(h^2)$ instead bounds its spurious finite-time growth, since $\log|G|\leq a^2k^2/(2h^2)$.

The [leapfrog advection scheme](../../../finite-difference.md#leapfrog-advection-scheme) illustrates a multilevel subtlety. Its [amplification polynomial of a multilevel finite difference scheme](../../../finite-difference.md#amplification-polynomial-of-a-multilevel-finite-difference-scheme) is

$$
\xi^2+2i\nu\sin\theta\,\xi-1=0.
$$

For $|\nu|<1$, both [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) have unit [modulus](../../../complex-analysis.md#modulus) and separation at least $2\sqrt{1-\nu^2}$. A uniformly conditioned eigenbasis of the companion [matrix](../../../vector-space.md#matrix) then proves [power boundedness of a two-level Fourier scheme](../../../finite-difference.md#power-boundedness-of-a-two-level-fourier-scheme) for arbitrary history data. At $|\nu|=1$ and a grid admitting $\theta=\pi/2$, the roots coincide on the [unit circle](../../../complex-analysis.md#complex-unit-circle), and a [Jordan block](../../../linear-operator-theory.md#jordan-block) produces $n\xi^n$ growth. Thus the endpoint fails the ordinary arbitrary-history [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method); checking only that both moduli equal one misses the instability. Restricting the starter or filtering the parasitic mode is an additional hypothesis.

The [energy method](../../../numerical-analysis.md#energy-method) handles variable coefficients and finite boundaries for which [Fourier stability analysis](../../../finite-difference.md#fourier-stability-analysis) may be unavailable. For the [Backward Euler diffusion scheme](../../../finite-difference.md#backward-euler-diffusion-scheme) with homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), define $\|U\|_h^2=h\sum_j|U_j|^2$. The discrete [summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula) identity is

$$
\langle U,L_hU\rangle_h=-\|D_+U\|_h^2.
$$

Take the [inner product](../../../linear-algebra.md#inner-product) of $U^{n+1}-U^n=kL_hU^{n+1}$ with $2U^{n+1}$. The elementary identity $2\operatorname{Re}\langle x-y,x\rangle=\|x\|^2-\|y\|^2+\|x-y\|^2$ gives

$$
\|U^{n+1}\|_h^2-\|U^n\|_h^2
+\|U^{n+1}-U^n\|_h^2+2k\|D_+U^{n+1}\|_h^2=0.
$$

This proves unconditional contractivity including the actual boundary treatment. More generally, a [dissipative operator](../../../functional-analysis.md#dissipative-operator) $L_h$ gives $(I-kL_h)^{-1}$ of [operator norm](../../../continuous-dual-space.md#operator-norm) at most one: with $V=(I-kL_h)U$, dissipativity implies $\operatorname{Re}\langle V,U\rangle\geq\|U\|^2$, and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|U\|\leq\|V\|$. In finite dimensions this also proves invertibility. For the second-order [backward differentiation formula](../../../numerical-analysis.md#backward-differentiation-formula), the [BDF2 discrete energy identity](../../../numerical-analysis.md#bdf2-discrete-energy-identity) used in question 4 controls both time levels and proves unconditional diffusion stability. A repeated root strictly inside the disk is harmless here; the energy argument supplies the uniform bound without a singular [eigenvector](../../../linear-operator-theory.md#eigenvector) formula.

A second technique is [eigenvalue stability analysis of a finite difference method](../../../finite-difference.md#eigenvalue-stability-analysis-of-a-finite-difference-method). Under the [method of lines](../../../finite-difference.md#method-of-lines), a time integrator advances $U'=L_hU$ by $R(kL_h)$. If $L_h$ is a [normal matrix](../../../linear-operator-theory.md#normal-matrix), the scalar [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) criterion on all $k\lambda_j(L_h)$ controls its powers exactly in the corresponding [L2 norm](../../../real-analysis.md#l2-norm). For the centered [Dirichlet discrete Laplacian](../../../finite-difference.md#dirichlet-discrete-laplacian), its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) lie between $-4/h^2$ and zero; intersecting this interval with a time integrator's stability interval determines its mesh restriction. A uniform bound on the [diagonalization of a matrix](../../../linear-operator-theory.md#diagonalization-of-a-matrix) is needed for nonnormal diagonalizable systems. Eigenvalues alone can be misleading. For example,

$$
C_{h,k}=\begin{pmatrix}1-k&k/h\\0&1-k\end{pmatrix}
$$

has both [eigenvalues](../../../linear-operator-theory.md#eigenvalue) inside the disk for $0<k<1$, but the upper-right entry of $C_{h,k}^n$ is $nk(1-k)^{n-1}/h$. Taking $k=h$, $nk\to T>0$, this grows like $Te^{-T}/h$. Hence stable scalar [eigenvalues](../../../linear-operator-theory.md#eigenvalue) do not give mesh-uniform [stability](../../../numerical-analysis.md#stability-of-a-numerical-method). Boundary closures can introduce precisely the extra growth that an interior [Fourier symbol](../../../finite-difference.md#fourier-symbol-of-a-difference-operator) overlooks, so [boundary stability of a finite-difference method](../../../finite-difference.md#boundary-stability-of-a-finite-difference-method) must be checked separately.

For nonlinear spatial discretizations, a useful replacement for [Fourier stability analysis](../../../finite-difference.md#fourier-stability-analysis) is a convexity argument. If the [Forward Euler method](../../../numerical-analysis.md#euler-method) map $E_k(U)=U+kF(U)$ is nonexpansive in a chosen [norm](../../../functional-analysis.md#norm) for $k\leq k_{\mathrm{FE}}$, the second-order [strong stability preserving Runge-Kutta method](../../../numerical-analysis.md#strong-stability-preserving-runge-kutta-method)

$$
Y=E_k(U),\qquad
U_{\mathrm{new}}=\frac12U+\frac12E_k(Y)
$$

is also nonexpansive under the same restriction. Indeed, for two inputs, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $\|U_{\mathrm{new}}-\widetilde U_{\mathrm{new}}\|\leq\frac12\|U-\widetilde U\|+\frac12\|E_k(Y)-E_k(\widetilde Y)\|\leq\|U-\widetilde U\|$. Its [Taylor expansion](../../../calculus.md#taylor-expansion) is $U+kF(U)+k^2F'(U)F(U)/2+O(k^3)$, proving order two. Such [strong stability preserving Runge-Kutta methods](../../../numerical-analysis.md#strong-stability-preserving-runge-kutta-method) transfer suitable forward-step bounds without relying on a linear spectral calculation.

Finally, [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) explains what stability buys. For a linear [Hadamard well-posed problem](../../../inverse-problem.md#well-posed-problem), the [Lax equivalence theorem](../../../finite-difference.md#lax-equivalence-theorem) equates convergence of a consistent discretization with its [stability](../../../numerical-analysis.md#stability-of-a-numerical-method), under the stated approximation-space and norm hypotheses. Directly, if the error satisfies $e^{n+1}=C_{h,k}e^n+k\tau^n$, iteration gives the discrete [Duhamel principle](../../../diffusion-equation.md#duhamel-s-principle)

$$
e^n=C_{h,k}^ne^0+k\sum_{j=0}^{n-1}C_{h,k}^{n-1-j}\tau^j,
\qquad
\|e^n\|\leq C_T\bigl(\|e^0\|+T\max_j\|\tau^j\|\bigr).
$$

Thus vanishing normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) and initial error yield convergence. With a nonlinear Lipschitz step estimate, the [discrete Gronwall inequality](../../../probability-and-statistics.md#discrete-gronwall-inequality) plays the same role. A stable but inconsistent stencil, such as the literal defective formulas in questions 3 and 4 under their usual refinement, is not rescued by any amplification bound. **The decisive checks are a mesh-uniform evolution bound, a valid boundary closure, and consistency with the actual PDE.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
