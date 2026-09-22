# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper7.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [harmonic function](../../../partial-differential-equation.md#harmonic-function) on $\Omega$ is a twice continuously differentiable function satisfying $\Delta u=0$ there. For complex-valued functions this means that both its [real part](../../../complex-analysis.md#real-part) and its [imaginary part](../../../complex-analysis.md#imaginary-part) are [harmonic functions](../../../partial-differential-equation.md#harmonic-function). The [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) characterizes harmonicity: a [continuous function](../../../calculus.md#continuous-function) is harmonic exactly when its value at each point equals its average over every [sphere](../../../geometry-and-topology.md#sphere), or equivalently every ball, whose closed ball lies in $\Omega$. In the forward direction, the derivative of the spherical average vanishes by the [divergence theorem](../../../calculus.md#divergence-theorem). Conversely, radial smoothing leaves a [continuous function](../../../calculus.md#continuous-function) with the mean value property unchanged locally; it is therefore smooth. Expanding its small-ball average gives $u(x)+r^2\Delta u(x)/(2(d+3))+o(r^2)$ in dimension $d+1$, and hence $\Delta u=0$.

Write $M=\|u\|_{h^1}$ and $v_{d+1}$ for the volume of the unit ball in $\mathbb R^{d+1}$. We first obtain a pointwise estimate directly from the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions), before using any boundary representation. For the ball of radius $r=t/2$ centered at $(x,t)$,

$$
|u(x,t)|\leq\frac{1}{v_{d+1}r^{d+1}}\int_{t-r}^{t+r}\int_{\mathbb R^d}|u(y,s)|\,dy\,ds
\leq\frac{2^{d+1}}{v_{d+1}}\frac{M}{t^d}.
$$

