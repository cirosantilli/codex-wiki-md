# Paper 68

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper68.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper68.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
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
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [uniform norm](../../../functional-analysis.md#supremum-norm) and the central second difference $\delta_h^2f(x)=f(x+h)-2f(x)+f(x-h)$, with

$$
\omega_2(f,a)=\sup_{|h|\leq a}\|\delta_h^2f\|_\infty.
$$

The [Jackson kernel](../../../uniform-approximation.md#jackson-kernel) is even, nonnegative and normalized. Pairing $t$ and $-t$ in its integral therefore gives

$$
j_n f(x)-f(x)=\frac12\int_{-\pi}^{\pi}\delta_t^2f(x)J_n(t)\,dt.
$$

We will estimate this expression directly in terms of the [second modulus of smoothness](../../../uniform-approximation.md#second-modulus-of-smoothness).

First prove the modulus scaling bound. With translations $T_hf(x)=f(x+h)$, the forward difference obeys

$$
(T_{mh}-I)^2=(T_h-I)^2\left(\sum_{r=0}^{m-1}T_{rh}\right)^2.
$$

Each [function translation](../../../function.md#translation-of-a-function) preserves the [uniform norm](../../../functional-analysis.md#supremum-norm), so $\|\delta_{mh}^2f\|_\infty\leq m^2\|\delta_h^2f\|_\infty$. For $t\ne0$, take $m=\lceil n|t|\rceil$ and $h=t/m$. Then $|h|\leq1/n$ and

$$
\|\delta_t^2f\|_\infty\leq(1+n|t|)^2\omega_2(f,1/n).
$$

The same bound is immediate at $t=0$.

For $|t|\leq\pi$, $|\sin(t/2)|\geq|t|/\pi$. Also $|\sin(nt/2)/\sin(t/2)|\leq n$, as follows by expressing the ratio, up to a unit-modulus factor, as a sum of $n$ complex exponentials. The given normalizing coefficient is at most a constant times $n^{-3}$. Consequently

$$
J_n(t)\leq Cn,\qquad
J_n(t)\leq\frac{C}{n^3|t|^4}\quad(t\ne0),
$$

and these two estimates combine into

$$
J_n(t)\leq\frac{C'n}{(1+n|t|)^4}.
$$

Indeed splitting at $n|t|=1$ shows this with an absolute change of constant. Hence

$$
\int_{-\pi}^{\pi}(1+n|t|)^2J_n(t)\,dt
\leq2C'\int_0^{n\pi}\frac{du}{(1+u)^2}\leq2C'.
$$

Substitute the modulus bound in the symmetrized [convolution](../../../fourier-analysis.md#convolution) and take the supremum over $x$ to obtain the [Jackson operator estimate](../../../uniform-approximation.md#jackson-operator-estimate)

$$
\boxed{\|j_nf-f\|_\infty\leq C'\omega_2(f,1/n).}
$$

The constant is independent of $f$ and the positive integer $n$; the kernel's quartic decay is what makes the weighted second-difference integral uniformly bounded.

## 2

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Put $x=\cos\theta$. The trigonometric identity

$$
\cos((n+1)\theta)+\cos((n-1)\theta)=2\cos\theta\cos(n\theta)
$$

gives

$$
\boxed{T_{n+1}(x)=2xT_n(x)-T_{n-1}(x).}
$$

Starting with $T_0=1$ and $T_1=x$, this recurrence proves inductively that each [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) is a [polynomial](../../../polynomial.md). For $n\geq1$, the highest-degree term in $2xT_n$ cannot cancel against $T_{n-1}$, so the degree increases by one and its [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial) doubles. Thus

$$
\boxed{\deg T_n=n,\qquad \operatorname{lc}(T_n)=2^{n-1}\quad(n\geq1).}
$$

The constant [polynomial](../../../polynomial.md) $T_0$ has [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial) one.

For $n\geq1$, the points $x_j=\cos(j\pi/n)$, $j=0,\ldots,n$, give $T_n(x_j)=(-1)^j$. They are all the points where $|T_n|=1$, since $|\cos(n\theta)|=1$ exactly when $n\theta$ is an integer multiple of $\pi$. Therefore there are **$n+1$ equioscillation points**, including the two endpoints. Reversing their order makes an increasing alternating sequence. For $n=0$ the [polynomial](../../../polynomial.md) is constant: every point has unit value, but an alternating sequence has at most one point.

Now take $n\geq1$ and $c=2^{1-n}$. Since $cT_n$ is monic, $p_0(x)=x^n-cT_n(x)$ has degree at most $n-1$, and $\|x^n-p_0\|_\infty=c$. This proves the upper bound for the best error.

For the lower bound, suppose a [polynomial](../../../polynomial.md) $p$ of degree at most $n-1$ had $\|x^n-p\|_\infty<c$. At each of the $n+1$ ordered extrema, $h=p-p_0$ must have the same strictly nonzero sign as $T_n$: if $cT_n=c$, then $|c-h|<c$ gives $h>0$, and if $cT_n=-c$, then $|-c-h|<c$ gives $h<0$. Between every consecutive pair, the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) gives a zero of $h$. These are $n$ distinct zeros, impossible for a nonzero [polynomial](../../../polynomial.md) of degree at most $n-1$; $h=0$ is incompatible with the strict error improvement. This first-principles sign argument proves the [monic Chebyshev extremal polynomial](../../../numerical-analysis.md#monic-chebyshev-extremal-polynomial) bound without using the alternation theorem:

$$
\boxed{E_{n-1}(x^n)=2^{1-n}.}
$$

The displayed $p_0$ supplies an actual best approximating [polynomial](../../../polynomial.md).

## 3

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Work with real-valued functions and put $\operatorname{sign}(0)=0$. Let $r=f-p_*$, and write an arbitrary competitor as $p=p_*+v$ with $v\in U$. Pointwise,

$$
|r-v|\geq |r|-v\,\operatorname{sign}(r).
$$

For $r\ne0$ this is $|r-v|\geq\operatorname{sign}(r)(r-v)$; for $r=0$ the right side is zero. Integrating and using the assumed orthogonality gives

$$
\|f-p\|_1=\int|r-v|
\geq\int|r|-\int v\,\operatorname{sign}(r)
=\|f-p_*\|_1.
$$

Thus **$p_*$ is a best $L^1$ approximation from $U$**. This [sign criterion for best L1 approximation](../../../functional-analysis.md#sign-criterion-for-best-l1-approximation) is sufficient without any finite-dimensionality or uniqueness assumption; possible residual zeros do not invalidate the inequality.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Here $n$ is a positive [integer](../../../number-theory.md#integer) and $m$ is an [integer](../../../number-theory.md#integer) index of a [Fourier coefficient](../../../fourier-series.md#fourier-coefficient). Split a period into $n$ intervals and set $y=nx-2\pi j$ on the $j$th interval. Periodicity and integrability give

$$
\begin{aligned}
\int_0^{2\pi}f(nx)e^{imx}\,dx
&=\frac1n\sum_{j=0}^{n-1}e^{2\pi imj/n}
\int_0^{2\pi}f(y)e^{imy/n}\,dy.
\end{aligned}
$$

For $0<|m|<n$, $\zeta=e^{2\pi im/n}$ is a [root of unity](../../../algebra.md#root-of-unity) different from one and satisfies $\zeta^n=1$, so $\sum_{j=0}^{n-1}\zeta^j=(1-\zeta^n)/(1-\zeta)=0$. Therefore

$$
\boxed{\int_{\mathbb T}f(nx)e^{imx}\,dx=0\qquad(0<|m|<n).}
$$

For $m=0$ the same substitution gives $\int_{\mathbb T}f(nx)\,dx=\int_{\mathbb T}f(x)\,dx$. If the [mean](../../../probability-theory.md#expected-value) of $f$ is zero, this last mode vanishes as well. Since the [linear span](../../../vector-space.md#linear-span) of the exponentials with $|m|\leq n-1$ is the space of [trigonometric polynomials](../../../fourier-series.md#trigonometric-polynomial) of degree at most $n-1$, every pairing with that space is zero. This is the [periodic dilation annihilates low Fourier modes](../../../fourier-series.md#periodic-dilation-annihilates-low-fourier-modes) property. The integer-index assumption is essential; the stated Fourier orthogonality would generally be false for noninteger $m$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

As printed in the original PDF, this claim is false for $n\geq2$. The displayed frequency is one, so the function already belongs to the space of [trigonometric polynomials](../../../fourier-series.md#trigonometric-polynomial) of degree at most $n-1$. Its best approximation is then the function itself, with zero error; for example, $\alpha=1,\beta=0$ gives a zero-approximant error $\int_0^{2\pi}|\cos x|\,dx=4$ instead. For $n=1$, zero is indeed the best constant approximation. Thus the literal answer is

$$
\boxed{p_*=f\quad(n\geq2),\qquad p_*=0\quad(n=1).}
$$

The natural intended version has frequency $n$. Set $g(y)=\alpha\cos y+\beta\sin y$ and $f_n(x)=g(nx)$. The sign function $h(y)=\operatorname{sign}g(y)$ is integrable and satisfies $h(y+\pi)=-h(y)$, so its [mean](../../../probability-theory.md#expected-value) is zero. Part (b) makes $h(nx)=\operatorname{sign}f_n(x)$ orthogonal to every degree-at-most-$n-1$ [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial). Part (a), with $p_*=0$, now proves

$$
\boxed{\text{The best approximation to }\alpha\cos(nx)+\beta\sin(nx)
\text{ from }\mathcal T_{n-1}\text{ in }L^1\text{ is }0.}
$$

The error is $4\sqrt{\alpha^2+\beta^2}$ for the unnormalized integral over a period.

The best approximant is unique. If the amplitude is nonzero and another continuous [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) $p$ has the same optimal error, equality in part (a)'s pointwise inequality holds almost everywhere. Near each zero of $f_n$, the function changes sign; if $p$ did not vanish at that zero, continuity would force an interval on one side where $f_n-p$ has the wrong sign, making the integral inequality strict. Thus $p$ vanishes at all $2n$ distinct zeros of $f_n$. A nonzero [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) of degree at most $n-1$ has at most $2n-2$ zeros in one period, since multiplication by $e^{i(n-1)x}$ turns it into a [polynomial](../../../polynomial.md) in $e^{ix}$ of degree at most $2n-2$. Hence $p=0$. Zero amplitude is immediate. The same reasoning proves the literal frequency-one assertion when $n=1$, while retaining the counterexample for larger $n$.

## 4

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For fixed $t$, put $g_t(u)=(u-t)_+^{k-1}$, a [truncated power function](../../../polynomial.md#truncated-power-function). Begin with distinct increasing knots. The two [interpolation polynomials](../../../numerical-analysis.md#interpolation-polynomial) $\ell_i(\cdot,t)$ and $\ell_{i+1}(\cdot,t)$ agree at their $k-1$ shared knots. Their difference has degree at most $k-1$, so

$$
\ell_{i+1}(x,t)-\ell_i(x,t)=c_i(t)\prod_{j=1}^{k-1}(x-t_{i+j})
=c_i(t)\omega_i(x).
$$

For $k=1$ the empty product is one and the same assertion holds for constant interpolants. The [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial) of a degree-at-most-$k-1$ interpolant on $k$ nodes is its order-$k-1$ [divided difference](../../../numerical-analysis.md#divided-difference), by the [Newton interpolation polynomial](../../../numerical-analysis.md#newton-polynomial). Therefore

$$
c_i(t)=[t_{i+1},\ldots,t_{i+k}]g_t-[t_i,\ldots,t_{i+k-1}]g_t
=(t_{i+k}-t_i)[t_i,\ldots,t_{i+k}]g_t=N_i(t).
$$

This proves the [Lee interpolation identity](../../../uniform-approximation.md#lee-interpolation-identity)

$$
\boxed{\omega_i(x)N_i(t)=\ell_{i+1}(x,t)-\ell_i(x,t).}
$$

The identity holds for every real $x,t$, with the usual convention for the order-zero truncated power. Admissible repeated knots are handled by the corresponding confluent [divided differences](../../../numerical-analysis.md#divided-difference) and consistent one-sided limits at breakpoints; taking these limits preserves the [Lee interpolation identity](../../../uniform-approximation.md#lee-interpolation-identity).

Sum over $i$ to telescope:

$$
\sum_{i=1}^n\omega_i(x)N_i(t)=\ell_{n+1}(x,t)-\ell_1(x,t).
$$

If $t_k<t<t_{n+1}$, the first $k$ knot values of $g_t$ are zero, so $\ell_1=0$. At the last $k$ knots $t_{n+1},\ldots,t_{n+k}$, the function $g_t$ agrees with the [polynomial](../../../polynomial.md) $(u-t)^{k-1}$, so uniqueness of [polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) gives $\ell_{n+1}(x,t)=(x-t)^{k-1}$. Thus the [Marsden identity](../../../uniform-approximation.md#marsden-identity) is

$$
\boxed{(x-t)^{k-1}=\sum_{i=1}^n\omega_i(x)N_i(t),
\qquad t_k<t<t_{n+1},\quad x\in\mathbb R.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $d=k-1$ and let $e_m$ denote the [elementary symmetric polynomial](../../../polynomial.md#elementary-symmetric-polynomial) of degree $m$ in the $d$ interior knots $t_{i+1},\ldots,t_{i+d}$, with $e_0=1$. Expand the two sides of the [Marsden identity](../../../uniform-approximation.md#marsden-identity) as [polynomials](../../../polynomial.md) in $x$:

$$
(x-t)^d=\sum_{m=0}^d(-1)^m\binom dm t^m x^{d-m},
$$

and

$$
\omega_i(x)=\prod_{j=1}^d(x-t_{i+j})
=\sum_{m=0}^d(-1)^m e_m(t_{i+1},\ldots,t_{i+d})x^{d-m}.
$$

Comparing the coefficient of $x^{d-m}$ and cancelling the common sign gives the [monomial B-spline coefficients](../../../uniform-approximation.md#monomial-b-spline-coefficients)

$$
\boxed{a_i^{(m)}=
\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}},
\qquad 0\leq m\leq k-1.}
$$

Equivalently,

$$
a_i^{(m)}=\binom{k-1}{m}^{-1}
\sum_{1\leq j_1<\cdots<j_m\leq k-1}
t_{i+j_1}\cdots t_{i+j_m}.
$$

In particular $a_i^{(0)}=1$, giving [partition of unity](../../../differential-geometry.md#partition-of-unity) on the interior interval. For $k\geq2$, $a_i^{(1)}=(t_{i+1}+\cdots+t_{i+k-1})/(k-1)$, and the highest-degree coefficient is the product of those interior knots. The formulas also cover $k=1,m=0$ through empty products.

## 5

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

There are $n$ basis [splines](../../../uniform-approximation.md#spline-mathematics) for the stated $n+k$ knots; the upper limit $k$ in the printed basis list is an indexing slip. Let

$$
A_{ij}=N_j(x_i^*),\qquad i,j=1,\ldots,n.
$$

The strictly increasing sites and $t_i<x_i^*<t_{i+k}$ give invertibility by the [Schoenberg–Whitney theorem](../../../uniform-approximation.md#schoenberg-whitney-theorem). The needed additional [matrix](../../../vector-space.md#matrix) property is [total nonnegativity of B-spline collocation matrices](../../../uniform-approximation.md#total-nonnegativity-of-b-spline-collocation-matrices): every ordered minor of $A$ is nonnegative.

Here is a structural justification of that sign property. [Knot insertion](../../../uniform-approximation.md#knot-insertion) refines [spline](../../../uniform-approximation.md#spline-mathematics) coefficients by rules of the form $b_j=\alpha_j a_j+(1-\alpha_j)a_{j-1}$, $0\leq\alpha_j\leq1$, with the usual unchanged coefficients before the insertion and shifted coefficients after it. Each coefficient map is a nonnegative rectangular bidiagonal [matrix](../../../vector-space.md#matrix); all its ordered minors are nonnegative, as its nonzero terms preserve row/column order. Products preserve this property by the [Cauchy–Binet formula](../../../linear-algebra.md#cauchy-binet-formula). Insert each ordered sampling site until it has full knot multiplicity. Evaluation at such a break is one of the refined coefficients, with a consistent one-sided convention. Consequently the [B-spline collocation matrix](../../../uniform-approximation.md#b-spline-collocation-matrix) is an ordered row submatrix of the product of refinement [matrices](../../../vector-space.md#matrix), proving its nonnegative minors. This also applies to repeated admissible original knots.

Since $A$ is invertible and totally nonnegative, $\det A>0$. The [adjugate identity](../../../linear-algebra.md#adjugate-identity) gives the [checkerboard inverse of a totally nonnegative matrix](../../../vector-space.md#checkerboard-inverse-of-a-totally-nonnegative-matrix):

$$
(A^{-1})_{ij}=(-1)^{i+j}\frac{\det A_{\widehat j,\widehat i}}{\det A},
\qquad (-1)^{i+j}(A^{-1})_{ij}\geq0.
$$

Now for any [spline](../../../uniform-approximation.md#spline-mathematics) $s=\sum_j a_jN_j$, its sampled-value vector is $y=Aa$. Hence the coefficient [linear functional](../../../linear-algebra.md#linear-functional) in the [dual basis](../../../linear-algebra.md#dual-basis) is exactly

$$
\boxed{\mu_i(s)=a_i=\sum_j(A^{-1})_{ij}s(x_j^*).}
$$

In particular $\mu_i(N_\ell)=\delta_{i\ell}$, verifying the hinted formula rather than assuming it. The [operator norm](../../../continuous-dual-space.md#operator-norm) of this [linear functional](../../../linear-algebra.md#linear-functional) is taken for the [uniform norm](../../../functional-analysis.md#supremum-norm) on the [spline](../../../uniform-approximation.md#spline-mathematics)'s interval, containing all sampling sites. Evaluation at a sampling site has norm at most one, so

$$
|\mu_i(s)|\leq\left(\sum_j|(A^{-1})_{ij}|\right)\|s\|_\infty,
\qquad
\|\mu_i\|\leq\sum_j|(A^{-1})_{ij}|.
$$

For the given unit-norm alternating [spline](../../../uniform-approximation.md#spline-mathematics), $s_*(x_j^*)=(-1)^j$, and the checkerboard signs make all terms in a fixed inverse row align:

$$
a_i^*=\mu_i(s_*)=\sum_j(A^{-1})_{ij}(-1)^j
=(-1)^i\sum_j|(A^{-1})_{ij}|.
$$

Since $\|s_*\|_\infty=1$, this supplies the reverse [operator norm](../../../continuous-dual-space.md#operator-norm) inequality and proves the [Chebyshev spline coefficient and dual norm equality](../../../uniform-approximation.md#chebyshev-spline-coefficient-and-dual-norm-equality)

$$
\boxed{|a_i^*|=\|\mu_i\|=\sum_j|(A^{-1})_{ij}|,\qquad i=1,\ldots,n.}
$$

This [spline](../../../uniform-approximation.md#spline-mathematics) attains the [operator norm](../../../continuous-dual-space.md#operator-norm) of each coefficient [linear functional](../../../linear-algebra.md#linear-functional).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use the order of the three [Bernstein basis](../../../functional-analysis.md#bernstein-basis) functions given in this part. Endpoint evaluation gives

$$
a_1=p(1),\qquad a_3=p(0),
$$

so both endpoint coefficients have absolute value at most one. At the midpoint,

$$
p(1/2)=\frac14a_1+\frac12a_2+\frac14a_3,
\qquad
a_2=2p(1/2)-\frac12[p(0)+p(1)].
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) therefore gives the [quadratic Bernstein coefficient bound](../../../functional-analysis.md#quadratic-bernstein-coefficient-bound)

$$
\boxed{|a_1|\leq1,\qquad |a_2|\leq3,\qquad |a_3|\leq1.}
$$

All three bounds are sharp. Indeed $p(x)=8x^2-8x+1=T_2(2x-1)$ has [uniform norm](../../../functional-analysis.md#supremum-norm) one and coefficient vector $(1,-3,1)$ in this basis. The reversed ordering of endpoint Bernstein functions does not affect these symmetric endpoint bounds.

## 6

↑ **Parent:** [Paper 68](paper-68.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For order $k\geq2$, set $g(u)=(u-t)_+^{k-2}$. Then $(u-t)g(u)=(u-t)_+^{k-1}$. Apply the given [divided difference](../../../numerical-analysis.md#divided-difference) product identity with nodes $t_i,\ldots,t_{i+k}$ and multiply by the length $t_{i+k}-t_i$ of their knot interval:

$$
\begin{aligned}
N_{i,k}(t)
&=(t-t_i)[t_i,\ldots,t_{i+k-1}]g\\
&\quad +(t_{i+k}-t)[t_{i+1},\ldots,t_{i+k}]g.
\end{aligned}
$$

Using the definition of each lower-order normalized [B-spline](../../../uniform-approximation.md#b-spline), the two [divided differences](../../../numerical-analysis.md#divided-difference) are $N_{i,k-1}(t)/(t_{i+k-1}-t_i)$ and $N_{i+1,k-1}(t)/(t_{i+k}-t_{i+1})$. Hence the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula) is

$$
\boxed{
N_{i,k}(t)=
\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)
+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t).}
$$

For completeness, the product identity itself follows from

$$
[t_0,\ldots,t_k](u-t)g(u)
=[t_0,\ldots,t_{k-1}]g+(t_k-t)[t_0,\ldots,t_k]g
$$

and the ordinary [divided difference](../../../numerical-analysis.md#divided-difference) recurrence. Substitution yields the stated convex combination of the two order-$k-1$ [divided differences](../../../numerical-analysis.md#divided-difference).

The initial order-one [splines](../../../uniform-approximation.md#spline-mathematics) are the indicators $N_{i,1}(t)=\mathbf1_{[t_i,t_{i+1})}(t)$. For repeated knots, a term with zero knot-span denominator is defined as zero; this agrees with the standard limiting basis convention. The recurrence uses the [partition of unity](../../../differential-geometry.md#partition-of-unity) normalization with $0\leq N_{i,k}\leq1$, not a separate rescaling of each [spline](../../../uniform-approximation.md#spline-mathematics) to make its actual supremum exactly one. The original PDF recurrence has the denominators above; several of these indices and signs were corrupted in the converted TeX.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For integer knots, the recurrence simplifies to

$$
N_{i,k}(t)=\frac{t-i}{k-1}N_{i,k-1}(t)
+\frac{i+k-t}{k-1}N_{i+1,k-1}(t).
$$

Order-two [splines](../../../uniform-approximation.md#spline-mathematics) are triangular: $N_{i,2}(i)=N_{i,2}(i+2)=0$ and $N_{i,2}(i+1)=1$. Applying the recurrence once more gives

$$
\begin{array}{c|ccc}
t&1&2&3\\ \hline
N_{0,3}(t)&1/2&1/2&0\\
N_{1,3}(t)&0&1/2&1/2.
\end{array}
$$

For example $N_{0,3}(1)=\frac12N_{0,2}(1)+N_{1,2}(1)=1/2$ and $N_{0,3}(2)=N_{0,2}(2)+\frac12N_{1,2}(2)=1/2$. Thus the [Cardinal cubic B-spline](../../../uniform-approximation.md#cardinal-cubic-b-spline) values are

$$
\begin{aligned}
N_{0,4}(1)&=\frac13\frac12+\frac33\,0=\frac16,\\
N_{0,4}(2)&=\frac23\frac12+\frac23\frac12=\frac23,\\
N_{0,4}(3)&=\frac33\,0+\frac13\frac12=\frac16.
\end{aligned}
$$

Therefore

$$
\boxed{(N_{0,4}(1),N_{0,4}(2),N_{0,4}(3))=(1/6,\,2/3,\,1/6).}
$$

In particular its actual maximum is $2/3$ in this standard normalization; dividing by that maximum would change the requested recurrence normalization.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
