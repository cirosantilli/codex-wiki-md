# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper24.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write the [predictable sigma-algebra](../../../martingale.md#predictable-sigma-algebra) on positive times as

$$
\mathcal P=\sigma\{B\times(s,t]:0\leq s<t<\infty,\ B\in\mathcal F_s\}.
$$

It is equivalently the smallest [sigma-algebra](../../../measure-theory.md#sigma-algebra) making all left-continuous [adapted processes](../../../stochastic-process.md#adapted-process) measurable. Indeed, the indicator of each generating rectangle is left-continuous and adapted, and approximating any left-continuous [adapted process](../../../stochastic-process.md#adapted-process) by its values at the preceding points of deterministic partitions gives the reverse inclusion. **Previsibility records information available immediately before observation.** If time zero is included, add $B\times\{0\}$ with $B\in\mathcal F_0$. The displayed description in part (b) uses positive times, as indicated by its product space.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Observing $X_s$ reveals exactly whether $\omega<s$. Thus the [natural filtration](../../../stochastic-process.md#natural-filtration) is

$$
\mathcal F_t=\sigma\{(0,s):0\leq s\leq t\}.
$$

Every generating [set](../../../set.md) either contains the entire tail $[t,\infty)$ or avoids it, so this tail remains one indistinguishable atom. Conversely, these initial intervals generate the full relative [Borel sigma-algebra](../../../measure-theory.md#borel-sigma-algebra) on $(0,t)$: use rational endpoints below $t$, together with $(0,t)$ itself. Therefore every [Borel set](../../../measure-theory.md#borel-set) contained in $(0,t)$, and its complement, belongs to $\mathcal F_t$. We obtain

$$
\boxed{\mathcal F_t=\{B\in\mathcal F:B\subseteq(0,t)\ \text{or}\ B^c\subseteq(0,t)\}.}
$$

The strict endpoint is essential: the value at $\omega=t$ is still $X_t=1$, so it cannot be distinguished from a later lifetime.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $D=\{(\omega,t):\omega\geq t\}$ and let $\mathcal C$ denote the proposed family of [sets](../../../set.md). This is a [sigma-algebra](../../../measure-theory.md#sigma-algebra): complements replace $T$ and $A$ by their complements, and countable unions replace them by their unions. For a generating [predictable rectangle](../../../martingale.md#predictable-rectangle) $B\times(s,u]$, part (a) says either $B\subseteq(0,s)$ or $B^c\subseteq(0,s)$. In the first case its trace on $D$ is empty; in the second it is exactly $D\cap(\Omega\times(s,u])$. Its trace on $D^c$ is always product-Borel. Hence $\mathcal P\subseteq\mathcal C$.

For the reverse inclusion, $X$ is left-continuous and adapted, so $D=\{X=1\}$ belongs to the [predictable sigma-algebra](../../../martingale.md#predictable-sigma-algebra). Every deterministic [Borel set](../../../measure-theory.md#borel-set) in time also belongs to that [sigma-algebra](../../../measure-theory.md#sigma-algebra), hence $D\cap(\Omega\times T)$ is predictable. For a product rectangle $E\times T$,

$$
(E\times T)\cap D^c=\bigcup_{s\in\mathbb Q_{>0}}\bigl((E\cap(0,s))\times(s,\infty)\bigr)\cap(\Omega\times T).
$$

Each term is predictable because $E\cap(0,s)\in\mathcal F_s$. Every pair with $\omega<t$ lies in such a term by choosing $\omega<s<t$. The class of product-Borel [sets](../../../set.md) $A$ for which $A\cap D^c$ is predictable is a [sigma-algebra](../../../measure-theory.md#sigma-algebra) containing the product rectangles, so it contains $\mathcal F\otimes\mathcal F$. Thus

$$
\boxed{\mathcal P=\{(D\cap(\Omega\times T))\cup(D^c\cap A):T\in\mathcal F,\ A\in\mathcal F\otimes\mathcal F\}.}
$$

This [survival-observation predictable sigma-algebra](../../../martingale.md#survival-observation-predictable-sigma-algebra) expresses a sharp distinction: before and at the lifetime the only observable coordinate is time, whereas strictly after it the lifetime is known.

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [simple predictable process](../../../martingale.md#simple-predictable-process), define its [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) by

$$
(H\mathbin\cdot M)_t=\sum_{k=0}^{n-1}Z_{t_k}\bigl(M_{t\wedge t_{k+1}}-M_{t\wedge t_k}\bigr).
$$

Common refinement of the deterministic partitions makes this definition independent of the representation. Each summand is a [martingale](../../../martingale.md) increment multiplied by information already available at its left endpoint, so the resulting process is a continuous square-integrable [martingale](../../../martingale.md) starting at zero. Its terminal value is the same sum with $t$ replaced by $t_n$.

Write $\Delta_kM=M_{t_{k+1}}-M_{t_k}$. If $j<k$, then $Z_{t_j}\Delta_jM\,Z_{t_k}$ is $\mathcal F_{t_k}$-measurable. By the [conditional expectation](../../../measure-theory.md#conditional-expectation) identity for increments of a [martingale](../../../martingale.md),

$$
\mathbb E[Z_{t_j}\Delta_jM\,Z_{t_k}\Delta_kM]=0.
$$

The [conditional bracket isometry for stopped martingale increments](../../../stochastic-calculus.md#conditional-bracket-isometry-for-stopped-martingale-increments) gives

$$
\mathbb E[(\Delta_kM)^2\mid\mathcal F_{t_k}]
=\mathbb E([M]_{t_{k+1}}-[M]_{t_k}\mid\mathcal F_{t_k}).
$$

For completeness, this identity follows by applying the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) to $M$ and $M^2-[M]$ and expanding the square. The latter process is a true uniformly integrable [martingale](../../../martingale.md) here: the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) bounds $\mathbb E\sup_t|M_t|^2$, stopped square identities and [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma) give $\mathbb E[M]_\infty<\infty$, and its absolute supremum is bounded by $\sup_t|M_t|^2+[M]_\infty$. Consequently all the stopped identities pass to the limit.

Multiplying the conditional identity by $Z_{t_k}^2$, taking [expectations](../../../probability-theory.md#expected-value), and using the vanished cross terms proves the [Itô isometry](../../../stochastic-calculus.md#ito-isometry):

$$
\boxed{\mathbb E[(H\mathbin\cdot M)_\infty^2]
=\sum_k\mathbb E[Z_{t_k}^2([M]_{t_{k+1}}-[M]_{t_k})]
=\mathbb E\int_0^\infty H_s^2\,d[M]_s.}
$$

To extend the [stochastic integral](../../../stochastic-calculus.md#stochastic-integral), use the finite [quadratic-variation measure](../../../stochastic-calculus.md#quadratic-variation-measure) $\nu_M(C)=\mathbb E\int\mathbf1_C\,d[M]$ on the [predictable sigma-algebra](../../../martingale.md#predictable-sigma-algebra). The [density of simple predictable processes for finite measures](../../../martingale.md#density-of-simple-predictable-processes-for-finite-measures) gives approximations to every $H\in L^2(\nu_M)$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) makes the corresponding terminal integrals Cauchy in $L^2$, and the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) makes the whole processes Cauchy in expected squared supremum. Their limit defines a continuous [martingale](../../../martingale.md), and the isometry persists. For a locally bounded [predictable process](../../../martingale.md#predictable-process), choose increasing [stopping times](../../../martingale.md#stopping-time) tending to infinity on which it is bounded, also restrict the time horizon, and perform this construction after stopping. The isometry shows that the stopped definitions agree on overlaps, so they patch into a uniquely defined continuous [local martingale](../../../martingale.md#local-martingale) $H\mathbin\cdot M$.

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) decomposes the smooth transform into a [continuous local martingale](../../../martingale.md#continuous-local-martingale) and a [finite-variation process](../../../stochastic-calculus.md#finite-variation-process):

$$
f(M_t)-f(0)=N_t+\frac12\int_0^tf''(M_s)\,d[M]_s,
\qquad N_t=\int_0^tf'(M_s)\,dM_s.
$$

If $f(M)$ has [finite variation](../../../real-analysis.md#total-variation-of-a-function), then $N$ also has [finite variation](../../../real-analysis.md#total-variation-of-a-function). A [continuous finite-variation local martingale is constant](../../../martingale.md#continuous-finite-variation-local-martingale-is-constant), so $N=0$ and

$$
0=[N]_t=\int_0^tf'(M_s)^2\,d[M]_s.
$$

It remains to show that the second-order term vanishes; the preceding observation alone does not establish this.

Let $Z=\{a:f'(a)=0\}$. By the [occupation-times formula](../../../brownian-motion.md#occupation-times-formula) for the [local time of a semimartingale](../../../stochastic-calculus.md#local-time-of-a-semimartingale),

$$
0=\int_{\mathbb R}f'(a)^2L_t^a(M)\,da.
$$

Therefore $L_t^a(M)=0$ for almost every $a\notin Z$. Also $f''(a)=0$ for almost every $a\in Z$: if $f'(a)=0$ and $f''(a)\ne0$, continuity of $f''$ makes $f'$ strictly monotone in a neighborhood of $a$, so that zero is isolated. Such isolated zeros form a countable [set](../../../set.md). Localizing to bounded paths and finite [quadratic variation](../../../stochastic-calculus.md#quadratic-variation), then using the [occupation-times formula](../../../brownian-motion.md#occupation-times-formula) once more, gives

$$
\int_0^t|f''(M_s)|\,d[M]_s
=\int_{\mathbb R}|f''(a)|L_t^a(M)\,da=0.
$$

Both terms in the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) now vanish. Apply this on all rational times and use continuity to obtain the simultaneous conclusion

$$
\boxed{f(M_t)=f(0)\quad\text{for every }t\geq0\text{ almost surely}.}
$$

This is the [finite-variation smooth transform of a continuous local martingale](../../../martingale.md#finite-variation-smooth-transform-of-a-continuous-local-martingale) property.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

There is an initial-value qualification in the printed conclusion. As written, nothing requires $A_0=0$. For example, $M\equiv0$ and $A\equiv1$ satisfy the hypotheses, because $M^2-A\equiv-1$ is a [local martingale](../../../martingale.md#local-martingale), but $M_t$ is not $N(0,1)$. **The correct variance is $A_t-A_0$; the printed formula holds under the usual normalization $A_0=0$.**

Indeed, $M^2-[M]$ is a [continuous local martingale](../../../martingale.md#continuous-local-martingale). Subtracting it from $M^2-A$ shows that $[M]-A$ is a continuous [local martingale](../../../martingale.md#local-martingale) with [finite variation](../../../real-analysis.md#total-variation-of-a-function), hence is its initial constant $-A_0$. Thus

$$
C_t:=A_t-A_0=[M]_t.
$$

In particular, $C$ is deterministic, continuous, nonnegative and increasing, regardless of the apparent allowance of a general [finite-variation process](../../../stochastic-calculus.md#finite-variation-process) in the premise.

For a real parameter $\theta$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives the complex [local martingale](../../../martingale.md#local-martingale)

$$
Z_t=\exp\left(i\theta M_t+\frac{\theta^2}{2}C_t\right),
\qquad dZ_t=i\theta Z_t\,dM_t.
$$

On every deterministic interval $[0,T]$, its modulus is at most $e^{\theta^2C_T/2}$, so its real and imaginary parts are bounded [local martingales](../../../martingale.md#local-martingale), hence true [martingales](../../../martingale.md). Taking [expectations](../../../probability-theory.md#expected-value) and using $Z_0=1$ yields

$$
\mathbb E e^{i\theta M_t}=e^{-\theta^2C_t/2}.
$$

By the [uniqueness theorem for characteristic functions](../../../probability-theory.md#uniqueness-theorem-for-characteristic-functions),

$$
\boxed{M_t\sim N(0,A_t-A_0).}
$$

A zero variance means the point mass at zero. This proves the requested normalized version by a direct [characteristic function](../../../probability-theory.md#characteristic-function) calculation.

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

First stop the solution on leaving $[-n,n]$, at $\tau_n$, and set $F_n(t)=\mathbb E\sup_{u\leq t}|X_{u\wedge\tau_n}|^2$. The [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) representation, the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give, for $0\leq t\leq1$,

$$
\begin{aligned}
F_n(t)&\leq 2\mathbb E\sup_{u\leq t}\left|\int_0^{u\wedge\tau_n}\sigma(X_s)\,dB_s\right|^2
+2\mathbb E\sup_{u\leq t}\left|\int_0^{u\wedge\tau_n}b(X_s)\,ds\right|^2\\
&\leq 8\mathbb E\int_0^{t\wedge\tau_n}\sigma(X_s)^2\,ds
+2t\mathbb E\int_0^{t\wedge\tau_n}b(X_s)^2\,ds\\
&\leq8A\int_0^t(1+F_n(s))\,ds.
\end{aligned}
$$

Here stopping ensures square integrability before the calculation, and $8\sigma^2+2t b^2\leq8(\sigma^2+b^2)$ explains the constant. The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives $F_n(t)\leq e^{8At}-1$. For globally [Lipschitz functions](../../../real-analysis.md#lipschitz-continuity) as coefficients, the [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients) supplies a nonexplosive solution. Letting $n$ increase and using [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma) proves the slightly stronger [maximal second-moment bound under linear growth](../../../stochastic-calculus.md#maximal-second-moment-bound-under-linear-growth):

$$
\boxed{\mathbb E\sup_{t\leq1}|X_t|^2\leq e^{8A}-1\leq e^{8A}.}
$$

For coefficients that are only [locally Lipschitz functions](../../../real-analysis.md#locally-lipschitz-function), let $\pi_n(x)=\max(-n,\min(x,n))$ and replace the coefficients by $\sigma(\pi_n(x))$ and $b(\pi_n(x))$. These are globally [Lipschitz functions](../../../real-analysis.md#lipschitz-continuity), agree with the originals on $[-n,n]$, and obey the same [linear growth condition for an SDE](../../../stochastic-calculus.md#linear-growth-condition-for-an-sde), since $|\pi_n(x)|\leq|x|$. The globally defined solutions agree until their common exits from $[-n,n]$ by [pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness). The uniform preceding estimate and [Markov's inequality](../../../probability-inequality.md#markov-inequality) imply

$$
\mathbb P(\tau_n\leq1)\leq\frac{e^{8A}-1}{n^2}\longrightarrow0.
$$

Patch the solutions before their increasing exit times. Their limiting lifetime exceeds $1$ almost surely by this bound. **Thus a pathwise unique strong solution exists throughout $[0,1]$ even for locally Lipschitz coefficients.**

## 5

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Separate $L$ into a [diffusion generator](../../../stochastic-process.md#diffusion-generator) and the constant killing term $-1/2$. The appropriate [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) and its explicit [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion) solution are

$$
dX_s=X_s\,dB_s+\frac12X_s\,ds,\qquad X_0=x,
\qquad \boxed{X_s=xe^{B_s}.}
$$

The second-order term in the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) cancels the drift of $\log|X|$ when $x\ne0$; if $x=0$, the solution stays zero.

Fix a terminal time $t$. Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $e^{-s/2}u(t-s,X_s)$ for $0\leq s\leq t$. Its drift is

$$
e^{-s/2}\left(-u_t+\frac{X_s^2}{2}u_{xx}+\frac{X_s}{2}u_x-\frac12u\right)(t-s,X_s)\,ds=0.
$$

After localization this is a [local martingale](../../../martingale.md#local-martingale), and it is bounded because $u$ is bounded. It is therefore a true [martingale](../../../martingale.md). Taking [expectations](../../../probability-theory.md#expected-value) at its endpoints gives the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula)

$$
\boxed{u(t,x)=e^{-t/2}\mathbb E[g(xe^{B_t})].}
$$

For $t>0$ and $x\ne0$, the change of variable $y=xe^z$ in the [normal density](../../../probability-theory.md#normal-density) produces the [killed geometric Brownian heat kernel](../../../stochastic-calculus.md#killed-geometric-brownian-heat-kernel) with respect to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure):

$$
\boxed{p(t,x,y)=
\begin{cases}
\displaystyle\frac{e^{-t/2}}{|y|\sqrt{2\pi t}}\exp\left[-\frac{\log^2(|y/x|)}{2t}\right],&xy>0,\\
0,&xy\leq0.
\end{cases}}
$$

For $xy>0$, an equivalent form is

$$
p(t,x,y)=\frac1{|x|\sqrt{2\pi t}}\exp\left[-\frac{(\log|y/x|+t)^2}{2t}\right].
$$

In particular,

$$
\boxed{p(t,1,y)=\frac1{\sqrt{2\pi t}}\exp\left[-\frac{(\log y+t)^2}{2t}\right]\quad(y>0).}
$$

The apparent missing $1/y$ in this last expression is absorbed into the completed square, together with the killing factor; it is not a transcription error. The total mass is $e^{-t/2}$, as expected for killing at rate $1/2$. At $x=0$ the fundamental kernel is instead the [measure](../../../measure-theory.md#measure) $e^{-t/2}\delta_0(dy)$; it has no [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) with respect to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Thus $u(t,0)=e^{-t/2}g(0)$. At $t=0$ the kernel is $\delta_x$, and continuity of bounded $g$ gives the initial condition. This also specifies the fundamental solution at the degenerate point omitted by a density-only formula.

## 6

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use coordinates $1,2,3$ for paper, scissors and stone. Let $X^N$ take values in the lattice [simplex](../../../algebraic-topology.md#simplex) $S_N=\{(n_1,n_2,n_3)/N:n_i\geq0,\ \sum_i n_i=N\}$. A uniformly selected unordered pair consists of types $i$ and $j$, $i\ne j$, with probability $2n_in_j/(N(N-1))$. Losing copies the winner, so the possible jumps of the [continuous-time Markov chain](../../../markov-process.md#continuous-time-markov-chain) are

$$
\frac{e_1-e_3}{N},\qquad\frac{e_2-e_1}{N},\qquad\frac{e_3-e_2}{N}.
$$

Ties make no change. For arbitrary event rate $\lambda$, the respective transition rates are $2\lambda Nx_1x_3/(N-1)$, $2\lambda Nx_2x_1/(N-1)$ and $2\lambda Nx_3x_2/(N-1)$. Choose

$$
\boxed{\lambda_N=\frac{N-1}{2}.}
$$

Then the rates are exactly $Nx_1x_3$, $Nx_2x_1$, $Nx_3x_2$. The [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) of this [cyclic imitation chain](../../../markov-process.md#cyclic-imitation-chain) is

$$
\mathcal L_Nf(x)=N\sum_{\ell\in\mathcal J}\beta_\ell(x)\bigl(f(x+\ell/N)-f(x)\bigr),
$$

where $\mathcal J=\{e_1-e_3,e_2-e_1,e_3-e_2\}$ and the three $\beta$ functions are, in that order, $x_1x_3,x_2x_1,x_3x_2$. Its drift is precisely

$$
F(x)=\sum_\ell\ell\beta_\ell(x)
=\bigl(x_1(x_3-x_2),\ x_2(x_1-x_3),\ x_3(x_2-x_1)\bigr).
$$

Here is a precise [fluid limit](../../../queueing-theory.md#fluid-limit) with its error control. Suppose $X^N_0\to x_0$ in probability, and let $x$ solve $\dot x=F(x)$, $x(0)=x_0$. For every finite $T$,

$$
\boxed{\sup_{0\leq t\leq T}\|X^N_t-x_t\|\longrightarrow0\quad\text{in probability}.}
$$

Indeed, the [martingale decomposition of a density-dependent jump process](../../../markov-process.md#martingale-decomposition-of-a-density-dependent-jump-process) gives

$$
X^N_t=X^N_0+\int_0^tF(X^N_s)\,ds+M^N_t,
\qquad
\langle M^N\rangle_t=\frac1N\int_0^t\sum_\ell\ell\ell^{\mathsf T}\beta_\ell(X^N_s)\,ds.
$$

This follows by compensating each transition count by its integrated rate; the compensated counts are square-integrable [martingales](../../../martingale.md), with variance equal to the expected compensator. Since $\|\ell\|^2=2$ and $x_1x_2+x_2x_3+x_3x_1\leq1/3$ on the [simplex](../../../algebraic-topology.md#simplex), the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality), applied coordinatewise, gives

$$
\mathbb E\sup_{t\leq T}\|M^N_t\|^2\leq4\mathbb E\|M^N_T\|^2
\leq\frac{8T}{3N}.
$$

The polynomial drift is [Lipschitz](../../../real-analysis.md#lipschitz-continuity) on the compact [simplex](../../../algebraic-topology.md#simplex), with some finite constant $L$. It preserves the sum of the coordinates, and each coordinate solves an equation of the form $\dot x_i=x_i h_i(x)$, so nonnegativity is preserved. Thus the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) stays in the [simplex](../../../algebraic-topology.md#simplex) and exists for all time. The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives

$$
\sup_{t\leq T}\|X^N_t-x_t\|
\leq e^{LT}\left(\|X^N_0-x_0\|+\sup_{t\leq T}\|M^N_t\|\right),
$$

which proves the claim by [Markov's inequality](../../../probability-inequality.md#markov-inequality). This proves the required version directly, rather than invoking an unspecified approximation theorem.

For an interior trajectory, differentiating the logarithm of the [product of numbers](../../../arithmetic.md#product-of-numbers) gives

$$
\frac{d}{dt}\log(x_1x_2x_3)
=(x_3-x_2)+(x_1-x_3)+(x_2-x_1)=0.
$$

The same identity for the product itself holds on the boundary, so **$x_1(t)x_2(t)x_3(t)$ is conserved.** A strictly positive initial product keeps the deterministic trajectory away from the boundary. Except at $(1/3,1/3,1/3)$ these interior trajectories are periodic: the strictly concave function $\sum_i\log x_i$ has smooth compact level curves surrounding its unique maximum, and the vector field is nonzero and tangent to each such curve.

The finite [Markov chain](../../../markov-process.md#markov-chain) behaves differently at long times. For $P(x)=x_1x_2x_3$, the change in $P$ during the first jump is

$$
P\left(x+\frac{e_1-e_3}{N}\right)-P(x)
=x_2\left(\frac{x_3-x_1}{N}-\frac1{N^2}\right).
$$

The other two terms are cyclic permutations. Their first-order contributions cancel, leaving the exact [product decay in a cyclic imitation chain](../../../markov-process.md#product-decay-in-a-cyclic-imitation-chain) identity

$$
\boxed{\mathcal L_NP=-\frac3NP,\qquad
\mathbb E P(X^N_t)=e^{-3t/N}\mathbb E P(X^N_0).}
$$

For $N\geq3$, while all three counts are positive, their product is at least $N-2$, so $P(X^N_t)\geq(N-2)/N^3$. A missing type cannot reappear. If $\tau$ is the first loss of a type, then

$$
\mathbb P(\tau>t)\leq\frac{N^3}{N-2}\,e^{-3t/N}\mathbb E P(X^N_0)\longrightarrow0.
$$

Once only two types remain, one always wins, so its count increases until an absorbing monochromatic vertex is reached, almost surely in finite time. The cases of one or two initially present types follow the same argument without the first stage. **Every finite chain eventually becomes monochromatic, whereas an interior deterministic solution retains its positive product.** The [fluid limit](../../../queueing-theory.md#fluid-limit) holds on each fixed finite interval; it does not justify exchanging the limits $N\to\infty$ and $t\to\infty$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
