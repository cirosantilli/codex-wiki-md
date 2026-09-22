# Paper 105

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_105.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_105.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a constant-coefficient differential operator $P(D)=\sum_{|\beta|\leq m}a_\beta D^\beta$, a hypersurface with nonzero normal covector $\nu$ is a [non-characteristic hypersurface](../../../partial-differential-equation.md#non-characteristic-hypersurface) precisely when its [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) $P_m(\nu)=\sum_{|\beta|=m}a_\beta\nu^\beta$ is nonzero. Multiplying the symbol by the conventional factor $i^m$ does not affect this criterion. For the initial line here the normal is $(0,1)$.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

**Characteristic.** The third-order [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) of $\partial_t-\partial_x^3$ is $-\nu_x^3$. The initial line has normal $(\nu_x,\nu_t)=(0,1)$, on which this symbol vanishes. Its evolution form does not make it non-characteristic in the ordinary total-order definition.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

**Characteristic.** The second-order [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) of $i\partial_t+\partial_x^2$ is $\nu_x^2$, which vanishes on the normal $(0,1)$. This uses total differential order, rather than an anisotropic convention that assigns different weights to time and space derivatives.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

**Non-characteristic.** The first-order [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) is $\nu_t-i\nu_x$, which equals one on $(0,1)$.

Set $z=x+it$. The equation is equivalent to $\partial_{\bar z}\phi=(\phi_x+i\phi_t)/2=0$. Because $\phi$ is continuously differentiable, the [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) imply that it is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) of $z$. Its convergent complex [Taylor series](../../../calculus.md#taylor-series) restricts to a real [power series](../../../real-analysis.md#power-series) along $t=0$, so $g$ is a [real analytic function](../../../analysis.md#real-analytic-function).

For [smooth-data instability of the Cauchy-Riemann Cauchy problem](../../../analysis.md#smooth-data-instability-of-the-cauchy-riemann-cauchy-problem), choose

$$
\boxed{\phi_n(x,t)=e^{-\sqrt n}\cos(n(x+it)).}
$$

These are [entire functions](../../../complex-analysis.md#entire-function) and satisfy the equation. Their initial [derivatives](../../../calculus.md#derivative) obey $\sup_x|\partial_x^jg_n|\leq n^j e^{-\sqrt n}$, so every finite sum tends to zero. But

$$
\sup_{x\in\mathbb R}|\phi_n(x,t)|=e^{-\sqrt n}\cosh(n|t|)\longrightarrow\infty\qquad(t\ne0).
$$

Thus analytic solutions can exist while [continuous dependence on initial data](../../../partial-differential-equation.md#continuous-dependence-on-initial-data) fails for this smooth-data topology.

The [Cauchy estimate](../../../analysis.md#cauchy-estimate) follows directly from the differentiated [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula):

$$
f^{(j)}(z_0)=\frac{j!}{2\pi i}\int_{|z-z_0|=r}\frac{f(z)}{(z-z_0)^{j+1}}\,dz,
\qquad
\boxed{|f^{(j)}(z_0)|\leq\frac{j!M}{r^j}.}
$$

The circle has length $2\pi r$, giving the bound for every integer $j\geq0$.

Put $w=\phi-\psi$ and integrate on the straight segment $z=\tau t/|t|$. For fixed $|x|<sR$, a disc centred at $x$ with radius approaching $R(\sigma(\tau)-s)$ stays inside $|\xi|\leq\sigma(\tau)R$. Applying the first-derivative [Cauchy estimate](../../../analysis.md#cauchy-estimate) there gives

$$
|w_x(x,z)|\leq\frac{\sup_{|\xi|\leq\sigma(\tau)R,\;|\zeta|\leq\tau}|w(\xi,\zeta)|}{R(\sigma(\tau)-s)}.
$$

Integrating its modulus and taking the supremum over $|x|<sR$ is exactly the asserted integral estimate. The source cancels from $T\phi-T\psi$.

To obtain a [contraction mapping](../../../analysis.md#contraction-mapping), use the [weighted holomorphic norm on a shrinking time domain](../../../complex-analysis.md#weighted-holomorphic-norm-on-a-shrinking-time-domain). Its finite-norm space consists of holomorphic functions on $\mathcal C_\alpha$ with zero initial value; the apparent quotient at $t=0$ is interpreted by a limit. Completeness follows because convergence in this norm implies [locally uniform convergence of holomorphic functions](../../../complex-analysis.md#locally-uniform-convergence-of-holomorphic-functions), including near $t=0$, and the limiting pointwise bounds give convergence in the norm.

Here is the explicit [contraction estimate on a shrinking holomorphic domain](../../../complex-analysis.md#contraction-estimate-on-a-shrinking-holomorphic-domain). Write $N=\|w\|_\alpha$, $r=|t|$, $A=\alpha(1-s)$, and choose

$$
\sigma(\tau)=s+\frac{A-\tau}{2\alpha}\qquad(0\leq\tau\leq r<A).
$$

Then $\sigma-s=(A-\tau)/(2\alpha)$ and $\alpha(1-\sigma)-\tau=(A-\tau)/2$. The whole auxiliary polydisc lies inside $\mathcal C_\alpha$, and its supremum of $|w|$ is at most $2N\tau/(A-\tau)$. Consequently

$$
\begin{aligned}
\frac{A-r}{r}|T\phi-T\psi|
&\leq\frac{4\alpha N}{R}\frac{A-r}{r}\int_0^r\frac{\tau}{(A-\tau)^2}\,d\tau\\
&=\frac{4\alpha N}{R}\left[1+\frac{A-r}{r}\log(1-r/A)\right]
\leq\frac{4\alpha N}{R}.
\end{aligned}
$$

Thus $\|T\phi-T\psi\|_\alpha\leq(4\alpha/R)\|\phi-\psi\|_\alpha$. Choose $0<\alpha<\min(\eta,R/4)$. The source is bounded on the closed polydisc, say by $M_f$, and $\|T0\|_\alpha\leq\alpha M_f$. Therefore $T$ maps the [Banach space](../../../banach-space.md) into itself and is a strict [contraction mapping](../../../analysis.md#contraction-mapping). The [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) gives a holomorphic fixed point with $\phi(x,0)=0$. Differentiating the integral identity yields $\phi_t-i\phi_x=f$, establishing this case of the [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem).

Finally, near each real initial point, a [real analytic function](../../../analysis.md#real-analytic-function) $g$ has a holomorphic extension $G$. Apply the same construction to $\phi=G(x)+v$ with $v(x,0)=0$ and source $iG'(x)$, restricting the discs if necessary. This gives a local [real analytic function](../../../analysis.md#real-analytic-function) of $(x,t)$ with the prescribed initial value. Equivalently the solution is $\boxed{\phi(x,t)=G(x+it)}$ wherever the extension is defined.

## 2

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an integer $s\geq0$, the [Sobolev space](../../../sobolev-space.md) is

$$
W^{s,p}(\mathbb R^d)=\{u\in L^p:D^\beta u\in L^p\text{ for every multi-index }|\beta|\leq s\},
$$

where $D^\beta$ is a [weak derivative](../../../distribution-theory.md#weak-derivative). For $p<\infty$ one may use the [Sobolev norm](../../../sobolev-space.md#sobolev-norm) $(\sum_{|\beta|\leq s}\|D^\beta u\|_p^p)^{1/p}$; for $p=\infty$ use the maximum of the finitely many essential-supremum norms.

For $1\leq p<d$, the [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) is $\|u\|_{p^*}\leq C_{d,p}\|\nabla u\|_p$, with [Sobolev conjugate exponent](../../../sobolev-space.md#sobolev-conjugate-exponent) $p^*=dp/(d-p)$. For $d<p<\infty$, [Morrey's inequality](../../../sobolev-space.md#morrey-s-inequality) supplies a continuous representative satisfying

$$
|u(x)-u(y)|\leq C_{d,p}|x-y|^{1-d/p}\|\nabla u\|_p,
\qquad
\|u\|_\infty\leq C_{d,p}(\|u\|_p+\|\nabla u\|_p).
$$

At $p=\infty$ the representative is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). At the critical exponent $p=d>1$, first-order Sobolev regularity gives every finite $L^q$ embedding for $q\geq d$, with an inhomogeneous norm, but generally no $L^\infty$ embedding. The one-dimensional endpoint $W^{1,1}(\mathbb R)\hookrightarrow L^\infty(\mathbb R)$ is an exception.

For the proof of [Morrey's inequality](../../../sobolev-space.md#morrey-s-inequality), start with a smooth $u$ and write $u_{B(x,r)}$ for its average on a ball. Averaging the [fundamental theorem of calculus along a line segment](../../../calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) and changing radial variables gives

$$
|u(x)-u_{B(x,r)}|
\leq C_d\int_{B(x,r)}\frac{|\nabla u(z)|}{|x-z|^{d-1}}\,dz
\leq C_{d,p}r^{1-d/p}\|\nabla u\|_p.
$$

The last step is the [Holder inequality](../../../functional-analysis.md#holder-inequality); integrability of the kernel to power $p'$ is exactly $(d-1)p'<d$. For $r=|x-y|$, translate the averaging ball along the segment from $x$ to $y$. The [fundamental theorem of calculus along a line segment](../../../calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) and the [Holder inequality](../../../functional-analysis.md#holder-inequality) give

$$
|u_{B(x,r)}-u_{B(y,r)}|\leq r|B_r|^{-1/p}\|\nabla u\|_p.
$$

Combining the two point-to-average bounds and this average-to-average bound proves the required Hölder estimate. The point-to-average bound with $r=1$, together with $|u_{B(x,1)}|\leq|B_1|^{-1/p}\|u\|_p$, gives the supremum estimate. [Density of smooth functions in a Sobolev space](../../../sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space) then gives a uniformly convergent sequence of smooth representatives, preserving both bounds. For $p=\infty$, mollification gives the Lipschitz version.

For the decay conclusion assume $d<p<\infty$. The representative is uniformly continuous. If $|u(x_j)|\geq2\theta>0$ along points escaping to infinity, the Hölder bound gives a radius $\rho>0$, independent of $j$, on which $|u|\geq\theta$. A subsequence has disjoint radius-$\rho$ balls, each contributing at least $\theta^p|B_\rho|$ to $\|u\|_p^p$, a contradiction. This is [uniformly continuous integrable functions vanish at infinity](../../../topological-analysis.md#uniformly-continuous-integrable-functions-vanish-at-infinity).

**The finite-$p$ restriction is necessary.** If the printed range includes $p=\infty$, its decay assertion is false: $u\equiv1$ belongs to $W^{1,\infty}$ but does not tend to zero.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) says that a uniformly bounded, equicontinuous family of continuous functions on a compact metric space is relatively compact in the uniform norm. Thus every sequence in that family has a uniformly convergent subsequence, and its limit is continuous.

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

On a bounded Lipschitz domain $\Omega\subset\mathbb R^d$, the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) states that $W^{1,p}(\Omega)\hookrightarrow L^q(\Omega)$ is compact for $1\leq p<\infty$ and

$$
\frac1q>\frac1p-\frac1d,
$$

with $1/q=0$ for $q=\infty$. Thus $q<p^*$ when $p<d$, every finite $q$ is allowed when $p=d$, and the embedding into continuous functions with their uniform norm is compact when $p>d$.

For the main proof, a [Sobolev extension operator](../../../sobolev-space.md#sobolev-extension-operator) puts a bounded sequence into a common compactly supported region of $\mathbb R^d$. The [Sobolev fundamental theorem of calculus on lines](../../../sobolev-space.md#sobolev-fundamental-theorem-of-calculus-on-lines) gives the uniform translation estimate $\|u(\cdot+h)-u\|_p\leq|h|\|\nabla u\|_p$. Convolution with a [mollifier](../../../distribution-theory.md#mollifier) therefore approximates the sequence uniformly in [Lp space](../../../measure-theory.md#lp-space). At any fixed smoothing scale, its derivatives and supremum are uniformly bounded, so the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) gives a convergent subsequence. A diagonal choice and the uniform approximation give strong [Lp space](../../../measure-theory.md#lp-space) convergence. The finite measure of $\Omega$ handles $q<p$, while [Lp interpolation inequality](../../../measure-theory.md#lp-interpolation-inequality) with the bounded Sobolev embeddings upgrades this to the larger subcritical finite [Lp spaces](../../../measure-theory.md#lp-space); for $p>d$, [Morrey's inequality](../../../sobolev-space.md#morrey-s-inequality) gives uniform equicontinuity directly and the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) gives uniform convergence. Boundedness of the domain is essential.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Choose continuous representatives using [Morrey's inequality](../../../sobolev-space.md#morrey-s-inequality). On the closed unit ball they are uniformly bounded by $C M$ and satisfy

$$
|u_n(x)-u_n(y)|\leq CM|x-y|^{1-d/p}.
$$

The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) therefore gives a uniformly convergent subsequence with a continuous limit. For $p=\infty$, use the uniform Lipschitz estimate instead; this part remains valid at that endpoint.

For [weak lower semicontinuity of the Hilbert norm](../../../hilbert-space.md#weak-lower-semicontinuity-of-the-hilbert-norm), weak convergence gives $\langle u_n-\phi,\phi\rangle\to0$, and hence

$$
\|u_n\|^2=\|\phi\|^2+\|u_n-\phi\|^2+o(1).
$$

Taking the lower limit proves $\boxed{\|\phi\|\leq\liminf_n\|u_n\|}$.

For the nonlinear integral, use [local Sobolev compactness gives lower semicontinuity of a nonnegative integral](../../../functional-analysis.md#local-sobolev-compactness-gives-lower-semicontinuity-of-a-nonnegative-integral). Select a subsequence attaining the lower limit of the integrals. The [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) on successively larger balls gives a diagonal subsequence converging strongly in local [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) to $\phi$. After a further subsequence it converges almost everywhere. Since $1-\cos s\geq0$, the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) gives

$$
\boxed{\int_{\mathbb R^3}(1-\cos\phi)\,dx\leq\liminf_n\int_{\mathbb R^3}(1-\cos u_n)\,dx.}
$$

Each integral is finite because $0\leq1-\cos s\leq s^2/2$. The argument uses local compactness rather than convexity: $1-\cos s$ is not a convex function on the whole real line.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Work with real-valued functions. The [screened sine-Gordon energy](../../../calculus-of-variations.md#screened-sine-gordon-energy) is well defined: $0\leq1-\cos u\leq u^2/2$, and $fu$ is integrable by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). It is coercive, because

$$
E[u]\geq\tfrac12\|u\|_{H^1}^2-\|f\|_2\|u\|_2
\geq\tfrac14\|u\|_{H^1}^2-\|f\|_2^2.
$$

A minimizing sequence is bounded in the [Hilbert space](../../../hilbert-space.md) $H^1$. [Weak sequential compactness of bounded sequences in a reflexive Banach space](../../../functional-analysis.md#weak-sequential-compactness-of-bounded-sequences-in-a-reflexive-banach-space) supplies a weakly convergent subsequence. The squared [H1 space](../../../sobolev-space.md#h1-space) norm is weakly lower semicontinuous, the source pairing is weakly continuous, and the nonlinear term is covered by [local Sobolev compactness gives lower semicontinuity of a nonnegative integral](../../../functional-analysis.md#local-sobolev-compactness-gives-lower-semicontinuity-of-a-nonnegative-integral). The [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) therefore gives a minimizer $\phi$.

Taking its [first variation](../../../calculus-of-variations.md#first-variation) in any $v\in H^1$ gives

$$
\int_{\mathbb R^3}\nabla\phi\cdot\nabla v+\phi v+\sin\phi\,v\,dx
=\int_{\mathbb R^3}fv\,dx.
$$

Thus the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
\boxed{-\Delta\phi+\phi+\sin\phi=f,}
$$

as a [weak solution](../../../partial-differential-equation.md#weak-solution), equivalently in [distributions](../../../distribution-theory.md#distribution-mathematical-analysis) when tested against smooth compactly supported functions. The derivative of the nonlinear term is justified by $|\sin\phi|\leq|\phi|$ and the second-order remainder bound $|\cos|\leq1$.

Now $G=f-\sin\phi\in L^2$, so the supplied [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) estimate puts $\phi$ in $H^2$. Applying the [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) to $\phi$ and each first [weak derivative](../../../distribution-theory.md#weak-derivative) gives $\phi\in W^{1,6}(\mathbb R^3)$. [Morrey's inequality](../../../sobolev-space.md#morrey-s-inequality) and [uniformly continuous integrable functions vanish at infinity](../../../topological-analysis.md#uniformly-continuous-integrable-functions-vanish-at-infinity) prove that its continuous representative tends to zero.

**The final printed supremum estimate is false in general.** The [maximum bound for a monotone reaction term](../../../elliptic-boundary-value-problem.md#maximum-bound-for-a-monotone-reaction-term) involves $h(s)=s+\sin s$, which is odd and strictly increasing: $h'=1+\cos s\geq0$, and its zeros are isolated. If $M=\|f\|_\infty<\infty$, a positive maximum $m$ of $\phi$ satisfies $h(m)\leq f\leq M$; apply the same argument to $-\phi$. The valid general estimate is

$$
\boxed{\|\phi\|_\infty\leq h^{-1}(M)\leq M+1.}
$$

The bound by $M$ is valid if $M\leq\pi$, but $h(s)$ can be smaller than $s$ for larger positive $s$.

For an explicit [failure of the source-size bound for the screened sine-Gordon equation](../../../calculus-of-variations.md#failure-of-the-source-size-bound-for-the-screened-sine-gordon-equation), take $a=3\pi/2$, $L=10$, $\phi(x)=a e^{-|x|^2/L^2}$ and $f=-\Delta\phi+\phi+\sin\phi$. These are smooth functions in the required spaces. With $q=|x|^2/L^2$,

$$
|\Delta\phi|=\frac{a}{L^2}|4q-6|e^{-q}\leq\frac{6a}{L^2},
\qquad
0\leq h(\phi)\leq h(a)=a-1.
$$

Hence $\|f\|_\infty\leq a-1+6a/L^2<a=\|\phi\|_\infty$. Moreover $V(s)=s^2/2+1-\cos s$ has $V''=1+\cos s\geq0$, so the energy is convex and this critical point is a minimizer. The example therefore satisfies even the minimizing and $C^2$ hypotheses of the printed claim.

## 3

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [contraction semigroup](../../../functional-analysis.md#contraction-semigroup) on a [Banach space](../../../banach-space.md) $X$ consists of bounded linear operators $S(t)$ with $S(0)=I$, $S(t+s)=S(t)S(s)$, $\|S(t)\|\leq1$, and $S(t)x\to x$ as $t\downarrow0$ for each $x\in X$. Its [infinitesimal generator of a semigroup](../../../functional-analysis.md#infinitesimal-generator-of-a-semigroup) is

$$
D(A)=\left\{x:\lim_{h\downarrow0}\frac{S(h)x-x}{h}\text{ exists in }X\right\},
\qquad
Ax=\lim_{h\downarrow0}\frac{S(h)x-x}{h}.
$$

For density, [Yosida averaging of a semigroup](../../../functional-analysis.md#yosida-averaging-of-a-semigroup) gives $x_h=h^{-1}\int_0^hS(s)x\,ds$. Taking the difference quotient of this [Bochner integral](../../../measure-theory.md#bochner-integral) shows that $x_h\in D(A)$ and $Ax_h=(S(h)x-x)/h$. Strong continuity gives $x_h\to x$, so $D(A)$ is dense.

For closedness, the [semigroup restricted to its generator domain](../../../functional-analysis.md#semigroup-restricted-to-its-generator-domain) satisfies

$$
S(t)x-x=\int_0^tS(s)Ax\,ds\qquad(x\in D(A)).
$$

If $x_n\to x$ and $Ax_n\to y$, pass to the limit in this identity. After dividing by $t$, strong continuity gives $(S(t)x-x)/t\to y$. Hence $x\in D(A)$ and $Ax=y$. This proves [generator of a strongly continuous semigroup is closed and densely defined](../../../functional-analysis.md#generator-of-a-strongly-continuous-semigroup-is-closed-and-densely-defined).

The contraction form of the [Hille-Yosida theorem](../../../functional-analysis.md#hille-yosida-theorem) states that a linear operator $A$ generates a [contraction semigroup](../../../functional-analysis.md#contraction-semigroup) if and only if it is densely defined and closed, every real $\lambda>0$ lies in its [resolvent set](../../../functional-analysis.md#resolvent-set-of-an-operator), and

$$
\|(\lambda-A)^{-n}\|\leq\lambda^{-n}\qquad(n\geq1).
$$

Here the $n=1$ bound implies the others by taking powers of the same bounded [resolvent](../../../functional-analysis.md#resolvent-of-an-operator).

The [H1 space](../../../sobolev-space.md#h1-space) is $H^1(\mathbb R)=\{u\in L^2:u'\in L^2\}$ with [weak derivative](../../../distribution-theory.md#weak-derivative) $u'$ and squared norm $\|u\|_2^2+\|u'\|_2^2$. The displayed weighted space is the [one-dimensional harmonic oscillator form domain](../../../quantum-mechanics.md#one-dimensional-harmonic-oscillator-form-domain), with inner product

$$
\langle u,v\rangle_X=\int_{\mathbb R}u\bar v+u'\overline{v'}+x^2u\bar v\,dx.
$$

If $u_n$ is Cauchy in $X$, it converges in $H^1$ to $u$, and $xu_n$ converges in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) to some $w$. On each bounded interval, multiplication by $x$ is bounded, so $w=xu$ there. Thus $xu\in L^2$ and convergence holds in $X$, proving completeness and the [Hilbert space](../../../hilbert-space.md) property. Equivalently this is closedness of the [multiplication operator](../../../vector-space.md#multiplication-operator) by $x$.

For the [Sobolev characterization by bounded difference quotients](../../../sobolev-space.md#sobolev-characterization-by-bounded-difference-quotients), if $f\in H^1$ then

$$
D_hf=\int_0^1f'(\cdot+\theta h)\,d\theta,
\qquad
\|D_hf\|_2\leq\|f'\|_2,
\qquad
D_hf\longrightarrow f'\text{ in }L^2.
$$

The last assertion uses continuity of [translation of a function](../../../function.md#translation-of-a-function) in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). Conversely, if $f\in L^2$ and the quotients are uniformly bounded for $0<|h|<1$, take a weakly convergent subsequence as $h\to0$. For every [test function](../../../distribution-theory.md#test-function) $v$,

$$
\int D_hf\,v\,dx=\int f(x)\frac{v(x-h)-v(x)}h\,dx\longrightarrow-\int f v'\,dx.
$$

The weak limit is therefore the [weak derivative](../../../distribution-theory.md#weak-derivative) $f'\in L^2$. This proves the characterization.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $B=-A=-\partial_x^2+1+x^2$. Smooth compactly supported functions lie in $D(A)$ and are dense in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space), so $A$ is densely defined.

For $\lambda>0$, use the form

$$
a_\lambda(u,v)=\int_{\mathbb R}u'\overline{v'}+(1+\lambda+x^2)u\bar v\,dx
$$

on the [one-dimensional harmonic oscillator form domain](../../../quantum-mechanics.md#one-dimensional-harmonic-oscillator-form-domain) $X$. It is bounded and coercive in the $X$ norm. The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) gives a unique $u\in X$ satisfying $a_\lambda(u,v)=\langle g,v\rangle$ for every $v\in X$. Thus $-u''+(1+\lambda+x^2)u=g$ in [distributions](../../../distribution-theory.md#distribution-mathematical-analysis).

We must verify the full specified [operator domain](../../../vector-space.md#operator-domain), not just the form domain. The equation first gives $u\in H^2_{\mathrm{loc}}$. For compactly supported $H^2$ functions, [integration by parts](../../../calculus.md#integration-by-parts) gives the [graph estimate for the harmonic oscillator](../../../quantum-mechanics.md#graph-estimate-for-the-harmonic-oscillator), obtained from

$$
\begin{aligned}
\|-v''+(1+\lambda+x^2)v\|_2^2
={}&\|v''\|_2^2+\|(1+\lambda+x^2)v\|_2^2\\
&+2\int(1+\lambda+x^2)|v'|^2\,dx-2\|v\|_2^2.
\end{aligned}
$$

Apply this to $v=\chi_Ru$, with $\chi_R=1$ on $[-R,R]$, supported in $[-2R,2R]$, and derivatives bounded by $C/R$ and $C/R^2$. Its right-hand source is $\chi_Rg-2\chi_R'u'-\chi_R''u$, uniformly bounded in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). The estimate and the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) give $x^2u\in L^2$; the original equation then gives $u''\in L^2$, and hence $u\in H^2$. Thus $u\in D(A)$, proving that $\lambda-A$ is onto. The energy identity proves injectivity and the [resolvent of the shifted harmonic oscillator](../../../quantum-mechanics.md#resolvent-of-the-shifted-harmonic-oscillator) estimate

$$
(1+\lambda)\|u\|_2^2\leq a_\lambda(u,u)=\operatorname{Re}\langle g,u\rangle
\leq\|g\|_2\|u\|_2,
\qquad
\boxed{\|(\lambda-A)^{-1}\|_{2\to2}\leq\frac1{1+\lambda}.}
$$

To prove closedness, suppose $u_n\to u$ and $Au_n\to v$ in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). For one fixed $\lambda>0$,

$$
u_n=(\lambda-A)^{-1}(\lambda u_n-Au_n)\longrightarrow(\lambda-A)^{-1}(\lambda u-v).
$$

Therefore $u$ belongs to the range of the resolvent, namely $D(A)$, and $Au=v$.

All hypotheses of the [Hille-Yosida theorem](../../../functional-analysis.md#hille-yosida-theorem) now hold; the resolvent bound is stronger than $1/\lambda$. Let $S(t)$ be its [contraction semigroup](../../../functional-analysis.md#contraction-semigroup). The [exponentially shifted semigroup](../../../functional-analysis.md#exponentially-shifted-semigroup)

$$
\boxed{\psi(t)=e^tS(t)\psi_0}
$$

has generator $A+I=\partial_x^2-x^2$. It is continuous in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space), takes the initial value $\psi_0$, and satisfies $\boxed{\|\psi(t)\|_2\leq e^t\|\psi_0\|_2}$. For $\psi_0\in D(A)$, its time derivative exists in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) and equals $(A+I)\psi(t)$, so the equation holds as a strong [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) solution. For general initial data it is the semigroup solution, without an unproved pointwise differentiability claim.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
