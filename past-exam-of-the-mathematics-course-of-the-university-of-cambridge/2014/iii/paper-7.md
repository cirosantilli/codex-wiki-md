# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_7.pdf)

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
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [characteristic equations for a transport equation](../../../partial-differential-equation.md#characteristic-equations-for-a-transport-equation) are $\dot X=V$ and $\dot V=X$, so $\ddot X=X$. For an initial point $(x_0,v_0)$ their solution is

$$
 \binom{X(t)}{V(t)}=A_t\binom{x_0}{v_0},\qquad
 A_t=\begin{pmatrix}\cosh t&\sinh t\\\sinh t&\cosh t\end{pmatrix}.
$$

This is the [hyperbolic characteristic flow for an inverted oscillator](../../../statistical-physics.md#hyperbolic-characteristic-flow-for-an-inverted-oscillator). The addition formulas give $A_sA_t=A_{s+t}$ and $A_t^{-1}=A_{-t}$. In particular, the backward [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) from the point $(x,v)$ at time $t$ to time $s$ is

$$
 S_{s,t}(x,v)=\bigl(x\cosh(t-s)-v\sinh(t-s),\ v\cosh(t-s)-x\sinh(t-s)\bigr).
$$

Along this [characteristic curve](../../../partial-differential-equation.md#characteristic-curve), the [chain rule](../../../calculus.md#chain-rule) changes the transport equation into $d[f(s,S_{s,t}(x,v))]/ds=h(s,S_{s,t}(x,v))$. Integrating from zero to $t$ gives

$$
 \boxed{f(t,x,v)=f_0(S_{0,t}(x,v))+\int_0^t h(s,S_{s,t}(x,v))\,ds.}
$$

The assumed $C^1$ regularity makes this a classical solution: on every compact set, the integrand and its needed derivatives are continuous, so differentiation under the finite-time [integral](../../../calculus.md#integral) is justified. At $t=0$ it has the required initial value, and the characteristic calculation verifies the equation. Conversely every classical solution must satisfy the same integrated identity, proving uniqueness. This is the [Duhamel formula for Hamiltonian transport](../../../statistical-physics.md#duhamel-formula-for-hamiltonian-transport), with Hamiltonian $(v^2-x^2)/2$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The derivative of the backward [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) is

$$
 DS_{0,t}=\begin{pmatrix}\cosh t&-\sinh t\\-\sinh t&\cosh t\end{pmatrix},
 \qquad \boxed{\det DS_{0,t}=\cosh^2t-\sinh^2t=1.}
$$

Thus the [change of variables formula](../../../calculus.md#change-of-variables-formula) preserves phase-space [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). With zero source, $f_t=f_0\circ S_{0,t}$, so for every finite $p>0$,

$$
 \int_{\mathbb R^2}|f_t(x,v)|^p\,dx\,dv
 =\int_{\mathbb R^2}|f_0(x_0,v_0)|^p\,dx_0\,dv_0.
$$

Taking the $p$th root proves **$\|f_t\|_p=\|f_0\|_p$**. For $0<p<1$ this is a [quasi-norm](../../../functional-analysis.md#quasi-norm), and the argument still works because it uses only a change of variables, not the [triangle inequality](../../../topological-analysis.md#triangle-inequality). The identity also holds in the extended sense when an [integral](../../../calculus.md#integral) is infinite. Since the flow is bijective and measure-preserving, it additionally preserves the [essential supremum](../../../measure-theory.md#essential-supremum), so the same conclusion holds for $p=\infty$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Taking the [essential supremum](../../../measure-theory.md#essential-supremum) in the characteristic solution gives the sharper estimate

$$
 \boxed{\|f_t\|_\infty\leq\|f_0\|_\infty+\int_0^t\|h(s,\cdot,\cdot)\|_\infty\,ds.}
$$

Indeed, the bijective [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) preserves each spatial-velocity [essential supremum](../../../measure-theory.md#essential-supremum). If $H_t=\operatorname*{ess\,sup}_{0\leq s\leq t,\ x,v\in\mathbb R}|h(s,x,v)|$, this proves $\|f_t\|_\infty\leq\|f_0\|_\infty+tH_t$. A time-independent source has $H_t=\|h\|_{L^\infty(\mathbb R^2)}$, which is the displayed form. For a time-dependent source, the same symbol must mean a bound uniform over the elapsed time interval; its [norm](../../../functional-analysis.md#norm) at the final time alone need not bound the accumulated forcing.

The bound is **sharp**. Take $f_0=1$ and $h=1$, giving $f(t,x,v)=1+t$ and equality for every $t\geq0$. Both functions are smooth and bounded, although their finite-$p$ [integrals](../../../calculus.md#integral) over the whole plane are infinite.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Choose $f_0(x,v)=e^{-(x^2+v^2)}$ and $h(t,x,v)=x^2+v^2$. The initial [Gaussian function](../../../calculus.md#gaussian-function) is smooth and belongs to every finite [Lp space](../../../measure-theory.md#lp-space), and is also bounded. The source is smooth and nonzero. The accumulated source along the backward [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) is

$$
 \begin{aligned}
 q_t(x,v)&=\int_0^t|A_{s-t}(x,v)|^2\,ds\\
 &=\frac{\sinh(2t)}2(x^2+v^2)-(\cosh(2t)-1)xv.
 \end{aligned}
$$

Its quadratic-form eigenvalues are $(e^{2t}-1)/2$ and $(1-e^{-2t})/2$. Both are positive for $t>0$, so

$$
 f_t(x,v)=e^{-|A_{-t}(x,v)|^2}+q_t(x,v)
 \geq\frac{1-e^{-2t}}2(x^2+v^2).
$$

Consequently **$\|f_t\|_p=\infty$ for every $t>0$ and every finite $p\geq1$**; it is unbounded, so its $L^\infty$ [norm](../../../functional-analysis.md#norm) is infinite as well. This [spatially nonintegrable forcing in transport](../../../statistical-physics.md#spatially-nonintegrable-forcing-in-transport) example avoids any ambiguity about whether the last endpoint is included in “all $p$”.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For each $p\geq1$ with $f_0\in L^p$, a sufficient condition is $h\in L^1([0,T];L^p(\mathbb R^2))$ on every finite interval. The [Minkowski integral inequality](../../../functional-analysis.md#minkowski-integral-inequality) and measure preservation give the [finite-time Lp bound for Hamiltonian transport](../../../statistical-physics.md#finite-time-lp-bound-for-hamiltonian-transport)

$$
 \boxed{\|f_t\|_p\leq\|f_0\|_p+\int_0^t\|h(s)\|_p\,ds<\infty.}
$$

For all finite $p$ simultaneously, impose, for example, $h\in L^1_{\rm loc}([0,\infty);L^1\cap L^\infty)$. The elementary bound $\|h_s\|_p\leq\|h_s\|_1^{1/p}\|h_s\|_\infty^{1-1/p}$ and the [Holder inequality](../../../functional-analysis.md#holder-inequality) in time show that its $L^p$ [norms](../../../functional-analysis.md#norm) are locally integrable for every $1\leq p<\infty$. If a bounded initial value is also required, the same assumption controls the $p=\infty$ endpoint by the previous part.

A concrete stronger condition, compatible with a nonzero $C^1$ source, is that on each finite time interval the source has a common [compact support](../../../function.md#compact-support) in $(x,v)$. Its continuity then makes it bounded on that compact cylinder, so all these integrability conditions hold. A nonzero smooth source compactly supported in phase space supplies examples.

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the unit-period [circle](../../../topology.md#circle) $\mathbb T=\mathbb R/\mathbb Z$, with total measure one. The free [characteristic flow map](../../../partial-differential-equation.md#characteristic-flow-map) gives

$$
 f_t(x,v)=f_0(x-tv,v).
$$

Translations in $x$ preserve its periodic measure. The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) and the [integral](../../../calculus.md#integral) [triangle inequality](../../../topological-analysis.md#triangle-inequality) yield

$$
 \boxed{\|\rho_t\|_{L^1(\mathbb T)}
 \leq\int_{\mathbb T}\int_{\mathbb R}|f_0(x-tv,v)|\,dv\,dx
 =\|f_0\|_{L^1(\mathbb T\times\mathbb R)}.}
$$

The [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) therefore applies also to signed data, and the same translation gives

$$
 \boxed{\int_{\mathbb T}\rho_t(x)\,dx=\int_{\mathbb T}\int_{\mathbb R}f_0(x,v)\,dv\,dx=\rho_\infty.}
$$

This holds for positive or negative time. The printed $L^1(\mathbb R)$ in this subpart is a domain typo: the spatial variable is periodic, so the correct space is $L^1(\mathbb T)$. For example, the smooth initial value $f_0(x,v)=e^{-v^2}$ gives the constant density $\sqrt\pi$, whose periodic extension is not integrable on the real line.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix the mixed [Fourier transform](../../../analysis.md#fourier-transform) convention

$$
 \widehat f(t,k,\xi)=\int_0^1\int_{\mathbb R}
 f(t,x,v)e^{-2\pi i(kx+\xi v)}\,dv\,dx,
 \qquad k\in\mathbb Z,\quad\xi\in\mathbb R.
$$

The spatial derivative transforms to $2\pi ik\widehat f$, and multiplication by $v$ transforms to $-(2\pi i)^{-1}\partial_\xi\widehat f$. Hence the transformed [free transport equation](../../../partial-differential-equation.md#free-transport-equation) is

$$
 \boxed{\partial_t\widehat f-k\partial_\xi\widehat f=0.}
$$

Its [characteristic equations for a transport equation](../../../partial-differential-equation.md#characteristic-equations-for-a-transport-equation) give $\dot\xi=-k$, so the characteristic ending at $\xi$ at time $t$ began at $\xi+kt$. Consequently

$$
 \boxed{\widehat f(t,k,\xi)=\widehat f_0(k,\xi+kt).}
$$

The same sign follows directly by substituting $x=y+tv$ in the [Fourier transform](../../../analysis.md#fourier-transform) of $f_0(x-tv,v)$. No first velocity moment is assumed, so the differential equation may be understood in the sense of [tempered distributions](../../../fourier-analysis.md#tempered-distribution); the explicit transform formula is valid pointwise because $f_0$ is integrable.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) of the velocity-integrated density is its mixed transform at zero velocity frequency. Thus

$$
 \widehat\rho_t(k)=\widehat f(t,k,0)=\widehat f_0(k,kt).
$$

The constant $\rho_\infty$ contributes only to the zero [Fourier mode](../../../fourier-analysis.md#fourier-mode), where it equals $\widehat f_0(0,0)$. Therefore

$$
 \boxed{\widehat r_t(k)=\widehat f_0(k,kt)-\mathbf1_{\{k=0\}}\widehat f_0(0,0)
 =\begin{cases}\widehat f_0(k,kt),&k\ne0,\\0,&k=0.\end{cases}}
$$

It is important to remove the zero mode, which is conserved rather than mixed away.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Interpret the given velocity regularity in the stated [Sobolev space](../../../sobolev-space.md) sense. Repeated [integration by parts](../../../calculus.md#integration-by-parts), or the [Fourier transform of a derivative](../../../fourier-analysis.md#fourier-transform-of-a-derivative) in distributions, gives

$$
 (2\pi i\xi)^{n+1}\widehat f_0(k,\xi)
 =\widehat{\partial_v^{n+1}f_0}(k,\xi).
$$

The usual one-dimensional [one-dimensional Sobolev representative](../../../sobolev-space.md#one-dimensional-sobolev-representative) or a smooth approximation justifies this identity without imposing extra decay of classical derivatives at specific boundary points. The transform of an integrable function has absolute value at most its $L^1$ [norm](../../../functional-analysis.md#norm). Therefore

$$
 |\widehat f_0(k,\xi)|\,|\xi|^{n+1}
 \leq\frac{\|\partial_v^{n+1}f_0\|_1}{(2\pi)^{n+1}}
 \leq\frac{\|f_0\|_{L_x^1W_v^{n+1,1}}}{(2\pi)^{n+1}}.
$$

Setting $\xi=kt$ and taking the supremum gives the required **uniform weighted bound**. The $k=0$ term on the left is zero; there is no division by that frequency in this argument.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Take the positive integer $n\geq1$ and put $m=n+1\geq2$. From the preceding estimate and the absent zero [Fourier mode](../../../fourier-analysis.md#fourier-mode), for $t\ne0$,

$$
 \begin{aligned}
 \sum_{k\in\mathbb Z}|\widehat r_t(k)|
 &\leq\frac{\|\partial_v^m f_0\|_1}{(2\pi)^m|t|^m}
 \sum_{k\ne0}\frac1{|k|^m}\\
 &=\frac{2\zeta(m)\|\partial_v^m f_0\|_1}{(2\pi)^m|t|^m}.
 \end{aligned}
$$

Here $\zeta$ is the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function), and its displayed series is finite because $m>1$. One may replace the last derivative [norm](../../../functional-analysis.md#norm) by the given full mixed [Sobolev norm](../../../sobolev-space.md#sobolev-norm) to obtain the requested constant depending only on $n$ and $f_0$.

An absolutely summable sequence of [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) gives a uniformly and absolutely convergent [Fourier series](../../../fourier-series.md), with supremum bounded by the sum of their absolute values. Its sum agrees almost everywhere with $r_t$ by uniqueness of [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) for integrable periodic functions. Hence

$$
 \boxed{\|\rho_t-\rho_\infty\|_{L^\infty(\mathbb T)}
 \leq\frac{2\zeta(n+1)}{(2\pi)^{n+1}}
 \frac{\|\partial_v^{n+1}f_0\|_1}{|t|^{n+1}}
 \longrightarrow0.}
$$

This is the [uniform phase-mixing bound from velocity derivatives](../../../statistical-physics.md#uniform-phase-mixing-bound-from-velocity-derivatives): uniform convergence for the continuous representative of the density, with rate $O(|t|^{-n-1})$. No uniform decay of the full phase-space distribution is asserted. The [free-transport phase mixing](../../../statistical-physics.md#free-transport-phase-mixing) acts by shifting nonzero spatial modes to large velocity frequency. If a convention allows $0\in\mathbb N$, that endpoint needs separate assumptions or an argument: the harmonic series in this proof would diverge.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $E=L^1(\mathbb R_x^d\times\mathbb R_v^d)$, and denote the [free-transport semigroup](../../../partial-differential-equation.md#free-transport-semigroup) by $(U_tg)(x,v)=g(x-tv,v)$. For fixed $v$, the spatial translation has unit [Jacobian determinant](../../../calculus.md#jacobian-determinant), so the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) gives

$$
 \boxed{\|U_tf_0\|_1=\int\int|f_0(x-tv,v)|\,dx\,dv
 =\int\int|f_0(y,v)|\,dy\,dv=\|f_0\|_1.}
$$

Thus the given free term is an [isometry](../../../riemannian-geometry.md#isometry) on $E$. The operators form a [strongly continuous semigroup](../../../functional-analysis.md#c0-semigroup): continuity first holds for smooth compactly supported functions by dominated convergence, and density plus the isometry extends it to every $L^1$ function.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) and [integral](../../../calculus.md#integral) [triangle inequality](../../../topological-analysis.md#triangle-inequality) give

$$
 \boxed{\|\rho(g)\|_{L^1_x}\leq\int\int|g(x,v)|\,dv\,dx=\|g\|_1.}
$$

Define the [normalized velocity-reset collision operator](../../../statistical-physics.md#normalized-velocity-reset-collision-operator) using the [normalized velocity-reset projection](../../../statistical-physics.md#normalized-velocity-reset-projection) $Pg(x,v)=\rho(g)(x)M(v)$ and $B=P-I$. Since $M\geq0$ and $\int M=1$,

$$
 \|Pg\|_1=\|\rho(g)\|_{L^1_x}\leq\|g\|_1,
 \qquad \|Bg\|_1\leq2\|g\|_1.
$$

Also $P^2=P$; the collision gain replaces the velocity distribution by $M$ while preserving the spatial mass. In [Bochner integral](../../../measure-theory.md#bochner-integral) notation the printed, undamped source operator is

$$
 (\tau f)(t)=\int_0^tU_{t-s}Bf(s)\,ds.
$$

Using the transport [isometry](../../../riemannian-geometry.md#isometry) and the [integral](../../../calculus.md#integral) [triangle inequality](../../../topological-analysis.md#triangle-inequality) proves

$$
 \boxed{\|\tau f(t)\|_1\leq2\int_0^t\|f(s)\|_1\,ds
 \leq2t\sup_{0\leq s\leq t}\|f(s)\|_1.}
$$

These estimates hold for measurable, locally time-bounded $E$-valued functions. If the displayed supremum is infinite, the numerical bound is interpreted in the extended sense; the construction below works in a space where it is finite.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Fix $T$ and set $A_T=\sup_{0\leq s\leq T}\|f(s)\|_1$. The preceding [integral](../../../calculus.md#integral) estimate gives the result for one iterate. If for some $n\geq0$ the bound $\|\tau^nf(s)\|_1\leq A_T2^ns^n/n!$ holds for $s\leq T$, then

$$
 \|\tau^{n+1}f(t)\|_1\leq2\int_0^t\|\tau^nf(s)\|_1\,ds
 \leq\frac{2^{n+1}A_T}{n!}\int_0^t s^n ds
 =\frac{2^{n+1}t^{n+1}}{(n+1)!}A_T.
$$

Taking $T=t$ yields exactly

$$
 \boxed{\|\tau^nf(t)\|_1\leq\frac{(2t)^n}{n!}
 \sup_{0\leq s\leq t}\|f(s)\|_1.}
$$

The case $n=0$ uses the identity operator. This [factorial bound for a Volterra iterate](../../../analysis.md#factorial-bound-for-a-volterra-iterate) comes from time ordering, so no commutation between free transport and the collision projection is assumed.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

On each finite interval use the [Banach space](../../../banach-space.md) $X_T=C([0,T];E)$ with the supremum [norm](../../../functional-analysis.md#norm). The free term $g(t)=U_tf_0$ belongs to $X_T$, and the time-[integral](../../../calculus.md#integral) operator $\tau$ maps $X_T$ to itself with [norm](../../../functional-analysis.md#norm) at most $2T$. The [strongly continuous semigroup](../../../functional-analysis.md#c0-semigroup) property and boundedness of $B$ justify continuity of the [Bochner integral](../../../measure-theory.md#bochner-integral).

Define

$$
 \boxed{f=\sum_{j=0}^\infty\tau^jg.}
$$

The [factorial bound for a Volterra iterate](../../../analysis.md#factorial-bound-for-a-volterra-iterate) gives $\|\tau^jg\|_{X_T}\leq(2T)^j\|f_0\|_1/j!$. The series therefore converges absolutely in $X_T$. Since $\tau$ is a bounded [linear operator](../../../vector-space.md#linear-operator) on $X_T$, it can be passed through the convergent sum, giving

$$
 \tau f=\sum_{j=1}^\infty\tau^jg=f-g.
$$

Thus $f=g+\tau f$, the required [integral](../../../calculus.md#integral) formulation, and $f(0)=f_0$. Each term on a larger interval restricts to the identical term on a smaller interval, so these constructions define a single global solution without having to restart at successive times. This is an [integrable Volterra solution for normalized velocity relaxation](../../../statistical-physics.md#integrable-volterra-solution-for-normalized-velocity-relaxation). It is a [mild solution of an abstract Cauchy problem](../../../functional-analysis.md#mild-solution-of-an-abstract-cauchy-problem) in $L^1$ and hence an $L^1$ weak solution in the paper's [integral](../../../calculus.md#integral)-formulation sense. No smallness condition such as $2T<1$ is needed.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For $0\leq s\leq t$, sum the same absolutely convergent [Neumann series](../../../banach-algebra.md#neumann-series) estimate:

$$
 \|f(s)\|_1\leq\sum_{j=0}^\infty\frac{(2s)^j}{j!}\|f_0\|_1
 =e^{2s}\|f_0\|_1.
$$

Consequently

$$
 \boxed{\sup_{0\leq s\leq t}\|f(s)\|_1\leq e^{2t}\|f_0\|_1<\infty.}
$$

This coarse bound is sufficient for the requested locally uniform control and the uniqueness argument. It is not claimed to be the sharp dissipative estimate for the collision model.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

If $f$ and $\widetilde f$ are two weak solutions with the same initial value and the required local time bound, their difference $w$ satisfies $w=\tau w$. By [linearity](../../../vector-space.md#linearity) this implies $w=\tau^nw$ for every $n$. On $[0,T]$ put $A_T=\sup_{s\leq T}\|w(s)\|_1<\infty$. The [factorial bound for a Volterra iterate](../../../analysis.md#factorial-bound-for-a-volterra-iterate) now gives

$$
 \|w(t)\|_1\leq A_T\frac{(2T)^n}{n!},\qquad0\leq t\leq T.
$$

For fixed $T$, the factor tends to zero; its successive-term ratio is $2T/(n+1)$. Therefore $w(t)=0$ as an $L^1$ element at every time on this interval. Since $T$ is arbitrary, **the locally time-bounded $L^1$ weak solution is unique globally**. This proof uses precisely the additional condition requested, rather than assuming arbitrary pointwise-in-time integrability alone supplies a finite uniform bound.

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the genuine planar [Givens rotation](../../../numerical-analysis.md#givens-rotation)

$$
 \binom{v_i(\theta)}{v_j(\theta)}
 =\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}
 \binom{v_i}{v_j}.
$$

In the second component the cosine multiplies $v_j$: the repeated $v_i$ in the printed formula is an error. With that printed expression, at $\theta=0$ the pair becomes $(v_i,v_i)$, which does not preserve length or measure. The rotation-based claims require the corrected expression. Also take $N\geq2$, since the normalization by $\binom N2$ is undefined for $N=1$.

Let $C_N=\binom N2$ and $U_{ij,\theta}F=F\circ R_{ij,\theta}$. The [change of variables formula](../../../calculus.md#change-of-variables-formula) and determinant one give $\|U_{ij,\theta}F\|_2=\|F\|_2$. Thus each is a [unitary operator](../../../vector-space.md#unitary-operator), with adjoint $U_{ij,-\theta}$. The [Kac collision operator](../../../statistical-physics.md#kac-collision-operator) is the average

$$
 Q=\frac1{C_N}\sum_{i<j}\frac1{2\pi}\int_0^{2\pi}U_{ij,\theta}\,d\theta.
$$

The [Minkowski integral inequality](../../../functional-analysis.md#minkowski-integral-inequality) gives $\|QF\|_2\leq\|F\|_2$, so $Q$ is bounded. For the [Hilbert space](../../../hilbert-space.md) [inner product](../../../linear-algebra.md#inner-product), integration and the angular change $\theta\mapsto-\theta$ give

$$
 \langle G,QF\rangle
 =\frac1{2\pi C_N}\sum_{i<j}\int_0^{2\pi}\langle U_{ij,-\theta}G,F\rangle d\theta
 =\langle QG,F\rangle.
$$

Hence **$Q=Q^*$ and $\|Q\|\leq1$**. In fact a nonzero radial [Gaussian function](../../../calculus.md#gaussian-function) is fixed by every rotation, showing $\|Q\|=1$. Angular averages can be understood as strong [Bochner integrals](../../../measure-theory.md#bochner-integral); continuity of rotations in $L^2$ follows first for smooth compactly supported functions, then by density.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For each rotation, [unitarity](../../../vector-space.md#unitary-operator) gives

$$
 \|U_{ij,\theta}F-F\|_2^2
 =2\|F\|_2^2-2\operatorname{Re}\langle F,U_{ij,\theta}F\rangle.
$$

Averaging and using self-adjointness of $Q$ yields the [Dirichlet form of the Kac collision operator](../../../statistical-physics.md#dirichlet-form-of-the-kac-collision-operator)

$$
 \boxed{\langle F,(I-Q)F\rangle
 =\frac1{4\pi C_N}\sum_{i<j}\int_0^{2\pi}\int_{\mathbb R^N}
 |F(R_{ij,\theta}\mathbf v)-F(\mathbf v)|^2\,d\mathbf v\,d\theta.}
$$

The velocity [integral](../../../calculus.md#integral) is necessary: its omission from the printed right-hand side would leave a function of $\mathbf v$ rather than a scalar. This identity applies to every $L^2$ function, with complex modulus when necessary, and is nonnegative.

If $(I-Q)F=0$, every nonnegative angular [integral](../../../calculus.md#integral) is zero, so $\|U_{ij,\theta}F-F\|_2=0$ for almost every angle. Strong continuity in angle extends equality to every angle. The coordinate-plane [Givens rotations](../../../numerical-analysis.md#givens-rotation) generate the [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) $SO(N)$, hence $F$ is invariant in $L^2$ under every element of this group. To identify its shape rigorously despite almost-everywhere representatives, average over the normalized [Haar measure](../../../measure-theory.md#haar-measure) of $SO(N)$. This averaging leaves $F$ unchanged, while transitivity of the rotation group on each sphere makes the average a [radial function](../../../partial-differential-equation.md#radial-function). Thus $F(\mathbf v)=\phi(|\mathbf v|)$ almost everywhere.

Conversely, every [radial function](../../../partial-differential-equation.md#radial-function) is fixed by every coordinate-plane rotation, and so by $Q$. Therefore

$$
 \boxed{\ker(I-Q)=\{F\in L^2(\mathbb R^N):F(\mathbf v)=\phi(|\mathbf v|)\ \text{a.e.}\}.}
$$

This is the [radial kernel of the Kac collision operator](../../../statistical-physics.md#radial-kernel-of-the-kac-collision-operator). The rotation correction is essential to this conclusion: with the literal printed map, even $F(\mathbf v)=e^{-|\mathbf v|^2}$ in dimension two is not fixed. At $\mathbf v=(0,1)$ its printed-map angular average is the average of $e^{-\sin^2\theta}$, strictly greater than its value $e^{-1}$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write $F=F_N$ and integrate the [Kac master equation](../../../statistical-physics.md#kac-master-equation) over $v_2,\ldots,v_N$. For a pair $i,j\geq2$, the rotation acts only on integrated variables. Its unit [Jacobian determinant](../../../calculus.md#jacobian-determinant) makes the integrated gain identical to the integrated loss, so all those pairs cancel.

The only remaining pairs are $(1,j)$, $j=2,\ldots,N$. For such a pair, first integrate over every variable except $v_1$ and $v_j$. This yields the corresponding two-coordinate [marginal distribution](../../../probability-theory.md#marginal-distribution) evaluated at the rotated pair. Permutation symmetry of $F_N$ makes all $N-1$ resulting [integrals](../../../calculus.md#integral) identical to the one for $(1,2)$. The coefficient is

$$
 \frac{N(N-1)}{2\pi\binom N2}=\frac1\pi.
$$

Consequently the [Kac marginal evolution equation](../../../statistical-physics.md#kac-marginal-evolution-equation) is

$$
 \boxed{\partial_t\Pi_1(F_N)(v_1)
 =\frac1\pi\int_{\mathbb R}\int_0^{2\pi}
 \left[\Pi_2(F_N)(v_1\cos\theta+v_2\sin\theta,
 -v_1\sin\theta+v_2\cos\theta)-\Pi_2(F_N)(v_1,v_2)\right]d\theta\,dv_2.}
$$

The time argument has been suppressed on the right. The loss is consistent with normalization, since $\int\Pi_2(v_1,v_2)dv_2=\Pi_1(v_1)$. Under the printed definition $k<N$, this use of $\Pi_2$ requires $N\geq3$. For $N=2$ the same formula holds with the natural extension $\Pi_N(F_N)=F_N$.

This identity is exact and generally unclosed. Replacing the two-coordinate [marginal distribution](../../../probability-theory.md#marginal-distribution) by the product of one-coordinate marginals would produce the quadratic collision equation associated with [Kac chaos](../../../statistical-physics.md#kac-chaos). Permutation symmetry alone does not imply that product approximation.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Put $u=F_N/\gamma_N$, where the Gaussian density is strictly positive. Extend $u\log u$ continuously at zero by $0\log0=0$. Both densities have [integral](../../../calculus.md#integral) one, so the [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) can be written as

$$
 \begin{aligned}
 H_N(F_N)&=\int_{\mathbb R^N}\gamma_N u\log u\,d\mathbf v\\
 &=\int_{\mathbb R^N}\gamma_N(u\log u-u+1)\,d\mathbf v.
 \end{aligned}
$$

The bracket is nonnegative and vanishes only at $u=1$: its derivative for $u>0$ is $\log u$, with a unique minimum at one. Hence

$$
 \boxed{H_N(F_N)\geq0,\qquad H_N(F_N)=0\ \Longleftrightarrow\ F_N=\gamma_N\ \text{a.e.}}
$$

The inequality holds also for infinite entropy. Its negative integrand part is integrable, since $u\log u\geq-1/e$ and $\gamma_N$ has [integral](../../../calculus.md#integral) one, so the extended-value [integral](../../../calculus.md#integral) is well defined. This is [relative entropy in Kac's model](../../../statistical-physics.md#relative-entropy-in-kac-s-model); no differentiation is needed for nonnegativity.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Use the correct Gaussian entropy decomposition

$$
 H_N(F)=\int F\log F\,d\mathbf v+\frac N2\log(2\pi)
 +\frac12\int|\mathbf v|^2F\,d\mathbf v.
$$

The last coefficient is $1/2$, as follows from $-\log\gamma_N=N\log(2\pi)/2+|\mathbf v|^2/2$; the printed hint omits it. Under the allowed differentiability and integrability assumptions, the supplied collision invariants conserve mass and energy. Differentiating therefore gives

$$
 \frac d{dt}H_N(F)=N\int(Q-I)F\log F\,d\mathbf v,
$$

where the extra derivative term $\int\partial_tF$ vanishes by [mass conservation](../../../continuum-mechanics.md#mass-conservation). Thus the [Kac entropy production](../../../statistical-physics.md#kac-entropy-production) is

$$
 D_N(F)=\frac{N}{2\pi C_N}\sum_{i<j}\int_{\mathbb R^N}\int_0^{2\pi}
 (F-F\circ R_{ij,\theta})\log F\,d\theta\,d\mathbf v.
$$

For one pair, call the double [integral](../../../calculus.md#integral) $A_{ij}$. The measure-preserving substitution $(\mathbf v,\theta)\mapsto(R_{ij,\theta}\mathbf v,-\theta)$ interchanges $F$ and $F\circ R_{ij,\theta}$, with angles taken modulo $2\pi$. Averaging the original and substituted expressions gives

$$
 A_{ij}=\frac12\int_{\mathbb R^N}\int_0^{2\pi}
 (F\circ R_{ij,\theta}-F)
 (\log(F\circ R_{ij,\theta})-\log F)\,d\theta\,d\mathbf v.
$$

Since $N/(4\pi C_N)=1/[2\pi(N-1)]$, the desired [Kac entropy dissipation](../../../statistical-physics.md#kac-entropy-production) formula is

$$
 \boxed{D_N(F)=\frac1{2\pi(N-1)}\sum_{i<j}\int_{\mathbb R^N}\int_0^{2\pi}
 (F(R_{ij,\theta}\mathbf v)-F(\mathbf v))
 \log\!\frac{F(R_{ij,\theta}\mathbf v)}{F(\mathbf v)}\,d\theta\,d\mathbf v\geq0.}
$$

For positive values $a,b$, $(a-b)(\log a-\log b)\geq0$ because the logarithm is increasing. At two zeros use value zero; at one zero and one positive value use the nonnegative extended value $+\infty$. One may first use positive densities and then regularize by $(F+\varepsilon\gamma_N)/(1+\varepsilon)$; rotation invariance of $\gamma_N$ preserves the formula and permits the usual limit at zeros under the stated assumptions.

Thus **relative entropy is nonincreasing** along the evolution. When the dissipation is finite, zero dissipation means pairwise rotation invariance and hence radiality, by the preceding kernel argument. Radial normalized densities other than $\gamma_N$ can be stationary with positive relative entropy: vanishing dissipation is not a claim that the unique stationary density is Gaussian.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
