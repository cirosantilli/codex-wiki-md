# Paper 68

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper68.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper68.pdf)

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

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write the [Runge-Kutta method](../../../numerical-analysis.md#runge-kutta-method) coefficients as $A\in\mathbb R^{\nu\times\nu}$, $b\in\mathbb R^\nu$, and let $e$ be the all-ones column. On the test equation $y'=\lambda y$, with $z=h\lambda$, the stage [vector](../../../vector-space.md#vector) satisfies $Y=ey_n+zAY$ and the next value is $y_{n+1}=y_n+zb^TY$. Hence its [stability function](../../../numerical-analysis.md#stability-function) is

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\frac{\det(I-zA+zeb^T)}{\det(I-zA)}.
$$

Both [polynomials](../../../polynomial.md) have degree at most $\nu$, and the denominator has value one at zero. [Order of a Runge-Kutta method](../../../numerical-analysis.md#order-of-a-runge-kutta-method) $2\nu$ implies that this test-equation approximation agrees with $e^z$ through degree $2\nu$:

$$
R(z)-e^z=O(z^{2\nu+1}).
$$

By uniqueness of the diagonal [Padé approximant](../../../isolated-singularity.md#pade-approximant), $R=[\nu/\nu]_{e^z}$. Explicitly,

$$
R(z)=\frac{P_\nu(z)}{P_\nu(-z)},\qquad
P_\nu(z)=\sum_{j=0}^\nu\frac{(2\nu-j)!\,\nu!}{(2\nu)!\,j!\,(\nu-j)!}\,z^j.
$$

The permitted diagonal [Padé approximant](../../../isolated-singularity.md#pade-approximant) property says this [rational function](../../../isolated-singularity.md#rational-function) has no poles in the closed left half-plane and satisfies $|R(z)|\le1$ there. Therefore

$$
\boxed{\text{Every }\nu\text{-stage Runge-Kutta method of order }2\nu\text{ is A-stable}.}
$$

There is also no hidden stage-solve singularity from a canceled denominator: the [Padé approximant](../../../isolated-singularity.md#pade-approximant) numerator and denominator are coprime and each has degree $\nu$. The original [determinant](../../../linear-algebra.md#determinant) denominator already has degree at most $\nu$, so, with its normalization at zero, it equals $P_\nu(-z)$ and cannot contain an additional canceled factor. This proves [maximal-order Runge-Kutta methods are A-stable](../../../numerical-analysis.md#maximal-order-runge-kutta-methods-are-a-stable).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the [Gauss collocation coefficient construction](../../../numerical-analysis.md#gauss-collocation-coefficient-construction). Find the $\nu$ [polynomial roots](../../../polynomial.md#root-of-a-polynomial) $c_1,\ldots,c_\nu$ of the shifted [Legendre polynomial](../../../differential-equation.md#legendre-polynomial) $P_\nu(2c-1)$ in $(0,1)$, and form

$$
\ell_j(s)=\prod_{m\ne j}\frac{s-c_m}{c_j-c_m}.
$$

Then set

$$
\boxed{a_{ij}=\int_0^{c_i}\ell_j(s)ds,\qquad b_j=\int_0^1\ell_j(s)ds.}
$$

These are explicit [polynomial](../../../polynomial.md) [integrals](../../../calculus.md#integral). For example, if $\ell_j(s)=\sum_{r=0}^{\nu-1}d_{jr}s^r$, calculate $a_{ij}=\sum_rd_{jr}c_i^{r+1}/(r+1)$ and $b_j=\sum_rd_{jr}/(r+1)$. The resulting implicit [Gauss collocation method](../../../numerical-analysis.md#gauss-legendre-method) has order $2\nu$; its [Gaussian quadrature](../../../numerical-analysis.md#gaussian-quadrature) nodes integrate [polynomials](../../../polynomial.md) through degree $2\nu-1$ exactly. The one-stage example is the [implicit midpoint rule](../../../numerical-analysis.md#implicit-midpoint-rule), with $c_1=a_{11}=1/2$ and $b_1=1$. No search over nonlinear [Runge-Kutta order conditions](../../../numerical-analysis.md#butcher-order-condition) systems is needed.

## 2

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $h=\Delta x$, $k=\Delta t$, with fixed positive $\mu=k/h$. Insert a smooth exact solution and divide the residual by $2k$:

$$
\frac{u(t+k)-u(t-k)}{2k}
-\frac{u(x+h,y)-u(x-h,y)+u(x,y+h)-u(x,y-h)}{2h}.
$$

[Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
u_t-u_x-u_y+\frac{k^2}{6}u_{ttt}-\frac{h^2}{6}(u_{xxx}+u_{yyy})+O(k^4+h^4).
$$

The [differential equation](../../../differential-equation.md) cancels the leading part, leaving normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) $O(k^2+h^2)$. Since $u_{ttt}=(\partial_x+\partial_y)^3u$ contains mixed [derivatives](../../../calculus.md#derivative), there is no fixed positive [Courant number](../../../finite-difference.md#courant-number) canceling this leading error for every smooth solution. Thus **the method is second order in time and space**. Global second-order convergence also requires [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) and initial values at both time levels accurate enough to retain this order.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use a spatial [discrete Fourier mode](../../../numerical-analysis.md#discrete-fourier-mode) $u_{k,j}^n=a_ne^{i(k\xi+j\eta)}$. Its recurrence and [amplification polynomial of a multilevel finite difference scheme](../../../finite-difference.md#amplification-polynomial-of-a-multilevel-finite-difference-scheme) are

$$
a_{n+1}=2is\,a_n+a_{n-1},\qquad G^2-2isG-1=0,\qquad
s=\mu(\sin\xi+\sin\eta).
$$

The [polynomial roots](../../../polynomial.md#root-of-a-polynomial) are $G_\pm=is\pm\sqrt{1-s^2}$. For $|s|<1$ both have modulus one and are separated. Since $|\sin\xi+\sin\eta|\le2$, a fixed $0<\mu<1/2$ bounds their separation below by $2\sqrt{1-4\mu^2}$. The two-level [companion matrix](../../../linear-operator-theory.md#companion-matrix) is therefore diagonalizable with uniformly bounded [eigenvector](../../../linear-operator-theory.md#eigenvector) [matrix](../../../vector-space.md#matrix) and inverse. To see the uniform bound explicitly, write $V=\begin{pmatrix}G_+&G_-\\1&1\end{pmatrix}$. Its determinant is $G_+-G_-$; all its entries have modulus one, and those of $V^{-1}$ are bounded by the reciprocal of the root separation. The companion matrix powers are $V\operatorname{diag}(G_+^n,G_-^n)V^{-1}$, bounded independently of frequency and step number. [Parseval's identity](../../../fourier-analysis.md#parseval-identity) converts this into a mesh-independent discrete $L^2$ bound for arbitrary perturbations at the two initial levels.

If $\mu>1/2$, choose $\xi=\eta=\pi/2$. Then $s=2\mu>1$, and one [polynomial root](../../../polynomial.md#root-of-a-polynomial) has modulus $s+\sqrt{s^2-1}>1$. On periodic meshes with the number of points divisible by four, this is an actual grid mode, producing exponential [linear instability](../../../algebra.md#linear-instability).

At $\mu=1/2$ the same phases give $(G-i)^2$. The [companion matrix](../../../linear-operator-theory.md#companion-matrix) is not a [scalar matrix](../../../linear-algebra.md#scalar-matrix), so the double [polynomial root](../../../polynomial.md#root-of-a-polynomial) has a nontrivial [Jordan block](../../../linear-operator-theory.md#jordan-block). The solution $a_n=ni^n$ has bounded starting amplitudes but grows like $n$. On a fixed physical time interval $n$ is of order $1/k$, so no mesh-independent [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) bound exists. Consequently

$$
\boxed{0<\mu<\tfrac12}
$$

is the [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) interval under the standard two-level definition. Testing only [polynomial root](../../../polynomial.md#root-of-a-polynomial) moduli would misleadingly include the endpoint. A special startup selecting the non-growing branch at that endpoint restricts the perturbations and does not establish [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) of the full recurrence. This is the [two-dimensional leapfrog stability threshold](../../../finite-difference.md#two-dimensional-leapfrog-stability-threshold).

## 3

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The first [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) factors as

$$
\rho(w)=(w-1)(w^2-2\alpha w+1).
$$

Also $\rho(1)=0$ and $\rho'(1)=\sigma(1)=2(1-\alpha)$, so the [order conditions for a linear multistep method](../../../numerical-analysis.md#order-conditions-for-a-linear-multistep-method) hold for every $\alpha$. Convergence of the full [linear multistep method](../../../numerical-analysis.md#linear-multistep-method) recurrence requires, in addition, the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method): all [polynomial roots](../../../polynomial.md#root-of-a-polynomial) of $\rho$ lie in the closed unit disk and its [polynomial roots](../../../polynomial.md#root-of-a-polynomial) on the unit circle are simple.

For $-1<\alpha<1$, write $\alpha=\cos\theta$ with $0<\theta<\pi$. The other [polynomial roots](../../../polynomial.md#root-of-a-polynomial) are $e^{\pm i\theta}$, distinct from each other and from 1, so the [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) holds. For $|\alpha|>1$, the two quadratic [polynomial roots](../../../polynomial.md#root-of-a-polynomial) are real and reciprocal, and one has modulus greater than one. At $\alpha=1$, $\rho=(w-1)^3$; at $\alpha=-1$, $\rho=(w-1)(w+1)^2$. Both endpoints violate simplicity. [Consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) plus [zero-stability](../../../numerical-analysis.md#zero-stability) therefore gives

$$
\boxed{-1<\alpha<1.}
$$

The conclusion applies to the recurrence as printed, including its starting data. Canceling common factors is not innocuous: at $\alpha=1$ the [polynomials](../../../polynomial.md) contain $(w-1)^2$, and at $\alpha=-13/5$ they contain $w+5$. The reduced recurrences exclude parasitic solutions of the original one. This is the [common-factor cancellation defect in a multistep recurrence](../../../numerical-analysis.md#common-factor-cancellation-defect-in-a-multistep-recurrence), so those parameter values are not added to the interval.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply the [exponential-symbol order criterion for a multistep method](../../../numerical-analysis.md#exponential-symbol-order-criterion-for-a-multistep-method), which follows by substituting the [bilateral shift operator](../../../banach-algebra.md#bilateral-shift-operator) $e^{h\partial_t}$ into the exact-solution residual. Direct expansion gives

$$
\rho(e^z)-z\sigma(e^z)
=-\frac{\alpha+5}{12}z^4-\frac{14\alpha+61}{90}z^5+O(z^6).
$$

All coefficients through degree three vanish. If $\alpha\ne-5$, the fourth-degree coefficient is nonzero, so the normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) has exact order three. At $\alpha=-5$, the fourth-degree coefficient vanishes and the fifth-degree coefficient is $1/10$, which is nonzero. Thus

$$
\boxed{p=3\text{ if }\alpha\ne-5,\qquad p=4\text{ if }\alpha=-5.}
$$

This is the formal order of the full recurrence. The order-four member is not [zero-stable](../../../numerical-analysis.md#zero-stability), so it is not convergent. All the convergent members from part (a) have order three. At the degenerate value $\alpha=1$, the full recurrence still has formal order three, while cancellation of its common factor gives [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) of order one; that cancellation changes the method rather than its order calculation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $|\alpha|>1$, an exterior [polynomial root](../../../polynomial.md#root-of-a-polynomial) of $\rho$ persists by [continuity](../../../calculus.md#continuous-function) for sufficiently small negative real $z$ in the [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) [polynomial](../../../polynomial.md) $\rho(w)-z\sigma(w)$. Hence these parameters cannot be [A-stable](../../../numerical-analysis.md#a-stability).

For $-1\le\alpha<1$, the principal [polynomial root](../../../polynomial.md#root-of-a-polynomial) at $w=1,z=0$ is simple. Let $s(z)=\log w(z)$ denote its analytic [logarithm](../../../calculus.md#logarithm) near zero. Using the expansion in part (b), and $\rho'(1)=2(1-\alpha)$, solve the [polynomial root](../../../polynomial.md#root-of-a-polynomial) equation to obtain

$$
s(z)=z+Cz^4+O(z^5),\qquad C=\frac{\alpha+5}{24(1-\alpha)}>0.
$$

Indeed the residual at $s=z$ is $-(\alpha+5)z^4/12$, and the correction in $s$ cancels it by multiplication with $2(1-\alpha)$. Choose $z=-C\varepsilon^4/2+i\varepsilon$. This lies strictly in the left half-plane, but

$$
\operatorname{Re}s(z)=\frac C2\varepsilon^4+O(\varepsilon^5)>0
$$

for small positive $\varepsilon$. Thus $|w(z)|=e^{\operatorname{Re}s(z)}>1$, proving [linear instability](../../../algebra.md#linear-instability) within the [A-stability](../../../numerical-analysis.md#a-stability) domain. This is a direct [principal-root obstruction to A-stability](../../../numerical-analysis.md#principal-root-obstruction-to-a-stability), rather than an appeal to an order-barrier theorem alone.

Finally, at $\alpha=1$, the full [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) [polynomial](../../../polynomial.md) is

$$
\rho(w)-z\sigma(w)=(w-1)^2\bigl((1-z)w-1\bigr).
$$

It retains a double unit [polynomial root](../../../polynomial.md#root-of-a-polynomial) for every negative $z$, allowing growing parasitic solutions. Therefore

$$
\boxed{\text{There is no real }\alpha\text{ for which the printed recurrence is A-stable}.}
$$

The canceled [Backward Euler method](../../../numerical-analysis.md#backward-euler-method) recurrence at $\alpha=1$ is [A-stable](../../../numerical-analysis.md#a-stability), but its admissible solutions and starting relations differ from those of the original method.

## 4

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Take $L=-d^2/dx^2+x$. The [Airy equation](../../../integrable-systems.md#airy-equation) is $Lu=0$. To discuss positivity of this [linear operator](../../../vector-space.md#linear-operator), use its homogeneous variation domain $D(L)=\{v\in H^2(0,1):v(0)=0,\ v'(1)=0\}$. [Integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\langle v,Lv\rangle_{L^2}=\int_0^1\bigl(|v'|^2+x|v|^2\bigr)dx>0\qquad(v\ne0).
$$

The boundary term is zero at both ends. The same calculation with two different functions proves that the associated form is a [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form). Positivity here concerns the homogeneous domain; the condition $u(0)=1$ instead defines an affine set of admissible solutions.

For the [variational problem](../../../calculus-of-variations.md#variational-problem) define

$$
V=\{v\in H^1(0,1):v(0)=0\},\qquad a(v,w)=\int_0^1(v'w'+xvw)dx,
$$

and minimize

$$
\boxed{J[u]=\frac12\int_0^1(u'^2+xu^2)dx\quad\text{over }u\in1+V.}
$$

The [Sobolev trace](../../../sobolev-space.md#trace-operator) at zero is meaningful in $H^1$. No [derivative](../../../calculus.md#derivative) boundary value is imposed on this trial space: the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) will emerge naturally. For $v\in V$, [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and integration give

$$
|v(x)|^2\le x\int_0^x|v'(s)|^2ds,\qquad
\|v\|_2^2\le\tfrac12\|v'\|_2^2,
$$

so $a(v,v)\ge\tfrac23\|v\|_{H^1}^2$. Thus $a$ is a bounded, symmetric, [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form) on the [Hilbert space](../../../hilbert-space.md) $V$. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) says that a bounded [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form) and a bounded [linear functional](../../../linear-algebra.md#linear-functional) determine a unique [weak solution](../../../partial-differential-equation.md#weak-solution). Apply it to

$$
a(v,w)=-\int_0^1xw\,dx\qquad(w\in V),
$$

and set $u=1+v$. This is precisely the [first variation](../../../calculus-of-variations.md#first-variation) condition $a(u,w)=0$ for $J$.

Compactly supported [test functions](../../../distribution-theory.md#test-function) first yield $u''=xu$ in the sense of [distributional derivatives](../../../distribution-theory.md#distributional-derivative). Since $xu\in L^2$, the solution is in $H^2$. [Integration by parts](../../../calculus.md#integration-by-parts) then leaves $u'(1)w(1)=0$ for every $w\in V$, hence $u'(1)=0$. The other [boundary condition](../../../differential-equation.md#boundary-condition) is built into $1+V$. Conversely a solution of this [boundary value problem](../../../differential-equation.md#boundary-value-problem) satisfies the [first variation](../../../calculus-of-variations.md#first-variation) condition. Finally,

$$
J[u+w]-J[u]=a(u,w)+\tfrac12a(w,w)=\tfrac12a(w,w)>0\qquad(0\ne w\in V).
$$

This proves existence, uniqueness and the global minimum characterization, including the natural [boundary condition](../../../differential-equation.md#boundary-condition). It is the [mixed-boundary Airy energy principle](../../../integrable-systems.md#mixed-boundary-airy-energy-principle).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose a partition $0=x_0<x_1<\cdots<x_N=1$, with the usual nodal [piecewise-linear hat functions](../../../numerical-analysis.md#piecewise-linear-hat-function) $\phi_i$, including the half hats at the endpoints. Write $u_h=\sum_{i=0}^NU_i\phi_i$ with $U_0=1$. Differentiating the [Ritz method](../../../numerical-analysis.md#rayleigh-ritz-method) energy with respect to $U_i$, $1\le i\le N$, gives

$$
\sum_{j=0}^NA_{ij}U_j=0,\qquad A_{ij}=\int_0^1(\phi_i'\phi_j'+x\phi_i\phi_j)dx.
$$

On an element $[a,b]$ of length $\ell$, its two basis functions are $(b-x)/\ell$ and $(x-a)/\ell$. Direct integration yields the element [matrix](../../../vector-space.md#matrix)

$$
\boxed{A^{[a,b]}=\frac1\ell\begin{pmatrix}1&-1\\-1&1\end{pmatrix}
+\frac\ell{12}\begin{pmatrix}3a+b&a+b\\a+b&a+3b\end{pmatrix}.}
$$

For example the first weighted diagonal is $\int_a^bx(b-x)^2/\ell^2\,dx=\ell(3a+b)/12$; the off-diagonal is $\int_a^bx(b-x)(x-a)/\ell^2\,dx=\ell(a+b)/12$. This gives the [affine-weighted hat mass matrix](../../../numerical-analysis.md#affine-weighted-hat-mass-matrix) and explicit equations on any partition by assembling adjacent elements.

For the uniform choice $h=1/N$, $x_i=ih$, the assembled interior equations are

$$
\boxed{\left[-\frac1h+\frac h{12}(2x_i-h)\right]U_{i-1}
+\left[\frac2h+\frac{2hx_i}{3}\right]U_i
+\left[-\frac1h+\frac h{12}(2x_i+h)\right]U_{i+1}=0,\quad1\le i<N.}
$$

The last node contributes only one element, so its equation is

$$
\boxed{\left[-\frac1h+\frac h{12}(2-h)\right]U_{N-1}
+\left[\frac1h+\frac h3-\frac{h^2}{12}\right]U_N=0,\qquad U_0=1.}
$$

In the first interior equation the known $U_0$ term moves to the right, giving $1/h-h^2/12$. For $N=1$ only the endpoint equation is needed. The last row enforces the weak [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition), so no artificial value outside the interval is introduced. The [matrix](../../../vector-space.md#matrix) on $U_1,\ldots,U_N$ is a [symmetric positive-definite matrix](../../../linear-algebra.md#symmetric-positive-definite-matrix): its [quadratic form](../../../linear-algebra.md#quadratic-form) is $a(v_h,v_h)>0$ for every nonzero trial variation $v_h$. The discrete minimizer is therefore unique.

## 5

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $h=\Delta x$, $k=\mu h$ and $M_r=\sum_{j\in\{-2,-1,1,2\}}a_jj^r$. Along a smooth solution, $\partial_t^r u=\partial_x^r u$. The exact difference $u(x,t+k)-u(x,t-k)$ contains only odd [derivatives](../../../calculus.md#derivative). Matching terms through degree four therefore requires

$$
M_0=M_2=M_4=0,\qquad M_1=2\mu,\qquad M_3=2\mu^3.
$$

The first two conditions give $a_{-1}+a_1=a_{-2}+a_2=0$, which also implies $M_4=0$. With $a_{-j}=-a_j$, the remaining equations are $a_1+2a_2=\mu$ and $a_1+8a_2=\mu^3$. Hence

$$
\boxed{a_1=\frac{\mu(4-\mu^2)}3,\qquad a_2=\frac{\mu(\mu^2-1)}6,\qquad a_{-1}=-a_1,\quad a_{-2}=-a_2.}
$$

The fifth spatial moment is $M_5=10\mu^3-8\mu$. After dividing the exact-minus-scheme residual by $2k$, its first possible nonzero term is

$$
\frac{h^4}{120}(\mu^2-1)(\mu^2-4)u_{xxxxx}+O(h^6).
$$

This is the [fourth-order two-step advection stencil](../../../finite-difference.md#fourth-order-two-step-advection-stencil). Thus the normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) is $O(h^4)$ at fixed positive [Courant number](../../../finite-difference.md#courant-number), as required. At $\mu=1$ or $2$ the formula translates the physical advection branch exactly, but [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) alone does not decide [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) of all two-level perturbations.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

[Fourier transform](../../../analysis.md#fourier-transform) on the infinite spatial lattice gives

$$
a_{n+1}=2iA(\theta)a_n+a_{n-1},\qquad
A(\theta)=a_1\sin\theta+a_2\sin2\theta,
$$

with [polynomial roots](../../../polynomial.md#root-of-a-polynomial) $G_\pm=iA\pm\sqrt{1-A^2}$. When $|A|$ is uniformly less than one, the [polynomial roots](../../../polynomial.md#root-of-a-polynomial) have modulus one and a uniform positive separation. Diagonalizing the [companion matrix](../../../linear-operator-theory.md#companion-matrix) then bounds all its powers independently of $\theta$ and $n$. [Parseval's identity](../../../fourier-analysis.md#parseval-identity) proves [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) in the discrete $L^2$ [norm](../../../functional-analysis.md#norm) for arbitrary square-summable starting perturbations at both levels.

At $\mu=1/2$ the coefficients give

$$
A(\theta)=\frac58\sin\theta-\frac1{16}\sin2\theta
=\frac{\sin\theta(5-\cos\theta)}8,\qquad |A(\theta)|\le\frac34<1.
$$

Consequently **$\mu=1/2$ is stable**.

At $\mu=3/2$,

$$
A(\theta)=\frac78\sin\theta+\frac5{16}\sin2\theta,
\qquad A(\pi/3)=\frac{19\sqrt3}{32}>1.
$$

The growing [polynomial root](../../../polynomial.md#root-of-a-polynomial) at this phase has modulus

$$
\boxed{|G|=\frac{19\sqrt3+\sqrt{59}}{32}>1.}
$$

To turn this into a [Cauchy problem](../../../partial-differential-equation.md#cauchy-problem) [linear instability](../../../algebra.md#linear-instability) proof, rather than rely on a [plane wave](../../../quantum-mechanics.md#plane-wave) of infinite [norm](../../../functional-analysis.md#norm), choose a small interval around $\pi/3$ on which the growing [polynomial root](../../../polynomial.md#root-of-a-polynomial) has modulus at least $1+\delta$. Choose an initial [Fourier transform](../../../analysis.md#fourier-transform) amplitude that is a nonzero [square-integrable function](../../../measure-theory.md#square-integrable-function) supported there, and set the level-one amplitude equal to that [polynomial root](../../../polynomial.md#root-of-a-polynomial) times the level-zero amplitude. The recurrence then multiplies by the same growing [polynomial root](../../../polynomial.md#root-of-a-polynomial) at every step on the support. [Parseval identity](../../../fourier-analysis.md#parseval-identity) gives $\|u^n\|_2\ge(1+\delta)^n\|u^0\|_2$, whereas both initial [norms](../../../functional-analysis.md#norm) are bounded independently of $h$. Real data can be obtained by adding the conjugate interval around $-\pi/3$. Since $n=T/(\mu h)$ tends to infinity at fixed $T$, **$\mu=3/2$ is unstable**.

## 6

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [Engquist-Osher method](../../../numerical-analysis.md#engquist-osher-method) is an upwind [finite volume method](../../../numerical-analysis.md#finite-volume-method). For cell values $U_j^n$, mesh width $h$ and time step $k$, put $r=k/h$ and use the conservative update

$$
U_j^{n+1}=U_j^n-r\bigl[F(U_j^n,U_{j+1}^n)-F(U_{j-1}^n,U_j^n)\bigr],
$$

where the [numerical flux](../../../numerical-analysis.md#numerical-flux) is

$$
\boxed{F(a,b)=f(0)+\int_0^a\max\{f'(s),0\}ds+\int_0^b\min\{f'(s),0\}ds.}
$$

[Consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) follows from $F(u,u)=f(u)$. Positive [characteristic speeds](../../../partial-differential-equation.md#characteristic-speed) use the left state, and negative speeds use the right state. The flux difference telescopes when summed over cells, giving a discrete [conservation law](../../../physics.md#conservation-law). The method is first order in space and time for smooth solutions; its [conservation law](../../../physics.md#conservation-law) form is also appropriate when [shock waves](../../../partial-differential-equation.md#shock-wave) develop.

Let $s_*$ be the unique [sonic point of a scalar flux](../../../partial-differential-equation.md#sonic-point-of-a-scalar-flux), $f'(s_*)=0$. [Convexity](../../../real-analysis.md#convex-function) implies $f'<0$ to its left and $f'>0$ to its right. Put $f_*=f(s_*)$ and split

$$
f^+(u)=\begin{cases}0&u\le s_*,\\f(u)-f_*&u>s_*,\end{cases}
\qquad f^-(u)=\begin{cases}f(u)-f_*&u<s_*,\\0&u\ge s_* .\end{cases}
$$

Then $f=f_*+f^++f^-$, $(f^+)'\ge0$, $(f^-)'\le0$, and

$$
F(a,b)=f_*+f^+(a)+f^-(b).
$$

This is the [sonic-point splitting of a convex Engquist-Osher flux](../../../numerical-analysis.md#sonic-point-splitting-of-a-convex-engquist-osher-flux). If both states are above $s_*$, $F=f(a)$; if both are below it, $F=f(b)$. Across a transsonic [rarefaction wave](../../../partial-differential-equation.md#rarefaction-wave), $a\le s_*\le b$, the flux is the minimum $f_*$. In the opposite crossing it is $f(a)+f(b)-f_*$, which in general differs from the exact [Godunov numerical flux](../../../numerical-analysis.md#godunov-numerical-flux). This distinction does not affect the [monotonicity](../../../calculus.md#monotonic-function) proof.

Here [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) requires the usual [Courant–Friedrichs–Lewy condition](../../../finite-difference.md#courant-friedrichs-lewy-condition). Let the initial values lie in $[m,M]$, and choose

$$
\boxed{r\max_{u\in[m,M]}|f'(u)|\le1.}
$$

A differentiable [convex function](../../../real-analysis.md#convex-function) has a continuous [derivative](../../../calculus.md#derivative) on this interval, so the maximum is finite. Write the three-input update as $H(a,b,c)$. Differentiating gives

$$
H_a=r(f^+)'(a)\ge0,\qquad H_c=-r(f^-)'(c)\ge0,\qquad
H_b=1-r\bigl[(f^+)'(b)-(f^-)'(b)\bigr]=1-r|f'(b)|\ge0.
$$

Thus the update $T$ preserves componentwise order. Constants are fixed, since $H(c,c,c)=c$, so comparison with the constants $m,M$ proves $m\le U_j^n\le M$ for every time level. In particular the same [CFL condition](../../../finite-difference.md#courant-friedrichs-lewy-condition) remains applicable. This is a mesh-independent maximum-principle [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) bound.

A stronger [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) statement is contraction in discrete $L^1$. Consider two solutions $U,V$ in the same invariant interval, on a periodic mesh or on the infinite lattice with summable differences. Let $Q=U\vee V$ be their componentwise maximum. [Monotonicity](../../../calculus.md#monotonic-function) gives $TQ\ge TU,TV$, hence

$$
\sum_j(TU_j-TV_j)^+\le\sum_j(TQ_j-TV_j)
=\sum_j(Q_j-V_j)=\sum_j(U_j-V_j)^+.
$$

The discrete [conservation law](../../../physics.md#conservation-law) for the difference gives the equality: on a finite periodic mesh the flux sum cancels exactly, and on the infinite lattice it follows by truncation and the fact that the flux is a [Lipschitz function](../../../real-analysis.md#lipschitz-continuity) on $[m,M]$. Interchanging $U,V$ and adding proves

$$
\boxed{h\sum_j|U_j^{n+1}-V_j^{n+1}|\le h\sum_j|U_j^n-V_j^n|.}
$$

This is [L1 contraction of a monotone conservative scheme](../../../numerical-analysis.md#l1-contraction-of-a-monotone-conservative-scheme). Since $T$ commutes with the cell shift, applying this contraction to $U$ and its shift gives $\sum_j|U_{j+1}^{n+1}-U_j^{n+1}|\le\sum_j|U_{j+1}^n-U_j^n|$. The scheme is therefore a [total variation diminishing scheme](../../../numerical-analysis.md#total-variation-diminishing-scheme) as well.

The same order argument proves a [discrete entropy inequality](../../../partial-differential-equation.md#discrete-entropy-inequality), explaining why this stable discretization selects [entropy solutions](../../../partial-differential-equation.md#entropy-solution) rather than nonphysical expansion [shock waves](../../../partial-differential-equation.md#shock-wave). For a constant $c\in[m,M]$, set

$$
Q_c(a,b)=F(a\vee c,b\vee c)-F(a\wedge c,b\wedge c).
$$

Because $T(U\vee c)\ge TU,c$ and $T(U\wedge c)\le TU,c$, their componentwise difference is at least $|TU-c|$. Subtracting their updates gives

$$
|U_j^{n+1}-c|\le|U_j^n-c|-r\bigl[Q_c(U_j^n,U_{j+1}^n)-Q_c(U_{j-1}^n,U_j^n)\bigr].
$$

For constants outside $[m,M]$, the entropy inequality is an equality by the invariant bound and the conservative update. At equal states $Q_c(u,u)=\operatorname{sgn}(u-c)[f(u)-f(c)]$, the [Kruzhkov entropy flux](../../../partial-differential-equation.md#kruzhkov-entropy-flux). The flux is a [Lipschitz function](../../../real-analysis.md#lipschitz-continuity) on the invariant interval: writing $L=\max|f'|$, the conservative update gives $h\sum_j|U_j^{n+1}-U_j^n|\le2kL\sum_j|U_{j+1}^n-U_j^n|$. This time-translation bound, the invariant bound and the [total variation](../../../real-analysis.md#total-variation) estimate give local space-time [compactness](../../../topology.md#compact-space) for bounded-variation [initial conditions](../../../differential-equation.md#initial-condition) as the mesh is refined; the conservative update passes to the weak [conservation law](../../../physics.md#conservation-law), and the displayed inequality passes to its [Kruzhkov entropy inequality](../../../partial-differential-equation.md#kruzhkov-entropy-inequality). This identifies the limit as the [entropy solution](../../../partial-differential-equation.md#entropy-solution).

Finally the time-step qualification is essential. For the convex [Inviscid Burgers equation](../../../partial-differential-equation.md#inviscid-burgers-equation) flux $f(u)=u^2/2$, whose unique [sonic point of a scalar flux](../../../partial-differential-equation.md#sonic-point-of-a-scalar-flux) is zero, linearize about a positive constant $U$. The perturbation update becomes $v_j^{n+1}=(1-rU)v_j^n+rUv_{j-1}^n$. At [Fourier frequency](../../../numerical-analysis.md#fourier-frequency) $\pi$ its multiplier is $1-2rU$, with modulus greater than one if $rU>1$. [Wave packets](../../../wave-equation.md#wave-packet) near this phase give [linear instability](../../../algebra.md#linear-instability) even for summable Cauchy perturbations. Thus the assumptions on $f$ imply the [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) results above under the [CFL condition](../../../finite-difference.md#courant-friedrichs-lewy-condition), not for arbitrary $k/h$. This is [CFL necessity for explicit Engquist-Osher stability](../../../numerical-analysis.md#cfl-necessity-for-explicit-engquist-osher-stability).

## 7

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

A [Mehrstellen method](../../../finite-difference.md#mehrstellen-method) gains accuracy by exploiting the [differential equation](../../../differential-equation.md) in the [local truncation error](../../../numerical-analysis.md#local-truncation-error) of a compact [finite difference method](../../../finite-difference.md#finite-difference-method) stencil. The extra nearby values alone do not guarantee higher order: one must also modify the source term. Consider $\Delta u=f$ on a square with prescribed [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data), using the same spacing $h$ in both directions.

For comparison, the [five-point Laplacian](../../../finite-difference.md#five-point-laplacian) has expansion

$$
D_5u=\Delta u+\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).
$$

Its leading error is not a multiple of $\Delta^2u$, because the mixed fourth [derivative](../../../calculus.md#derivative) is missing. To obtain an isotropic leading error, consider a symmetric [nine-point finite-difference stencil](../../../finite-difference.md#nine-point-finite-difference-stencil) with weight $a$ on each axial neighbor, $b$ on each diagonal neighbor, and $c$ on the center, all divided by $h^2$. Vanishing on constants and [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) require $4a+4b+c=0$ and $a+2b=1$. [Taylor expansion](../../../calculus.md#taylor-expansion) then gives the fourth-derivative contribution

$$
h^2\left[\frac1{12}(u_{xxxx}+u_{yyyy})+b\,u_{xxyy}\right].
$$

For this to equal $h^2\Delta^2u/12$ we must choose $b=1/6$, hence $a=2/3$, $c=-10/3$. The resulting [nine-point finite-difference stencil](../../../finite-difference.md#nine-point-finite-difference-stencil) operator is

$$
D_9U_{ij}=\frac{4(U_{i+1,j}+U_{i-1,j}+U_{i,j+1}+U_{i,j-1})
+U_{i+1,j+1}+U_{i+1,j-1}+U_{i-1,j+1}+U_{i-1,j-1}-20U_{ij}}{6h^2}.
$$

Its expansion, retaining the next term for later use, is

$$
D_9u=\Delta u+\frac{h^2}{12}\Delta^2u
+\frac{h^4}{360}\bigl(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy}\bigr)+O(h^6).
$$

Thus $D_9$ by itself is second order on a general function. On a [Poisson equation](../../../partial-differential-equation.md#poisson-equation) solution, however, $\Delta^2u=\Delta f$. Approximating this known source [derivative](../../../calculus.md#derivative) by $D_5f$ gives the fourth-order [Mehrstellen method](../../../finite-difference.md#mehrstellen-method) equation

$$
\boxed{D_9U_{ij}=f_{ij}+\frac{h^2}{12}D_5f_{ij}
=\frac23f_{ij}+\frac1{12}(f_{i+1,j}+f_{i-1,j}+f_{i,j+1}+f_{i,j-1}).}
$$

Equivalently, its two stencils are

$$
\frac1{6h^2}\begin{pmatrix}1&4&1\\4&-20&4\\1&4&1\end{pmatrix}U
=\frac1{12}\begin{pmatrix}0&1&0\\1&8&1\\0&1&0\end{pmatrix}f.
$$

The normalized [local truncation error](../../../numerical-analysis.md#local-truncation-error) is $O(h^4)$, since $D_5f-\Delta f=O(h^2)$. If the equation is multiplied by $6h^2$, the row residual is $O(h^6)$; this change of normalization does not make the solution sixth order. The [fourth-order correction of the nine-point Poisson stencil](../../../finite-difference.md#fourth-order-correction-of-the-nine-point-poisson-stencil) retains only the closest axial and diagonal unknowns. A fourth-order one-dimensional second [derivative](../../../calculus.md#derivative) instead uses $( -U_{i+2}+16U_{i+1}-30U_i+16U_{i-1}-U_{i-2})/(12h^2)$, widening the unknown stencil and introducing negative outer weights. [Mehrstellen method](../../../finite-difference.md#mehrstellen-method) accuracy is obtained by correcting known source values rather than widening that unknown stencil.

The compact scheme has useful [stability](../../../numerical-analysis.md#stability-of-a-numerical-method) and solvability properties. With homogeneous [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data), $-D_9$ is symmetric, has positive diagonal and nonpositive off-diagonal entries, and is a [positive definite symmetric operator](../../../hilbert-space.md#positive-definite-symmetric-operator). Indeed its [quadratic form](../../../linear-algebra.md#quadratic-form) is a sum of positive edge weights times squared differences, with boundary values set to zero. Vanishing of this sum would force a constant on the connected grid and then zero by connection to the boundary. Consequently the [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) [linear system](../../../linear-algebra.md#system-of-linear-equations) has a unique solution. The same weights give a [discrete maximum principle](../../../finite-difference.md#discrete-maximum-principle): if $D_9v\ge0$ at every interior node and $v\le0$ on the boundary, a positive maximum inside would make every weighted difference to its neighbors nonpositive. Equality forces the maximum to propagate to the boundary, which is impossible. Thus $v\le0$ everywhere.

This also turns [consistency of a numerical method](../../../numerical-analysis.md#consistency-of-a-numerical-method) into a quantitative convergence result, rather than merely suggesting an order. Let $B_hf=f+h^2D_5f/12$, let $\tau=D_9u-B_hf$ be the normalized residual of the exact solution, and set $e=U-u$. Exact [Dirichlet boundary data](../../../differential-equation.md#dirichlet-boundary-data) imply $e=0$ on the boundary and $D_9e=-\tau$. On the unit square the quadratic barrier

$$
q(x,y)=\frac{x(1-x)+y(1-y)}4
$$

has $D_9q=-1$ exactly, is nonnegative on the boundary, and has maximum $1/8$. If $\|\tau\|_\infty\le\varepsilon$, then $D_9(e-\varepsilon q)\ge0$ and $D_9(-e-\varepsilon q)\ge0$, while both comparison functions are nonpositive on the boundary. The [discrete maximum principle](../../../finite-difference.md#discrete-maximum-principle) proves

$$
\boxed{|e_{ij}|\le\varepsilon q(x_i,y_j),\qquad
\|U-u\|_\infty\le\tfrac18\|\tau\|_\infty=O(h^4).}
$$

This is [maximum-norm convergence of the corrected nine-point Poisson scheme](../../../finite-difference.md#maximum-norm-convergence-of-the-corrected-nine-point-poisson-scheme). It requires sufficient smoothness of the solution up to the boundary for the uniform truncation bound. On other domains the source and boundary closures must retain the required accuracy; boundary singularities can invalidate a smooth-solution order estimate.

The same expansion reveals how to add still more accuracy. Differentiating $\Delta u=f$ gives

$$
u_{xxxxyy}+u_{xxyyyy}=f_{xxyy},\qquad
u_{xxxxxx}+u_{yyyyyy}=\Delta^2f-3f_{xxyy}.
$$

Thus the sixth [derivatives](../../../calculus.md#derivative) appearing in the $h^4$ term can also be expressed solely through the source. With exact source [derivatives](../../../calculus.md#derivative),

$$
D_9U=f+\frac{h^2}{12}\Delta f
+\frac{h^4}{360}(f_{xxxx}+4f_{xxyy}+f_{yyyy})
$$

is the [sixth-order source correction of the nine-point Poisson stencil](../../../finite-difference.md#sixth-order-source-correction-of-the-nine-point-poisson-stencil), with normalized residual $O(h^6)$. If source [derivatives](../../../calculus.md#derivative) are replaced by differences, $\Delta f$ must be approximated through fourth order and the fourth [derivatives](../../../calculus.md#derivative) through second order to retain that accuracy. The unknowns still occupy the same [nine-point finite-difference stencil](../../../finite-difference.md#nine-point-finite-difference-stencil); only evaluation of known source data becomes more elaborate. The same inverse bound yields sixth-order convergence when these approximations and the boundary data have matching accuracy.

A particularly instructive case is the [Laplace equation](../../../partial-differential-equation.md#laplace-equation), $f=0$. Both displayed error corrections automatically vanish: $\Delta^2u=0$ and $u_{xxxxyy}+u_{xxyyyy}=\Delta u_{xxyy}=0$, which also makes the pure sixth [derivatives](../../../calculus.md#derivative) sum to zero. Expanding the stencil two orders further gives, for a sufficiently smooth [harmonic function](../../../partial-differential-equation.md#harmonic-function),

$$
\boxed{D_9u=\frac{h^6}{3024}u_{xxxxxxxx}+O(h^8).}
$$

For verification, the three eighth-derivative contributions are $(u_{xxxxxxxx}+u_{yyyyyyyy})/20160$, $(u_{xxxxxxyy}+u_{xxyyyyyy})/2160$ and $u_{xxxxyyyy}/864$. Because $u$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function), their sum is $u_{xxxxxxxx}(1/10080-1/1080+1/864)=u_{xxxxxxxx}/3024$. The example $u=\operatorname{Re}(x+iy)^8$ has $D_9u(0,0)=40h^6/3$, so this term is genuinely present. The unmodified harmonic nine-point scheme therefore has sixth-order nodal convergence under the same smoothness and boundary assumptions. This [harmonic superconvergence of the nine-point stencil](../../../finite-difference.md#harmonic-superconvergence-of-the-nine-point-stencil) is special to [harmonic functions](../../../partial-differential-equation.md#harmonic-function); it should not be confused with the fourth-order source-corrected scheme for general [Poisson equation](../../../partial-differential-equation.md#poisson-equation) data.

The appeal of [Mehrstellenverfahren](../../../finite-difference.md#mehrstellen-method) is this combination of a compact [sparse matrix](../../../vector-space.md#sparse-matrix), favorable [discrete maximum principle](../../../finite-difference.md#discrete-maximum-principle) properties, and high accuracy obtained by using the governing equation. The derivation also shows precisely which accuracy belongs to the operator on arbitrary functions, which belongs to its action on solutions, and which survives in the computed boundary-value solution.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
