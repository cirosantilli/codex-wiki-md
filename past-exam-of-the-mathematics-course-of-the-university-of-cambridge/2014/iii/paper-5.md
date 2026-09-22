# Paper 5

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_5.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_5.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
    - [v](#3/a/v)
      - [Solution](#3/a/v/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)

## 1

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Taylor series](../../../calculus.md#taylor-series) definition says that $f\in C^\infty(\mathbb R)$ and, for every $a$, there is $r>0$ such that

$$
f(x)=\sum_{n=0}^\infty\frac{f^{(n)}(a)}{n!}(x-a)^n\qquad(|x-a|<r).
$$

The equivalent [factorial derivative criterion for real analyticity](../../../analysis.md#factorial-derivative-criterion-for-real-analyticity) says that, for every $a$, there are a neighborhood $I$ of $a$ and constants $C,A>0$ such that

$$
\boxed{\sup_{x\in I}|f^{(n)}(x)|\leq CA^n n!\quad(n\geq0).}
$$

The uniformity over $I$ matters: bounds only at $a$ do not exclude a [flat function](../../../analysis.md#flat-function).

Assume the [factorial derivative criterion for real analyticity](../../../analysis.md#factorial-derivative-criterion-for-real-analyticity). The [Taylor theorem with Lagrange remainder](../../../calculus.md#taylor-theorem-with-lagrange-remainder) gives

$$
\left|f(a+h)-\sum_{n=0}^{N-1}\frac{f^{(n)}(a)}{n!}h^n\right|\leq C(A|h|)^N
$$

when the segment from $a$ to $a+h$ is contained in $I$. For sufficiently small $|h|<A^{-1}$ the [Taylor remainder](../../../calculus.md#taylor-remainder) tends to zero, proving the [Taylor series](../../../calculus.md#taylor-series) definition.

Conversely, write the convergent [power series](../../../real-analysis.md#power-series) at $a$ as $\sum b_k h^k$. Choose $\rho$ strictly inside its radius of convergence; then $|b_k|\leq M\rho^{-k}$ for some $M$. Termwise [differentiation](../../../calculus.md#differentiation) on $|h|\leq\rho/2$ gives

$$
|f^{(n)}(a+h)|\leq M\rho^{-n}n!\sum_{j=0}^\infty\binom{j+n}{n}2^{-j}
=2M(2/\rho)^n n!.
$$

Here the sum is $(1-1/2)^{-n-1}$, obtained by differentiating the [geometric series](../../../real-analysis.md#geometric-series). This is the required locally uniform bound. **The two definitions of a [real analytic function](../../../analysis.md#real-analytic-function) are equivalent.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Consider the [flat function](../../../analysis.md#flat-function)

$$
f(x)=\begin{cases}e^{-1/x^2},&x\ne0,\\0,&x=0.\end{cases}
$$

Away from zero every [derivative](../../../calculus.md#derivative) has the form $P_n(1/x)e^{-1/x^2}$ for a [polynomial](../../../polynomial.md) $P_n$: differentiating preserves this form. For every $m\geq0$,

$$
\lim_{x\to0}|x|^{-m}e^{-1/x^2}=0,
$$

because an [exponential function](../../../calculus.md#exponential-function) decays faster than any power. Inductively, extend each displayed [derivative](../../../calculus.md#derivative) by zero at zero. It is continuous there, and its difference quotient at zero also tends to zero by the same estimate with one extra power of $|x|^{-1}$. Thus each extension is the [derivative](../../../calculus.md#derivative) of the preceding extension. This proves $f\in C^\infty(\mathbb R)$ and $f^{(n)}(0)=0$ for all $n$.

Its [Taylor series](../../../calculus.md#taylor-series) at zero is identically zero, whereas $f(x)>0$ for every $x\ne0$. **It is [smooth](../../../analysis.md#smooth-function) everywhere but not [real analytic](../../../analysis.md#real-analytic-function) at zero.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The complex [Liouville theorem](../../../complex-analysis.md#liouville-theorem) states that a bounded [entire function](../../../complex-analysis.md#entire-function) is constant. Indeed, if $|f|\leq M$, the [Cauchy estimate](../../../analysis.md#cauchy-estimate) on any disc of radius $R$ centered at $z$ gives $|f'(z)|\leq M/R$. Letting $R\to\infty$ gives $f'(z)=0$ everywhere.

**The analogous conclusion for bounded [real analytic functions](../../../analysis.md#real-analytic-function) on $\mathbb R$ is false.** For example, $\sin x$ is bounded, nonconstant, and [real analytic](../../../analysis.md#real-analytic-function) on the whole real line. Boundedness only on that line does not bound its [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) extension on the complex plane.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

A [separable Hilbert space](../../../hilbert-space.md#separable-hilbert-space) has a countable subset dense in its [norm topology](../../../functional-analysis.md#norm-topology).

**The printed assertion about all [locally square-integrable functions](../../../measure-theory.md#locally-square-integrable-function) is false.** The proposed average is not even finite for every such function: for $f(x)=x$,

$$
\frac1R\int_{-R}^R f(x)^2\,dx=\frac23R^2\longrightarrow\infty.
$$

It also fails positive definiteness. The nonzero function $f=\mathbf1_{[0,1]}$ has

$$
\lim_{R\to\infty}\frac1R\int_{-R}^R f(x)^2\,dx=0.
$$

Consequently this formula cannot define an [inner product](../../../linear-algebra.md#inner-product), much less a [Hilbert space](../../../hilbert-space.md), on $L^2_{\mathrm{loc}}(\mathbb R)$.

A precise version of the intended nonseparability argument uses the [mean-square completion of trigonometric polynomials](../../../hilbert-space.md#mean-square-completion-of-trigonometric-polynomials). Start with the real vector space $V$ of finite linear combinations of $1$, $\cos(\lambda x)$, and $\sin(\lambda x)$, with arbitrary $\lambda>0$. Product-to-sum identities show that all the proposed cross averages exist. Distinct frequencies are [orthogonal](../../../linear-algebra.md#orthogonal-vectors), each sine and cosine has squared [norm](../../../functional-analysis.md#norm) one, and the constant function has squared [norm](../../../functional-analysis.md#norm) two. Thus, after collecting equal frequencies,

$$
\left\|a_0+\sum_j\bigl(a_j\cos(\lambda_j x)+b_j\sin(\lambda_j x)\bigr)\right\|^2
=2a_0^2+\sum_j(a_j^2+b_j^2).
$$

This is positive definite on $V$. Its [Hilbert space completion](../../../hilbert-space.md#hilbert-space-completion) $H$ contains the uncountable [orthonormal set](../../../linear-algebra.md#orthonormal-set) $\{\cos(\lambda x):\lambda>0\}$. The distance between two distinct members is $\sqrt2$. Their open balls of radius $1/2$ are pairwise disjoint, and a dense subset must meet each one. A countable dense subset is therefore impossible: **this corrected completed space is nonseparable.** Completion is an essential additional construction; it does not validate the printed claim about all of $L^2_{\mathrm{loc}}$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [closest point theorem in a Hilbert space](../../../hilbert-space.md#hilbert-projection-theorem) says that, for every nonempty closed [convex set](../../../mathematical-optimization.md#convex-set) $C\subset H$ and $x\in H$, there is exactly one $p\in C$ minimizing $\|x-p\|$.

Put $d=\inf_{y\in C}\|x-y\|$ and choose $y_n\in C$ with $\|x-y_n\|\to d$. The midpoint belongs to $C$ because it is a [convex set](../../../mathematical-optimization.md#convex-set). The [parallelogram law](../../../linear-algebra.md#parallelogram-law) gives

$$
\|y_n-y_m\|^2
=2\|x-y_n\|^2+2\|x-y_m\|^2-4\left\|x-\frac{y_n+y_m}{2}\right\|^2
\leq2\|x-y_n\|^2+2\|x-y_m\|^2-4d^2\longrightarrow0.
$$

Thus $(y_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence). Completeness of the [Hilbert space](../../../hilbert-space.md) and closedness of $C$ give a limit $p\in C$, with $\|x-p\|=d$. Applying the same identity to two minimizers gives their squared distance at most zero, proving uniqueness.

The resulting projection is characterized by

$$
\boxed{\operatorname{Re}\langle x-p,z-p\rangle\leq0\quad(z\in C).}
$$

Indeed, differentiate $\|x-p-t(z-p)\|^2$ at $t=0^+$; the minimum there gives the inequality. Conversely, expanding $\|x-z\|^2$ proves minimality from this inequality. For a closed linear subspace, both signs of each direction are allowed, so $x-p$ is [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to that subspace: this recovers the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection).

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem) states that every bounded [linear functional](../../../linear-algebra.md#linear-functional) $L$ on a real or complex [Hilbert space](../../../hilbert-space.md) $H$ is represented by a unique $h\in H$:

$$
\boxed{L(v)=\langle v,h\rangle\quad(v\in H),\qquad\|L\|=\|h\|.}
$$

For the complex case take the [inner product](../../../linear-algebra.md#inner-product) to be linear in its first argument.

If $L=0$, choose $h=0$. Otherwise its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $K$ is a closed linear subspace. Choose $x$ with $L(x)\ne0$ and let $z=x-P_Kx$, using the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection). Then $z\ne0$, $z\perp K$, and $L(z)=L(x)\ne0$. For every $v$,

$$
v-\frac{L(v)}{L(z)}z\in K,
\qquad
\langle v,z\rangle=\frac{L(v)}{L(z)}\|z\|^2.
$$

Therefore take $h=L(z)z/\|z\|^2$ in the real case, and $h=\overline{L(z)}z/\|z\|^2$ in the complex case. The conjugate in the latter formula compensates for conjugate linearity in the second argument.

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $|L(v)|\leq\|v\|\|h\|$, and evaluation at $v=h/\|h\|$ when $h\ne0$ gives equality of the [norms](../../../functional-analysis.md#norm). If two vectors represent $L$, their difference is [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to every vector, including itself, hence zero. This proves all assertions of the [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem).

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The real [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) applies to a [Hilbert space](../../../hilbert-space.md) $H$ and a [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form) $a$ satisfying

$$
|a(u,v)|\leq M\|u\|\|v\|,\qquad a(v,v)\geq\alpha\|v\|^2\quad(\alpha>0).
$$

For every bounded [linear functional](../../../linear-algebra.md#linear-functional) $L$ there is a unique $u\in H$ with

$$
\boxed{a(u,v)=L(v)\quad(v\in H),\qquad\|u\|\leq\alpha^{-1}\|L\|.}
$$

Symmetry of the [bilinear form](../../../linear-algebra.md#bilinear-form) is not required.

By the [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem), write $a(u,v)=\langle Au,v\rangle$ and $L(v)=\langle g,v\rangle$. The operator $A$ is linear and bounded, with $\|A\|\leq M$. The [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form) bound and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) imply

$$
\alpha\|u\|^2\leq\langle Au,u\rangle\leq\|Au\|\|u\|,
\qquad\|Au\|\geq\alpha\|u\|.
$$

Hence $A$ is injective. Its range is closed: if $Au_n$ converges, this last inequality applied to differences makes $u_n$ a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence), and its limit maps to the proposed range limit. If $w$ is in the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of the range, then $a(u,w)=0$ for all $u$; taking $u=w$ and using coercivity gives $w=0$. The range is thus dense as well as closed, so it is all of $H$. Solve $Au=g$ uniquely; the displayed lower bound gives the asserted estimate.

For complex [Hilbert spaces](../../../hilbert-space.md) the same proof works for a bounded [sesquilinear form](../../../linear-algebra.md#sesquilinear-form), linear in the first argument, with $\operatorname{Re}a(v,v)\geq\alpha\|v\|^2$. In the convention $a(u,v)=L(v)$, $L$ must then be a bounded conjugate-linear functional represented as $\langle g,v\rangle$.

## 2

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The total differential order of $\partial_t-\partial_x^2$ is two, so its [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) is $p(\tau,\xi)=-\xi^2$. The conormal to $t=0$ is $(1,0)$, on which $p$ vanishes. **The initial line is a [characteristic hypersurface](../../../partial-differential-equation.md#characteristic-hypersurface)** for this total-order symbol; the first-order time derivative does not enter it.

Suppose a [real analytic](../../../analysis.md#real-analytic-function) solution existed near $(0,0)$. Repeated use of the [heat equation](../../../diffusion-equation.md#heat-equation) gives $\partial_t^k u=\partial_x^{2k}u$. The initial [power series](../../../real-analysis.md#power-series) is $\sum_{j\geq0}(-1)^j x^{2j}$ near zero, hence

$$
\partial_t^k u(0,0)=(-1)^k(2k)!.
$$

The time [Taylor series](../../../calculus.md#taylor-series) at $x=0$ would therefore have coefficients $(-1)^k(2k)!/k!$. The ratio of successive absolute coefficients is $2(2k+1)\to\infty$, giving radius of convergence zero. This contradicts the assumed [real analytic](../../../analysis.md#real-analytic-function) regularity. **No such analytic local solution exists**, although the initial function itself is [real analytic](../../../analysis.md#real-analytic-function).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a defining function $\phi$ with $d\phi\ne0$, the [characteristic hypersurface](../../../partial-differential-equation.md#characteristic-hypersurface) test is that the [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) vanish at $d\phi$.

For the [wave equation](../../../wave-equation.md) with speed $c>0$,

$$
u_{tt}-c^2\Delta_xu=0,\qquad p(\tau,\xi)=\tau^2-c^2|\xi|^2.
$$

Thus its [characteristic hypersurfaces](../../../partial-differential-equation.md#characteristic-hypersurface) satisfy $\phi_t^2=c^2|\nabla_x\phi|^2$. In one space dimension the two families are $x\pm ct=\text{constant}$; cones are characteristic away from their vertices.

For the [free Schrodinger equation](../../../physics.md#free-schrodinger-equation), in normalized units,

$$
i u_t+\Delta_xu=0,\qquad p(\tau,\xi)=|\xi|^2.
$$

Its total-order [characteristic hypersurfaces](../../../partial-differential-equation.md#characteristic-hypersurface) satisfy $\nabla_x\phi=0$. Their normal is purely temporal, so locally they are constant-time hypersurfaces. Multiplying the equation by a nonzero constant or choosing the opposite sign convention does not change this test.

For the [Laplace equation](../../../partial-differential-equation.md#laplace-equation),

$$
\Delta_xu=0,\qquad p(\xi)=|\xi|^2.
$$

**There are no real [characteristic hypersurfaces](../../../partial-differential-equation.md#characteristic-hypersurface) for the [Laplace equation](../../../partial-differential-equation.md#laplace-equation)**, since their normal cannot be zero. These statements concern the ordinary total-order [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation), not a weighted space-time grading.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The interior [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) assertion for the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) is that a [harmonic function](../../../partial-differential-equation.md#harmonic-function) is [smooth](../../../analysis.md#smooth-function), in fact [real analytic](../../../analysis.md#real-analytic-function), throughout $U$. No boundary regularity of its unspecified boundary values is implied.

First let $u\in C^2(U)$ and $\Delta u=0$. On a ball compactly contained in $U$, differentiating its spherical average and applying the [divergence theorem](../../../calculus.md#divergence-theorem) expresses that derivative as a constant factor times $\int_{B_r}\Delta u$, which is zero. The spherical average tends to $u$ at the center as $r\to0$. This proves the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions).

Choose a radially symmetric [smooth](../../../analysis.md#smooth-function) [mollifier](../../../distribution-theory.md#mollifier) $\eta_r$, supported in $B_r$, with integral one. By integrating the spherical [mean value property](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions),

$$
u(x)=\int\eta_r(x-y)u(y)\,dy
$$

whenever $B_r(x)\Subset U$. For fixed $r$ the right side is a [smooth](../../../analysis.md#smooth-function) [convolution](../../../fourier-analysis.md#convolution), since all [derivatives](../../../calculus.md#derivative) can be placed on $\eta_r$. Thus $u$ is [smooth](../../../analysis.md#smooth-function). The same argument proves the [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma) for a distributionally [harmonic](../../../partial-differential-equation.md#harmonic-function) $u\in L^1_{\mathrm{loc}}$: first mollify $u$, apply the fixed-radius identity, and let the mollification radius tend to zero in distributions to obtain the same smooth representative.

To prove [real analytic](../../../analysis.md#real-analytic-function) regularity, differentiating the fixed-radius [convolution](../../../fourier-analysis.md#convolution) gives the [interior derivative estimate for a harmonic function](../../../partial-differential-equation.md#interior-derivative-estimate-for-a-harmonic-function)

$$
|\partial_j v(x)|\leq\frac{C_\ell}{r}\sup_{B_r(x)}|v|
$$

for any [harmonic](../../../partial-differential-equation.md#harmonic-function) $v$. All [derivatives](../../../calculus.md#derivative) of $u$ are [harmonic](../../../partial-differential-equation.md#harmonic-function). On nested balls between $B_R(a)$ and $B_{R/2}(a)$, apply this estimate $k$ times, decreasing the radius by $R/(2k)$ each time. For $|\alpha|=k$,

$$
\sup_{B_{R/2}(a)}|D^\alpha u|\leq\left(\frac{Ck}{R}\right)^k\sup_{B_R(a)}|u|
\leq\left(\frac{Ce}{R}\right)^k k!\sup_{B_R(a)}|u|.
$$

The inequality $k^k\leq e^k k!$ follows by integrating $\log s$ below the sum defining $\log(k!)$. Apply the one-dimensional [Taylor theorem](../../../calculus.md#taylor-theorem) along each segment, expanding directional [derivatives](../../../calculus.md#derivative) by the multinomial formula. The remainder is bounded by $M(A\sum_j|h_j|)^k$, so it tends to zero for sufficiently small $h$. This gives a locally convergent multivariate [Taylor series](../../../calculus.md#taylor-series). **A [harmonic function](../../../partial-differential-equation.md#harmonic-function) is [real analytic](../../../analysis.md#real-analytic-function) in the interior.**

The usual inhomogeneous [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) statement also follows: if $\Delta u=f$ and $f$ is [smooth](../../../analysis.md#smooth-function), take a cutoff $\chi$ equal to one near a given point and set $w=\Phi*(\chi f)$, where $\Phi$ is a [fundamental solution of the Laplace equation](../../../partial-differential-equation.md#fundamental-solution-of-the-laplace-equation) with $\Delta\Phi=\delta$. Moving every [derivative](../../../calculus.md#derivative) to the compactly supported [smooth](../../../analysis.md#smooth-function) function $\chi f$ shows $w$ is [smooth](../../../analysis.md#smooth-function). Locally $u-w$ is [harmonic](../../../partial-differential-equation.md#harmonic-function), so $u$ is [smooth](../../../analysis.md#smooth-function) there too.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Cauchy problem for a partial differential equation](../../../partial-differential-equation.md#cauchy-problem) here prescribes both the value $u|_\Gamma=g$ and the [normal derivative](../../../differential-geometry.md#normal-derivative) $\partial_nu|_\Gamma=h$, together with $\Delta u=0$. Only one of these traces would be boundary data for a usual elliptic boundary problem, rather than full [Cauchy data](../../../partial-differential-equation.md#cauchy-data).

Every real hypersurface is a [non-characteristic hypersurface](../../../partial-differential-equation.md#non-characteristic-hypersurface) for the [Laplace equation](../../../partial-differential-equation.md#laplace-equation). In local [real analytic](../../../analysis.md#real-analytic-function) coordinates flattening the [real analytic](../../../analysis.md#real-analytic-function) hypersurface $\Gamma$, the coefficient of the second transverse derivative is nonzero: its principal coefficient is the squared length of the conormal. The equation can therefore be solved for that second derivative. The [normal derivative](../../../differential-geometry.md#normal-derivative) data determine the transverse first derivative, because the coefficient relating them is nonzero and the tangential first derivatives are already determined by $g$.

The coefficients, flattened [Cauchy data](../../../partial-differential-equation.md#cauchy-data), and coordinate change are all [real analytic](../../../analysis.md#real-analytic-function). **The [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) applies**, giving a unique local [real analytic](../../../analysis.md#real-analytic-function) solution around each point of $\Gamma$. This is a local existence assertion, not a claim of stable dependence in arbitrary [Sobolev space](../../../sobolev-space.md) norms.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**The [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) cannot be applied to merely $C^2$, non-$C^3$ [Cauchy data](../../../partial-differential-equation.md#cauchy-data).** It requires [real analytic](../../../analysis.md#real-analytic-function) data.

There is also no $C^2$ solution of the [Laplace equation](../../../partial-differential-equation.md#laplace-equation) on a neighborhood of a point where one of these prescribed traces fails to be $C^3$. By interior [elliptic regularity](../../../distribution-theory.md#elliptic-regularity), any such solution would be [smooth](../../../analysis.md#smooth-function) and [real analytic](../../../analysis.md#real-analytic-function). On the [real analytic](../../../analysis.md#real-analytic-function) hypersurface retained from the preceding part, both its restriction and its [normal derivative](../../../differential-geometry.md#normal-derivative) would then be [real analytic](../../../analysis.md#real-analytic-function), hence $C^3$. This contradicts the prescribed trace. **There is no solution on a neighborhood of all of $\Gamma$ with the stated non-$C^3$ data.** This does not exclude solutions near other points where the data happen to be [real analytic](../../../analysis.md#real-analytic-function).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Use unit speed and write the [Cauchy data](../../../partial-differential-equation.md#cauchy-data) as $u(0)=f$, $u_t(0)=g$. For finite-energy data define the [wave energy estimate](../../../partial-differential-equation.md#wave-energy-estimate) quantity

$$
E(t)=\frac12\int_{\mathbb R^n}\bigl(u_t^2+|\nabla_xu|^2\bigr)\,dx.
$$

Multiply $u_{tt}-\Delta_xu=0$ by $u_t$ and use [integration by parts](../../../calculus.md#integration-by-parts). With compact support or sufficient decay the boundary flux is zero, so

$$
E'(t)=\int u_t(u_{tt}-\Delta_xu)\,dx=0,
\qquad
\boxed{\|u_t(t)\|_2^2+\|\nabla_xu(t)\|_2^2=\|g\|_2^2+\|\nabla f\|_2^2.}
$$

For general finite-energy solutions, cutoff or approximation arguments justify this identity; equivalently the local estimate below, applied in both time directions and with radii tending to infinity, gives the same equality. Arbitrary [smooth](../../../analysis.md#smooth-function) data need not have finite global energy; then the global bound with an infinite right side is uninformative, while the local estimate remains useful.

If $f\in H^1$ and $g\in L^2$, the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and the [wave energy estimate](../../../partial-differential-equation.md#wave-energy-estimate) further give

$$
\|u(t)\|_2\leq\|f\|_2+|t|\sqrt{\|g\|_2^2+\|\nabla f\|_2^2}.
$$

Together these yield an a priori bound for $\|u(t)\|_{H^1}+\|u_t(t)\|_2$ on each bounded time interval. No existence assumption is proved by the estimate itself; it controls any sufficiently regular solution.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

The [local wave energy estimate](../../../partial-differential-equation.md#local-wave-energy-estimate) is, for $T\geq0$, $r>0$, and any center $x_0$,

$$
\boxed{\int_{B_r(x_0)}(u_t^2+|\nabla u|^2)(T,x)\,dx
\leq\int_{B_{r+T}(x_0)}(g^2+|\nabla f|^2)(x)\,dx.}
$$

To prove it, let $R=r+T$ and integrate the local [energy estimate](../../../partial-differential-equation.md#energy-estimate) identity $\partial_t e=\operatorname{div}(u_t\nabla u)$, where $e=(u_t^2+|\nabla u|^2)/2$, over the shrinking ball $B_{R-t}(x_0)$. Differentiation of this moving-domain integral yields

$$
\frac{d}{dt}\int_{B_{R-t}}e
=\int_{\partial B_{R-t}}\left(u_t\partial_nu-\frac12u_t^2-\frac12|\nabla u|^2\right)\,dS
=-\frac12\int_{\partial B_{R-t}}\left((u_t-\partial_nu)^2+|\nabla_{\mathrm{tan}}u|^2\right)\,dS\leq0.
$$

Integrating in time proves the [local wave energy estimate](../../../partial-differential-equation.md#local-wave-energy-estimate), without assumptions at spatial infinity.

Let the union of the initial [supports](../../../function.md#support) be a compact set $K$. If $\operatorname{dist}(x_0,K)>T$, choose $r>0$ with $r+T<\operatorname{dist}(x_0,K)$. The initial energy on $B_{r+T}(x_0)$ vanishes. Applying the shrinking-ball identity up to every intermediate time shows $u_t$ and $\nabla u$ vanish throughout that cone. In particular, along the vertical segment through $x_0$, $u_t=0$; its initial value is also zero, so $u(T,x_0)=0$. This last value check removes the constant ambiguity invisible to gradient energy.

Consequently the [finite propagation speed](../../../wave-equation.md#finite-propagation-speed) conclusion is

$$
\boxed{\operatorname{supp}u(t,\cdot)\subseteq\{x:\operatorname{dist}(x,K)\leq|t|\}.}
$$

This set is compact for each finite $t$. The speed is at most one in these units, or $c$ for $u_{tt}-c^2\Delta u=0$. Time reversal gives the same conclusion for negative time.

## 3

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

For this [Neumann Poisson problem](../../../partial-differential-equation.md#neumann-poisson-problem), interpret the forcing in $L^2(U)$, as is automatic if it is [smooth](../../../analysis.md#smooth-function) up to the boundary. Literal interior smoothness alone does not ensure the integrals or bounded functionals required in this question: for example, $f(x)=x^{-2}$ on $(0,1)$ is interior [smooth](../../../analysis.md#smooth-function) but even $\int f\cdot1$ diverges. Classical regularity in the converse is likewise understood up to the boundary.

Suppose the [weak solution](../../../partial-differential-equation.md#weak-solution) is [smooth](../../../analysis.md#smooth-function) on $\overline U$. Testing against compactly supported [test functions](../../../distribution-theory.md#test-function) gives $-\Delta u=f$ in distributions and hence pointwise. Now the weak identity and [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) imply

$$
0=\int_U\nabla u\cdot\nabla v-\int_Ufv=\int_{\partial U}(\partial_nu)v\,dS
$$

for every [smooth](../../../analysis.md#smooth-function) $v$ on $\overline U$. Every [smooth](../../../analysis.md#smooth-function) boundary function has such an extension, so $\partial_nu=0$ on $\partial U$. This proves both the interior equation and the boundary condition.

Conversely, for $u\in C^2(\overline U)$ satisfying the equation and zero [normal derivative](../../../differential-geometry.md#normal-derivative), [Green's first identity](../../../partial-differential-equation.md#green-s-first-identity) gives the weak identity for all [smooth](../../../analysis.md#smooth-function) $v$ on $\overline U$. The [density of smooth functions in a Sobolev space](../../../sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) extend it continuously to every $v\in H^1(U)$. Thus **the classical solution is a [weak solution](../../../partial-differential-equation.md#weak-solution)**, and the smooth [weak solution](../../../partial-differential-equation.md#weak-solution) is classical.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Subtract the two [weak solution](../../../partial-differential-equation.md#weak-solution) identities and test with their difference $w\in H^1(U)$. Then

$$
\int_U|\nabla w|^2=0.
$$

A [Sobolev function with zero weak gradient](../../../sobolev-space.md#sobolev-function-with-zero-weak-gradient) is constant on each connected component. One justification is to mollify locally: each mollification has zero gradient and is constant on its ball, and overlaps identify the constants; taking limits gives the original assertion. Since $U$ is connected, $w$ is one constant on $U$.

Conversely, adding a constant changes neither the [weak derivative](../../../distribution-theory.md#weak-derivative) nor the weak identity. **The solution is unique up to an additive constant.**

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

There is a normalization error in the PDF. With the printed unnormalized integral, testing a constant function equal to one would give a left side $|U|(1-|U|)^2$ and a right side zero. Thus that formulation fails whenever $|U|\ne1$.

Use instead the average $v_U=|U|^{-1}\int_Uv$. The [Poincare-Wirtinger inequality](../../../sobolev-space.md#poincare-wirtinger-inequality), also called the [Neumann-Poincare inequality](../../../sobolev-space.md#poincare-wirtinger-inequality), is

$$
\boxed{\|v-v_U\|_{L^2(U)}^2\leq C_P\|\nabla v\|_{L^2(U)}^2.}
$$

If no $C_P$ exists, subtract the average and normalize a violating sequence to obtain $w_j\in H^1(U)$ with $\int_Uw_j=0$, $\|w_j\|_2=1$, and $\|\nabla w_j\|_2\to0$. This sequence is bounded in the [Sobolev space](../../../sobolev-space.md) $H^1(U)$. The [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) supplies a subsequence converging strongly in $L^2(U)$ to $w$.

For every compactly supported [test function](../../../distribution-theory.md#test-function) $\varphi$, [integration by parts](../../../calculus.md#integration-by-parts) and these convergences give $\int w\partial_i\varphi=0$. Thus $w$ has zero [weak gradient](../../../distribution-theory.md#weak-gradient). The [Sobolev function with zero weak gradient](../../../sobolev-space.md#sobolev-function-with-zero-weak-gradient) result and connectedness make $w$ constant. Strong $L^2$ convergence preserves its zero integral, so $w=0$. It also preserves its [norm](../../../functional-analysis.md#norm) one, a contradiction. This proves the correctly normalized [Neumann-Poincare inequality](../../../sobolev-space.md#poincare-wirtinger-inequality).

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/a/iv)

Work in the [mean-zero Sobolev space](../../../sobolev-space.md#mean-zero-sobolev-space)

$$
H=\left\{v\in H^1(U):\int_Uv=0\right\},\qquad a(u,v)=\int_U\nabla u\cdot\nabla v.
$$

The integral is a continuous functional on $H^1(U)$, so $H$ is closed. The [Neumann-Poincare inequality](../../../sobolev-space.md#poincare-wirtinger-inequality) shows that $\|v\|_a=\|\nabla v\|_2$ is equivalent to the usual $H^1$ [norm](../../../functional-analysis.md#norm) on $H$, making $a$ a complete [inner product](../../../linear-algebra.md#inner-product) there.

For $f\in L^2(U)$ the functional $L(v)=\int_Ufv$ satisfies

$$
|L(v)|\leq\|f\|_2\|v\|_2\leq\sqrt{C_P}\|f\|_2\|v\|_a.
$$

The [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem), or the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem), gives a unique $u\in H$ with $a(u,v)=L(v)$ for all $v\in H$. To recover every $H^1(U)$ test, write $v=(v-v_U)+v_U$. The constant contributes zero to $a$ and contributes $v_U\int_Uf=0$ to $L$. Thus the same equality holds for all $v\in H^1(U)$.

**A [weak solution](../../../partial-differential-equation.md#weak-solution) exists whenever $\int_Uf=0$; fixing its average to zero makes it unique.** Moreover $\|\nabla u\|_2\leq\sqrt{C_P}\|f\|_2$ and the [Neumann-Poincare inequality](../../../sobolev-space.md#poincare-wirtinger-inequality) also controls $\|u\|_2$.

<h4 id="3/a/v">v</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/v/solution">Solution</h5>

↑ **Parent:** [V](#3/a/v)

The constant function $v=1$ is an admissible $H^1(U)$ test for the [Neumann Poisson problem](../../../partial-differential-equation.md#neumann-poisson-problem). Its [weak gradient](../../../distribution-theory.md#weak-gradient) is zero, so the weak identity immediately gives

$$
\boxed{\int_Uf\,dx=0.}
$$

This is necessary, and the preceding Hilbert-space construction proves sufficiency for $f\in L^2(U)$. It is the balance condition corresponding to zero total boundary flux.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The [clamped second-order Sobolev space](../../../sobolev-space.md#clamped-second-order-sobolev-space) is $H_0^2(U)=\overline{C_c^\infty(U)}^{H^2}$. On a smooth bounded domain the [Sobolev trace theorem](../../../sobolev-space.md#sobolev-trace-theorem) characterizes it by zero value and zero [normal derivative](../../../differential-geometry.md#normal-derivative) on the boundary. In particular, its whole first-order boundary jet is zero, since tangential derivatives of the zero trace also vanish. As above, assume $f\in L^2(U)$ and classical regularity up to the boundary.

For a [smooth](../../../analysis.md#smooth-function) [weak solution](../../../partial-differential-equation.md#weak-solution), compactly supported [test functions](../../../distribution-theory.md#test-function) and two [integrations by parts](../../../calculus.md#integration-by-parts) give

$$
\int_U(\Delta^2u-f)v=0\quad(v\in C_c^\infty(U)),
$$

so $\Delta^2u=f$ pointwise. Membership in $H_0^2(U)$ supplies $u=\partial_nu=0$ on $\partial U$. Thus it is a classical solution of the [clamped biharmonic problem](../../../calculus.md#clamped-biharmonic-problem).

Conversely, a $C^4(\overline U)$ classical solution with these traces belongs to $H_0^2(U)$. For every compactly supported [test function](../../../distribution-theory.md#test-function), two [integrations by parts](../../../calculus.md#integration-by-parts) give $\int_U\Delta u\Delta v=\int_Ufv$. Both sides are continuous for the $H^2$ [norm](../../../functional-analysis.md#norm), so the defining density of $C_c^\infty(U)$ in $H_0^2(U)$ extends this equality to every required test. **The two notions agree under the stated smoothness.**

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The difference $w$ of two [weak solutions](../../../partial-differential-equation.md#weak-solution) lies in the [clamped second-order Sobolev space](../../../sobolev-space.md#clamped-second-order-sobolev-space). Testing with $w$ yields $\int_U(\Delta w)^2=0$, so $\Delta w=0$. Since $w\in H_0^1(U)$, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\|\nabla w\|_2^2=-\int_Uw\Delta w=0.
$$

The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) for zero boundary values now implies $\|w\|_2=0$. **The [clamped biharmonic problem](../../../calculus.md#clamped-biharmonic-problem) has at most one [weak solution](../../../partial-differential-equation.md#weak-solution).** Unlike the [Neumann Poisson problem](../../../partial-differential-equation.md#neumann-poisson-problem), no additive constant is allowed by these boundary traces.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

For $v\in C_c^\infty(U)$, two [integrations by parts](../../../calculus.md#integration-by-parts) give the [clamped Hessian identity](../../../sobolev-space.md#clamped-hessian-identity)

$$
\sum_{i,j}\int_U(\partial_{ij}v)^2=\sum_{i,j}\int_U(\partial_{ii}v)(\partial_{jj}v)=\int_U(\Delta v)^2.
$$

By density it remains valid on $H_0^2(U)$. Each $\partial_i v$ has zero integral, first for compactly supported [test functions](../../../distribution-theory.md#test-function) and then by $H^2$ convergence. Applying the [Neumann-Poincare inequality](../../../sobolev-space.md#poincare-wirtinger-inequality) to each $\partial_i v$ gives

$$
\|\nabla v\|_2^2\leq C_P\sum_{i,j}\|\partial_{ij}v\|_2^2=C_P\|\Delta v\|_2^2.
$$

The zero-boundary [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) also gives $\|v\|_2^2\leq C_D\|\nabla v\|_2^2$. Hence, using a full-Hessian equivalent $H^2$ [norm](../../../functional-analysis.md#norm),

$$
\boxed{\|v\|_{H^2}^2\leq\bigl(1+C_P+C_DC_P\bigr)\|\Delta v\|_2^2\quad(v\in H_0^2(U)).}
$$

Thus $a(u,v)=\int_U\Delta u\Delta v$ is an [inner product](../../../linear-algebra.md#inner-product) whose [norm](../../../functional-analysis.md#norm) is equivalent to the complete $H^2$ [norm](../../../functional-analysis.md#norm) on the [clamped second-order Sobolev space](../../../sobolev-space.md#clamped-second-order-sobolev-space). The functional $L(v)=\int_Ufv$ is bounded for this [norm](../../../functional-analysis.md#norm) by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the displayed bound. Apply the [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem), or the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem), to get a unique $u\in H_0^2(U)$ representing $L$. **The [clamped biharmonic problem](../../../calculus.md#clamped-biharmonic-problem) has a unique [weak solution](../../../partial-differential-equation.md#weak-solution) for every $f\in L^2(U)$**, with $\|u\|_{H^2}\leq C\|f\|_2$ and no zero-integral compatibility condition.

## 4

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Let $M=\|F'\|_\infty$. The sharper [energy estimate](../../../partial-differential-equation.md#energy-estimate) uses the divergence structure of the [viscous scalar conservation law](../../../partial-differential-equation.md#viscous-scalar-conservation-law). Multiply by $u$ and integrate over the line. With $G(s)=\int_0^s rF'(r)\,dr$,

$$
\int u\partial_xF(u)=\int\partial_xG(u)=0,
$$

because the decay makes $G(u)$ tend to zero at both ends. [Integration by parts](../../../calculus.md#integration-by-parts) in the diffusion term therefore gives

$$
\frac12\frac{d}{dt}\|u(t)\|_2^2+\varepsilon\|u_x(t)\|_2^2=0,
\qquad
\boxed{\|u(t)\|_2^2+2\varepsilon\int_0^t\|u_x(s)\|_2^2\,ds=\|u(0)\|_2^2.}
$$

**One may take $C_0=0$, uniformly in $\varepsilon$.** This does not require $F(0)=0$.

If a bound explicitly involving $M$ and $\varepsilon$ is desired, retaining the transport term and using the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the elementary inequality $ab\leq(a^2+b^2)/2$ gives

$$
M\|u\|_2\|u_x\|_2\leq\frac\varepsilon2\|u_x\|_2^2+\frac{M^2}{2\varepsilon}\|u\|_2^2.
$$

The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) then gives the valid but weaker choice $C_0=M^2/\varepsilon$. The exact cancellation explains why its divergence is unnecessary.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Multiply the [viscous scalar conservation law](../../../partial-differential-equation.md#viscous-scalar-conservation-law) by $-u_{xx}$, rather than estimating $F''$ after differentiating. [Integration by parts](../../../calculus.md#integration-by-parts) yields

$$
\frac12\frac{d}{dt}\|u_x\|_2^2+\varepsilon\|u_{xx}\|_2^2
=\int F'(u)u_xu_{xx}
\leq M\|u_x\|_2\|u_{xx}\|_2
\leq\frac\varepsilon2\|u_{xx}\|_2^2+\frac{M^2}{2\varepsilon}\|u_x\|_2^2.
$$

Thus $d\|u_x\|_2^2/dt\leq(M^2/\varepsilon)\|u_x\|_2^2$. Applying the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives

$$
\boxed{\|u_x(t)\|_2^2\leq e^{M^2t/\varepsilon}\|u_x(0)\|_2^2,\qquad C_1=M^2/\varepsilon.}
$$

Only the assumed bound on $F'$ is used; a global bound on $F''$ is not needed for this [energy estimate](../../../partial-differential-equation.md#energy-estimate).

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

For the sharp [energy estimate](../../../partial-differential-equation.md#energy-estimate), **$C_0=0$ stays uniform while the available bound $C_1=M^2/\varepsilon$ diverges as $\varepsilon\downarrow0$ when $M>0$.** If the coarser estimate is used for the first part, both displayed bounds $M^2/\varepsilon$ diverge, but the first divergence is only an artifact of discarding an exact cancellation.

The [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) explains why uniform control of the [gradient](../../../calculus.md#gradient) cannot generally persist for the inviscid [scalar conservation law](../../../partial-differential-equation.md#scalar-conservation-law). Before [characteristic crossing](../../../partial-differential-equation.md#characteristic-crossing), with initial data $u_0$,

$$
x=\xi+tF'(u_0(\xi)),\qquad u(t,x)=u_0(\xi),\qquad
u_x(t,x)=\frac{u_0'(\xi)}{1+tF''(u_0(\xi))u_0'(\xi)}.
$$

If $F''(u_0(\xi))u_0'(\xi)<0$ somewhere, the denominator reaches zero in finite positive time. The solution steepens and the smooth description breaks down; an [entropy solution](../../../partial-differential-equation.md#entropy-solution) can subsequently contain [shocks](../../../partial-differential-equation.md#shock-wave). Positive viscosity replaces such a discontinuity by a thin smooth layer, which can have large [gradient](../../../calculus.md#gradient) even while its $L^2$ [norm](../../../functional-analysis.md#norm) remains controlled. The divergent bound does not assert that every flux and every initial datum form a [shock](../../../partial-differential-equation.md#shock-wave); a linear flux, for example, has no such steepening.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Insert the [travelling wave](../../../analysis.md#travelling-wave) into the [viscous scalar conservation law](../../../partial-differential-equation.md#viscous-scalar-conservation-law). With $s=x-\sigma t$ the equation becomes

$$
-\sigma v'+F'(v)v'=\varepsilon v'',
$$

and one integration gives

$$
\varepsilon v'=F(v)-\sigma v+b=:Q(v).
$$

For a nonconstant profile, $Q(v(s))$ never vanishes. Indeed, the autonomous [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) $v'=Q(v)/\varepsilon$ has unique local solutions since $Q$ is $C^1$; reaching an equilibrium would force the whole solution to be constant. Separation and $c=v(0)$ therefore give

$$
\boxed{s=\int_c^{v(s)}\frac{\varepsilon}{F(z)-\sigma z+b}\,dz.}
$$

A different choice of reference point gives $s-s_0$ on the left, expressing the translation freedom of the [travelling wave](../../../analysis.md#travelling-wave).

**The printed formula needs a nonconstant-profile qualification.** Constant profiles also solve the PDE, but their denominator vanishes at their constant value, so the separated integral is not defined. They must be included separately as equilibrium solutions of the integrated [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation).

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

The integrated [travelling wave](../../../analysis.md#travelling-wave) equation is $v'=Q(v)/\varepsilon$. A finite limiting value $a$ at either end must satisfy $Q(a)=0$. Otherwise continuity of $Q$ makes $v'$ eventually have a fixed sign and an absolute value bounded below, which is incompatible with convergence to $a$. Therefore

$$
F(u_l)-\sigma u_l+b=0,\qquad F(u_r)-\sigma u_r+b=0.
$$

Subtracting yields the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions)

$$
\sigma(u_l-u_r)=F(u_l)-F(u_r).
$$

For distinct end states this gives

$$
\boxed{\sigma=\frac{F(u_l)-F(u_r)}{u_l-u_r}.}
$$

**Distinctness is needed for the printed quotient.** If $u_l=u_r$, the identity is $0=0$. A nonconstant global profile is strictly monotone by the scalar [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation), so cannot have equal finite end states. The equal-state profiles here are constant and their representation allows any $\sigma$.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Fix $u_l>u_r$ and the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions) speed from the preceding part. The new hypothesis is a [uniformly convex scalar flux](../../../partial-differential-equation.md#uniformly-convex-scalar-flux), $F''\geq\kappa>0$; it replaces the globally bounded-$F'$ hypothesis of part (a). Choose $b=\sigma u_r-F(u_r)$. Then

$$
Q(z)=F(z)-\bigl(F(u_r)+\sigma(z-u_r)\bigr)<0\quad(u_r<z<u_l),
$$

since a strictly [convex function](../../../real-analysis.md#convex-function) lies below the chord between its two endpoint values. Also $Q(u_l)=Q(u_r)=0$ and

$$
F'(u_r)<\sigma<F'(u_l).
$$

The zeros at the endpoints are simple, so the separated integral diverges logarithmically there. Thus the [travelling wave](../../../analysis.md#travelling-wave) is a decreasing connection defined for all $s$, unique up to translation.

To specify a limit, fix a number $c\in(u_r,u_l)$ independently of $\varepsilon$ and normalize $v_\varepsilon(0)=c$. If $V'=Q(V)$ and $V(0)=c$, uniqueness gives $v_\varepsilon(s)=V(s/\varepsilon)$. Consequently

$$
\boxed{u_\varepsilon(t,x)\longrightarrow
\begin{cases}u_l,&x<\sigma t,\\u_r,&x>\sigma t.\end{cases}}
$$

At $x=\sigma t$ the normalized profile equals $c$ for every $\varepsilon$. This single-line value is immaterial to the [weak solution](../../../partial-differential-equation.md#weak-solution). Convergence holds pointwise off the line and in $L^1_{\mathrm{loc}}$ by bounded convergence; it cannot be uniform across a nonzero jump. The transition has thickness of order $\varepsilon$.

This is the [vanishing viscosity approximation](../../../partial-differential-equation.md#vanishing-viscosity-approximation) to a compressive [entropy shock](../../../partial-differential-equation.md#entropy-shock). The [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions) makes the step a [weak solution](../../../partial-differential-equation.md#weak-solution) of the inviscid [scalar conservation law](../../../partial-differential-equation.md#scalar-conservation-law), while $F'(u_r)<\sigma<F'(u_l)$ means [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) enter the shock from both sides. For every [smooth](../../../analysis.md#smooth-function) [convex function](../../../real-analysis.md#convex-function) $\eta$ used as an entropy, with [entropy flux for a scalar conservation law](../../../partial-differential-equation.md#entropy-flux-for-a-scalar-conservation-law) $q'=\eta'F'$, the viscous equation gives

$$
\partial_t\eta(u)+\partial_xq(u)
=\varepsilon\partial_{xx}\eta(u)-\varepsilon\eta''(u)u_x^2
\leq\varepsilon\partial_{xx}\eta(u).
$$

Against compactly supported tests the right side tends to zero, since $u_\varepsilon$ stays in $[u_r,u_l]$. Passing to the $L^1_{\mathrm{loc}}$ limit yields the entropy inequality, explaining the direction selected by positive viscosity.

**A translation must be fixed to obtain this particular limit.** An $\varepsilon$-dependent translate $V((s-a_\varepsilon)/\varepsilon)$ can converge to a shock at a different location, to a constant if its center escapes, or fail to converge if the centers oscillate. Thus existence of profiles alone does not specify a single vanishing-viscosity limit without a phase normalization.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