Thus every upward shift of $u$ is a bounded [harmonic function](../../../partial-differential-equation.md#harmonic-function), with a continuous bounded boundary value.

The required map is the [Poisson integral](../../../partial-differential-equation.md#poisson-integral)

$$
P\mu(x,t)=\int_{\mathbb R^d}P_t(x-y)\,d\mu(y),\qquad
P_t(x)=c_d\frac{t}{(t^2+|x|^2)^{(d+1)/2}},\qquad
c_d=\frac{\Gamma((d+1)/2)}{\pi^{(d+1)/2}}.
$$

The [Poisson kernel for the upper half-space](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-space) is positive, has integral one, and is harmonic as a function of $(x,t)$. Its normalization follows by polar coordinates and $r=\tan\theta$, which reduces the radial integral to $\int_0^{\pi/2}\sin^{d-1}\theta\,d\theta$; direct differentiation gives $\Delta_{x,t}P_t=0$. Differentiation under the integral on compact subsets proves that $P\mu$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function). [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) gives

$$
\int|P\mu(x,t)|\,dx\leq\int\int P_t(x-y)\,dx\,d|\mu|(y)=\|\mu\|_{\mathrm{TV}}.
$$

Here the [total variation norm of a measure](../../../measure-theory.md#total-variation-norm-of-a-measure) is the [norm](../../../functional-analysis.md#norm) on finite signed or complex [Borel measures](../../../measure-theory.md#borel-measure).

The [Poisson kernel for the upper half-space](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-space) is an [approximate identity](../../../fourier-analysis.md#approximate-identity): for $\psi\in C_0(\mathbb R^d)$, $P_t*\psi\to\psi$ uniformly. Indeed, [uniform continuity](../../../topological-analysis.md#uniform-continuity) controls translations smaller than a fixed radius, and the kernel mass outside that radius tends to zero. Consequently

$$
\int\psi(x)P\mu(x,t)\,dx\longrightarrow\int\psi\,d\mu.
$$

The dual characterization of the [total variation norm of a measure](../../../measure-theory.md#total-variation-norm-of-a-measure), as the supremum over $\psi\in C_0$ of supremum [norm](../../../functional-analysis.md#norm) at most one, now gives the reverse inequality $\|\mu\|_{\mathrm{TV}}\leq\|P\mu\|_{h^1}$. Thus $P$ is a linear [isometry](../../../riemannian-geometry.md#isometry) and is injective.

For surjectivity, fix $s>0$ and put $u_s(x)=u(x,s)$. Bounded harmonic uniqueness in the upper half-space gives

$$
u(x,s+t)=P_t*u_s(x),\qquad t>0.
$$

To justify this uniqueness, subtract the [Poisson integral](../../../partial-differential-equation.md#poisson-integral) of the bounded continuous boundary value from the upward-shifted harmonic function. Their difference is bounded and harmonic and has zero continuous boundary values. Its odd reflection across the boundary is an entire bounded [harmonic function](../../../partial-differential-equation.md#harmonic-function); the reflection is harmonic across the flat boundary by [harmonic odd reflection across a hyperplane](../../../partial-differential-equation.md#harmonic-odd-reflection-across-a-hyperplane). The [Liouville theorem for harmonic functions](../../../partial-differential-equation.md#harmonic-liouville-theorem) makes it constant, and oddness makes it zero. The initial pointwise estimate supplies the boundedness needed here. To see the reflection locally, take a ball centered on the hyperplane and extend the boundary data on its upper hemisphere oddly to its lower hemisphere. The harmonic solution on this ball is odd and zero on its equatorial disk. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) identifies it with the given difference on the upper half-ball, proving that the reflected function is harmonic across the boundary.

Choose $s_j\downarrow0$. The measures $u_{s_j}\,dx$ have [total variation norm of a measure](../../../measure-theory.md#total-variation-norm-of-a-measure) at most $M$. By the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem), and separability of $C_0(\mathbb R^d)$, a [subsequence](../../../real-analysis.md#subsequence) converges in the [weak-star topology](../../../weak-topology.md#weak-star-topology) to a finite measure $\mu$ with $\|\mu\|_{\mathrm{TV}}\leq M$. For fixed $(x,t)$ and $s_j<t$,

$$
u(x,t)=\int P_{t-s_j}(x-y)u(y,s_j)\,dy.
$$

The kernels in this display belong to $C_0$ and converge uniformly to $P_t(x-\cdot)$. The uniform measure [norm](../../../functional-analysis.md#norm) bound therefore allows passage to the limit, giving $u(x,t)=P\mu(x,t)$. This proves the [Poisson representation of harmonic h1 by finite measures](../../../partial-differential-equation.md#poisson-representation-of-harmonic-h1-by-finite-measures), including onto-ness.

Finally $P_t(x)\leq c_dt^{-d}$, so the [Poisson representation of harmonic h1 by finite measures](../../../partial-differential-equation.md#poisson-representation-of-harmonic-h1-by-finite-measures) improves the preliminary pointwise constant:

$$
\boxed{\|P\mu\|_{h^1}=\|\mu\|_{\mathrm{TV}},\qquad |u(x,t)|\leq c_dt^{-d}\|u\|_{h^1}.}
$$

The last occurrence of $h^1(\mathbb R^{d+1})$ in the printed question is understood as the [harmonic Hardy space of the upper half-space](../../../partial-differential-equation.md#harmonic-hardy-space-of-the-upper-half-space) defined earlier in that question.

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a positive [Borel measure](../../../measure-theory.md#borel-measure) $\nu$, the centered [Hardy-Littlewood maximal function](../../../analysis.md#hardy-littlewood-maximal-function) and the [uncentered maximal function of a finite measure](../../../analysis.md#uncentered-maximal-function-of-a-finite-measure) are

$$
m\nu(x)=\sup_{r>0}\frac{\nu(B(x,r))}{|B(x,r)|},\qquad
m_u\nu(x)=\sup_{x\in B(c,r)}\frac{\nu(B(c,r))}{|B(c,r)|}.
$$

We use open balls and allow infinite values. For signed or complex measures the definition uses their [total variation measure](../../../measure-theory.md#variation-measure). Since a centered ball is also an admissible uncentered ball, and every ball $B(c,r)$ containing $x$ lies in $B(x,2r)$,

$$
\boxed{m\nu(x)\leq m_u\nu(x)\leq2^d m\nu(x).}
$$

For functions, $m(f)$ means the centered [Hardy-Littlewood maximal function](../../../analysis.md#hardy-littlewood-maximal-function) of $|f|\,dx$.

The set $E_\alpha$ is the union of the open balls $B$ with $\nu(B)>\alpha|B|$. In particular, each witnessing ball lies entirely inside $E_\alpha$. If $K\subset E_\alpha$ is compact, take a finite witnessing cover of $K$. Choose its largest-radius ball, discard all balls meeting it, and repeat. The selected balls $B_j$ are disjoint. Every discarded ball has no larger radius than the selected ball that discarded it and is contained in its threefold dilation. Hence

$$
|K|\leq3^d\sum_j|B_j|\leq\frac{3^d}{\alpha}\sum_j\nu(B_j)
\leq\frac{3^d}{\alpha}\nu(E_\alpha).
$$

Taking the supremum over compact $K$ by [inner regularity of Lebesgue measure](../../../measure-theory.md#inner-regularity-of-lebesgue-measure) proves the stronger, localized estimate

$$
\boxed{|E_\alpha|\leq\frac{3^d}{\alpha}\nu(E_\alpha).}
$$

If the right side is infinite there is nothing to prove. Positivity of the measure is important: a signed version uses $|\nu|(E_\alpha)$, not $\nu(E_\alpha)$.

For the radial-kernel inequality, integrability implies $\phi(r)\to0$. For $0<s<\phi(0)$, let $r(s)$ be the unique radius with $\phi(r(s))=s$. The [layer cake representation](../../../functional-analysis.md#layer-cake-representation) and [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) give

$$
\begin{aligned}
t^{-d}\int\phi(|x-y|/t)|f(y)|\,dy
&=\int_0^{\phi(0)}t^{-d}\int_{B(x,tr(s))}|f(y)|\,dy\,ds\\
&\leq m(f)(x)\int_0^{\phi(0)}v_d r(s)^d\,ds
=m(f)(x).
\end{aligned}
$$

The last integral equals the total mass of $\phi(|\cdot|)$, namely one. Taking the absolute value of the original [convolution](../../../fourier-analysis.md#convolution) therefore proves the claim with constant exactly one. This is [radial decreasing kernel domination by the maximal function](../../../analysis.md#radial-decreasing-kernel-domination-by-the-maximal-function).

An application is boundary convergence of the [Poisson integral](../../../partial-differential-equation.md#poisson-integral). Its normalized radial profile is $c_d(1+r^2)^{-(d+1)/2}$, so $\sup_{t>0}|P_t*f|\leq m(f)$. For a continuous compactly supported $g$, the [approximate identity](../../../fourier-analysis.md#approximate-identity) property gives $P_t*g\to g$ pointwise. For arbitrary $f\in L^1$, put $h=f-g$; then

$$
\limsup_{t\downarrow0}|P_t*f(x)-f(x)|\leq m(h)(x)+|h(x)|.
$$

The preceding [weak type (1,1)](../../../functional-analysis.md#weak-type-1-1) estimate and the elementary integral bound for $|h|$ show that the set where this exceeds $2a$ has measure at most $(3^d+1)\|h\|_1/a$. Continuous compactly supported functions are dense in $L^1$, so this measure is zero. Thus **the Poisson integrals of an integrable function converge to it almost everywhere**; the same [approximate identity](../../../fourier-analysis.md#approximate-identity) also gives convergence in $L^1$.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We first construct a terminal integrable function without using the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem). Put $G=\sup_n|g_n|$ and $d\eta=G\,dx$ on $(0,1]^d$. This is a finite positive measure. If $G=0$ almost everywhere the conclusion is immediate. Otherwise, for a bounded dyadic step function $h$ measurable with respect to $\mathcal F_n$ in the [dyadic filtration](../../../stochastic-process.md#dyadic-filtration), define

$$
\Lambda(h)=\int h g_n\,dx.
$$

The [martingale](../../../martingale.md) property makes the definition independent of the choice of a sufficiently large $n$. Moreover $|\Lambda(h)|\leq\int|h|\,d\eta$. Dyadic step functions are dense in $L^1(\eta)$: [continuous functions](../../../calculus.md#continuous-function) on the closed unit cube are dense for this finite [Borel measure](../../../measure-theory.md#borel-measure) (extend the measure by zero onto the omitted faces), and [uniform continuity](../../../topological-analysis.md#uniform-continuity) approximates each [continuous function](../../../calculus.md#continuous-function) by step functions on fine dyadic partitions. Thus $\Lambda$ extends to a [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) on $L^1(\eta)$ of [norm](../../../functional-analysis.md#norm) at most one. The [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces) representation of this functional gives $H\in L^\infty(\eta)$ with $|H|\leq1$ and $\Lambda(h)=\int hH\,d\eta$. Set $g=HG$, taking $g=0$ where $G=0$. Then $g\in L^1(dx)$ and testing indicators of all dyadic atoms proves

$$
\boxed{g_n=\mathbb E(g\mid\mathcal F_n).}
$$

This argument also works for complex-valued [martingales](../../../martingale.md), with a complex [linear functional](../../../linear-algebra.md#linear-functional).

To prove convergence, choose a dyadic step function $h$ with $\|g-h\|_1$ arbitrarily small. For all $n$ beyond its dyadic level, $\mathbb E(h\mid\mathcal F_n)=h$. The [L1 contraction of conditional expectation](../../../measure-theory.md#l1-contraction-of-conditional-expectation) yields

$$
\|g_n-g\|_1\leq\|\mathbb E(g-h\mid\mathcal F_n)\|_1+\|g-h\|_1
\leq2\|g-h\|_1.
$$

This proves convergence in $L^1$. For convergence [almost everywhere](../../../measure-theory.md#almost-everywhere), [Doob maximal inequality](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) applied to the [conditional expectations](../../../measure-theory.md#conditional-expectation) of $g-h$ gives

$$
\begin{aligned}
\left|\left\{\limsup_n|g_n-g|>2a\right\}\right|
&\leq\left|\left\{\sup_n|\mathbb E(g-h\mid\mathcal F_n)|>a\right\}\right|
+|\{|g-h|>a\}|\\
&\leq\frac{2\|g-h\|_1}{a}.
\end{aligned}
$$

Let the approximation error tend to zero, and then take positive rational $a$. Hence **$g_n\to g$ both in $L^1$ and almost everywhere**.

For the second assertion, write $M=\sup_n\mathbb E|f_n|<\infty$ and take the given first-exit [stopping time](../../../martingale.md#stopping-time) $\tau$. Each $g_n=f_{\tau\wedge n}$ is integrable, being a finite sum of restrictions of integrable variables. Its increments satisfy

$$
g_{n+1}-g_n=\mathbf1_{\{\tau>n\}}(f_{n+1}-f_n).
$$

The indicator is $\mathcal F_n$-measurable, so taking its [conditional expectation](../../../measure-theory.md#conditional-expectation) proves that $(g_n)$ is a [martingale](../../../martingale.md).

The overshoot at $\tau$ need not be bounded by $N$. Instead, for a fixed $m$, on $\{\tau=j\}$ with $j\leq m$ we have $|f_j|\leq\mathbb E(|f_m|\mid\mathcal F_j)$. Integrating over this $\mathcal F_j$-measurable event, summing the disjoint events, and including $\{\tau>m\}$ gives

$$
\mathbb E|g_m|\leq\mathbb E|f_m|\leq M.
$$

The variables $Z_m=|f_\tau|\mathbf1_{\{\tau\leq m\}}$ increase to $Z$, and $Z_m\leq|g_m|$. The [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) gives $\mathbb E Z\leq M$. Before stopping, the process has magnitude less than $N$; after stopping it remains at $f_\tau$. Consequently

$$
\boxed{g^*\leq Z\vee N,\qquad\mathbb E(Z\vee N)\leq M+N<\infty.}
$$

This is the [integrable overshoot of a stopped L1-bounded martingale](../../../martingale.md#integrable-overshoot-of-a-stopped-l1-bounded-martingale). The first part now proves that every such stopped process converges [almost everywhere](../../../measure-theory.md#almost-everywhere).

Finally, [Doob maximal inequality](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) gives $|\{\sup_n|f_n|\geq N\}|\leq M/N$, by applying the finite-horizon estimate and then increasing the horizon. Thus $\sup_n|f_n|$ is finite [almost everywhere](../../../measure-theory.md#almost-everywhere). Outside the union of the null sets for all positive integer stopping thresholds, choose an integer $N$ larger than this supremum. No stopping occurs at that point, so $f_n=g_n$ for all $n$, and **$f_n$ converges to a finite limit almost everywhere**. We have not assumed, or concluded, $L^1$ convergence for this general $L^1$-bounded [martingale](../../../martingale.md).

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The defining [convolution](../../../fourier-analysis.md#convolution) integral is absolutely convergent for every $x$ when $e\in L^1+L^2$. Indeed, writing $e=a+b$ with $a\in L^1$ and $b\in L^2$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\int|K(x-y)e(y)|\,dy\leq\|K\|_\infty\|a\|_1+\|K\|_2\|b\|_2<\infty.
$$

Disjoint supports imply $\sum_n|e_n(y)|=|e(y)|$ almost everywhere. The [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) therefore yields

$$
\sum_n\int|K(x-y)e_n(y)|\,dy=\int|K(x-y)e(y)|\,dy<\infty.
$$

We may exchange the sum and integral; the resulting numerical series is absolutely convergent. Its [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\boxed{|T(e)(x)|\leq\sum_n|T(e_n)(x)|.}
$$

Here $e$ belongs to the stated operator domain, as is implicit when writing $T(e)$. Disjoint supports also ensure that each summand belongs to that domain.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Let $c$ be the center and $\ell$ the side length of $Q$. The zero integral of $f$ lets us subtract a constant kernel value:

$$
T(f)(x)=\int_Q\bigl[K(x-y)-K(x-c)\bigr]f(y)\,dy.
$$

Choose $L=4\sqrt d$. For $x$ outside the concentric [cube](../../../geometry-and-topology.md#cube) $\widehat Q$ of side length $L\ell$, and for $y\in Q$,

$$
|x-c|\geq\frac{L\ell}{2}=2\sqrt d\,\ell,
\qquad 2|y-c|\leq\sqrt d\,\ell.
$$

Thus the domain of integration in $x$ is contained in $\{|x-c|>2|y-c|\}$. After the translations $X=x-c$ and $Y=y-c$, the [Hörmander integral kernel condition](../../../fourier-analysis.md#hormander-integral-kernel-condition) gives

$$
\int_{\widehat Q^c}|K(x-y)-K(x-c)|\,dx\leq C.
$$

If $Y=0$ the difference is zero and the same inequality holds. Apply the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) to obtain the [cancellation estimate outside a dilated cube](../../../fourier-analysis.md#cancellation-estimate-outside-a-dilated-cube):

$$
\boxed{\int_{\widehat Q^c}|T(f)(x)|\,dx\leq C\int_Q|f(y)|\,dy=C\|f\|_1.}
$$

In particular the constant on the right is the same $C$ as in the hypothesis; only the dilation $L$ depends on the dimension.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

We derive the required [Calderón–Zygmund decomposition](../../../analysis.md#calderon-zygmund-decomposition) and apply the preceding two parts. Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$, and put $A=\|\widehat K\|_\infty$. The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) gives

$$
\|Tf\|_2\leq A\|f\|_2.
$$

For completeness this starts with smooth rapidly decreasing inputs, where $\widehat{K*f}=\widehat K\widehat f$, and extends by $L^2$ density. It agrees with the pointwise [convolution](../../../fourier-analysis.md#convolution) in the question: if $f_j\to f$ in $L^2$, then $\|K*(f_j-f)\|_\infty\leq\|K\|_2\|f_j-f\|_2$. Thus there is no need to assume that $K$ itself is integrable.

Fix $f\in L^1(\mathbb R^d)$, let $F=\|f\|_1$, and choose $\lambda>0$. Select the maximal dyadic [cubes](../../../geometry-and-topology.md#cube) $Q$ for which $|Q|^{-1}\int_Q|f|>\lambda$. They exist above every qualifying [cube](../../../geometry-and-topology.md#cube) because averages over increasingly large ancestors tend to zero. They are disjoint, their total volume is at most $F/\lambda$, and maximality gives

$$
\lambda<\frac1{|Q|}\int_Q|f|\leq2^d\lambda.
$$

Outside their union, dyadic differentiation gives $|f|\leq\lambda$ almost everywhere. One can obtain this differentiation fact from the allowed [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem): on each fixed dyadic [cube](../../../geometry-and-topology.md#cube) the averages are [conditional expectations](../../../measure-theory.md#conditional-expectation) of the integrable restriction, their almost-everywhere limit exists, and approximation by dyadic step functions shows in $L^1$ that this limit is $f$.

Let $f_Q=|Q|^{-1}\int_Qf$, define $g=f$ outside the selected [cubes](../../../geometry-and-topology.md#cube) and $g=f_Q$ on $Q$, and set $b_Q=(f-f_Q)\mathbf1_Q$. This constructs

$$
f=g+b,\qquad b=\sum_Qb_Q,\qquad \int b_Q=0,
$$

with the estimates

$$
\|g\|_\infty\leq2^d\lambda,\qquad \|g\|_1\leq F,\qquad
\|g\|_2^2\leq2^d\lambda F,\qquad \sum_Q\|b_Q\|_1\leq2F.
$$

These follow by integrating separately on each selected [cube](../../../geometry-and-topology.md#cube); $|f_Q||Q|\leq\int_Q|f|$ gives both the good-part [norm](../../../functional-analysis.md#norm) bound and the last cancellation-error bound.

Let $\Omega=\bigcup_Q\widehat Q$, with the dilation $L=4\sqrt d$ from part (ii). Then $|\Omega|\leq L^dF/\lambda$. On its complement, part (i), followed by part (ii), gives

$$
\int_{\Omega^c}|Tb|\leq\sum_Q\int_{\Omega^c}|Tb_Q|
\leq\sum_Q\int_{\widehat Q^c}|Tb_Q|\leq2CF.
$$

Finally, $|Tf|>\lambda$ implies $|Tg|>\lambda/2$ or $|Tb|>\lambda/2$. The first alternative is controlled by the $L^2$ operator bound, and the second by the last integral outside $\Omega$. Hence

$$
\begin{aligned}
|\{|Tf|>\lambda\}|
&\leq|\Omega|+\frac{4}{\lambda^2}\|Tg\|_2^2
+\frac{2}{\lambda}\int_{\Omega^c}|Tb|\\
&\leq\left(L^d+2^{d+2}A^2+4C\right)\frac{F}{\lambda}.
\end{aligned}
$$

Thus **$T$ has weak type $(1,1)$**, with a constant depending only on the dimension, the bounded [Fourier transform](../../../analysis.md#fourier-transform), and the [Hörmander integral kernel condition](../../../fourier-analysis.md#hormander-integral-kernel-condition).

## 5

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Put $M=\sup_{y>0}\int_{\mathbb R}|f(x+iy)|\,dx$. The goal is to obtain an integrable [non-tangential maximal function](../../../analysis.md#non-tangential-maximal-function) without assuming in advance that $f$ has an integrable boundary density. We use a square root to place the boundary data in $L^2$, where the [Hardy-Littlewood maximal function](../../../analysis.md#hardy-littlewood-maximal-function) is strongly bounded.

First recall this strong bound directly from Q2. For a nonnegative $h\in L^2(\mathbb R)$ and $\lambda>0$, split $h=h\mathbf1_{\{h>\lambda/2\}}+h\mathbf1_{\{h\leq\lambda/2\}}$. The second summand has centered maximal function at most $\lambda/2$; the first is in $L^1$. Q2's weak estimate, in dimension one, therefore gives

$$
|\{mh>\lambda\}|\leq\frac6\lambda\int_{\{h>\lambda/2\}}h.
$$

The [layer cake representation](../../../functional-analysis.md#layer-cake-representation) and [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) then imply

$$
\|mh\|_2^2=2\int_0^\infty\lambda|\{mh>\lambda\}|\,d\lambda
\leq12\int h(s)\int_0^{2h(s)}d\lambda\,ds=24\|h\|_2^2.
$$

This is the needed [Strong Lp bound for the Hardy-Littlewood maximal function](../../../analysis.md#strong-lp-bound-for-the-hardy-littlewood-maximal-function), with an explicit adequate constant.

For $\varepsilon>0$, let $f_\varepsilon(z)=f(z+i\varepsilon)$ and $h_\varepsilon(x)=|f(x+i\varepsilon)|^{1/2}$. Q1's elementary harmonic pointwise estimate makes $f_\varepsilon$ bounded on the closed upper half-plane. Its boundary value is continuous, and $\|h_\varepsilon\|_2^2\leq M$. The function $|f_\varepsilon|^{1/2}$ is [subharmonic](../../../partial-differential-equation.md#subharmonic-function): away from zeros, for any $q>0$,

$$
\Delta |f_\varepsilon|^q=q^2|f_\varepsilon|^{q-2}|f_\varepsilon'|^2\geq0,
$$

and regularization, or the submean inequality at zeros, extends this to the whole domain. Bounded subharmonic comparison with the [Poisson integral](../../../partial-differential-equation.md#poisson-integral) gives

$$
|f_\varepsilon(x'+iy)|^{1/2}\leq(P_y*h_\varepsilon)(x').
$$

Here $h_\varepsilon$ need not be in $L^1$. The [Poisson integral](../../../partial-differential-equation.md#poisson-integral) is nevertheless defined, since $h_\varepsilon\in L^2\cap L^\infty$ and $P_y\in L^1\cap L^2$, and it tends to its continuous boundary values. To justify comparison on this unbounded domain, the difference between the two sides is bounded above, subharmonic, and zero on the real boundary. On an upper half-disk of radius $R$, use the positive harmonic barrier

$$
b_R(z)=\frac{2R\operatorname{Im}z}{|R-z|^2}+\frac{2R\operatorname{Im}z}{|R+z|^2}.
$$

On its semicircular arc, $b_R(Re^{i\theta})=2/\sin\theta\geq2$, while $b_R(z)\to0$ for every fixed interior $z$ as $R\to\infty$. The [maximum principle for subharmonic functions](../../../partial-differential-equation.md#maximum-principle-for-subharmonic-functions), with a fixed bound for the difference, proves the comparison. The barrier's positive blow-up at the arc endpoints causes no difficulty.

For $|x-x'|\leq y$, the elementary inequality $y^2+|x-s|^2\leq3(y^2+|x'-s|^2)$ gives

$$
P_y(x'-s)\leq3P_y(x-s).
$$

Q2's [radial decreasing kernel domination by the maximal function](../../../analysis.md#radial-decreasing-kernel-domination-by-the-maximal-function) extends to nonnegative $L^2$ inputs by applying it to increasing bounded compactly supported truncations. Hence, taking the supremum over the cone,

$$
\bigl(f_\varepsilon^*(x)\bigr)^{1/2}\leq3m(h_\varepsilon)(x),\qquad
\int f_\varepsilon^*\leq9\|m(h_\varepsilon)\|_2^2\leq216M.
$$

For any fixed cone point, $f_\varepsilon(z)\to f(z)$ as $\varepsilon\downarrow0$. Therefore $f^*(x)\leq\liminf_{\varepsilon\downarrow0}f_\varepsilon^*(x)$; use a sequence of positive shifts and the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) to conclude

$$
\boxed{\int_{\mathbb R}f^*(x)\,dx\leq216\sup_{y>0}\int_{\mathbb R}|f(x+iy)|\,dx<\infty.}
$$

The precise numerical constant is unimportant. Suprema over countable dense sets of cone points give the same values, so the maximal functions used here are measurable.

This yields boundary [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) rather than assuming it. The [holomorphic function](../../../complex-analysis.md#holomorphic-function) $f$ is a complex-valued [harmonic function](../../../partial-differential-equation.md#harmonic-function), so Q1 represents it as $f(x+iy)=P_y*\mu(x)$ for a finite complex measure $\mu$, with $f(\cdot+iy)\,dx\to\mu$ weak-star. Since $|f(x+iy)|\leq f^*(x)$, every compactly supported continuous $\psi$ satisfies

$$
\left|\int\psi\,d\mu\right|\leq\int|\psi(x)|f^*(x)\,dx.
$$

The dual characterization of the [total variation measure](../../../measure-theory.md#variation-measure) implies $|\mu|\leq f^*\,dx$, so the [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem) gives $\mu=F\,dx$ with $F\in L^1$. The [approximate identity](../../../fourier-analysis.md#approximate-identity) now gives $f(\cdot+iy)\to F$ in the [L1 norm](../../../functional-analysis.md#l1-norm) and [almost everywhere](../../../measure-theory.md#almost-everywhere). Thus the analytic [Hardy space](../../../analysis.md#hardy-space) has an integrable boundary function, unlike the unrestricted harmonic $h^1$ space.

In the real-line form of the [F. and M. Riesz theorem](../../../analysis.md#f-and-m-riesz-theorem), start with a finite complex measure whose [Fourier transform of a finite measure](../../../analysis.md#fourier-transform-of-a-finite-measure) vanishes for $\xi<0$. Its [Poisson integral](../../../partial-differential-equation.md#poisson-integral) is holomorphic: the transformed operators $\partial_y$ and $i\partial_x$ act by $-|\xi|$ and $-\xi$, which agree on that spectrum. These identities can first be read as distributional identities and then classically, since the [Poisson integral](../../../partial-differential-equation.md#poisson-integral) is smooth. Its harmonic $h^1$ [norm](../../../functional-analysis.md#norm) is finite by Q1, so the preceding argument makes the measure absolutely continuous. **A one-sided Fourier spectrum forces a finite boundary measure to have a Lebesgue density.**

For the customary circle form, normalize arc length by $dm=d\theta/(2\pi)$. If $\widehat\mu(n)=\int e^{-in\theta}\,d\mu(\theta)=0$ for $n<0$, then

$$
F(w)=\sum_{n\geq0}\widehat\mu(n)w^n,\qquad |w|<1,
$$

is analytic and $F(re^{i\theta})$ is the [Poisson integral on the unit disk](../../../partial-differential-equation.md#poisson-integral-on-the-unit-disk) of $\mu$. Positivity and unit mass of the [Poisson kernel on the circle](../../../partial-differential-equation.md#poisson-kernel-on-the-circle) imply $\sup_r\int|F(re^{i\theta})|\,dm\leq\|\mu\|_{\mathrm{TV}}$. The same square-root argument on the disk gives an integrable radial maximum, as follows. For $0<\rho<1$, put $h_\rho(\theta)=|F(\rho e^{i\theta})|^{1/2}$. The [maximum principle for subharmonic functions](../../../partial-differential-equation.md#maximum-principle-for-subharmonic-functions) on the disk gives

$$
|F(\rho r e^{i\theta})|^{1/2}\leq(P_r*h_\rho)(\theta).
$$

The supremum of these [Poisson integrals](../../../partial-differential-equation.md#poisson-integral) is bounded by a constant times the circular [Hardy-Littlewood maximal function](../../../analysis.md#hardy-littlewood-maximal-function). Indeed, for $r\geq1/2$ the circular kernel is bounded by a constant times $(1-r)/((1-r)^2+\theta^2)$ for $|\theta|\leq\pi$; splitting into arcs of radii $2^j(1-r)$ gives a summable geometric series of arc averages. For $r<1/2$ the kernel is uniformly bounded, and the whole-circle average suffices. The covering proof and the truncation argument already used on the line give the strong $L^2$ maximal bound for arcs on the circle as well. Thus

$$
\int\sup_{0<r<1}|F(\rho r e^{i\theta})|\,dm
\leq C\|h_\rho\|_2^2\leq C\|\mu\|_{\mathrm{TV}}.
$$

Let $\rho\uparrow1$ and apply [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) to obtain an integrable radial maximum $R(\theta)=\sup_{0<r<1}|F(re^{i\theta})|$. The measures $F(re^{i\theta})\,dm$ tend weak-star to $\mu$ and are dominated in magnitude by $R\,dm$. The same continuous-test-function argument gives $|\mu|\leq R\,dm$. This proves **the F. and M. Riesz theorem: a finite complex measure on the circle with all negative Fourier coefficients zero is absolutely continuous with respect to arc length**. Reversing the Fourier convention interchanges positive and negative indices.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
