# Paper 31

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper31.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper31.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work with the [filtration](../../../stochastic-process.md#filtration-probability-theory) relative to which the given [Brownian motion](../../../brownian-motion.md) or [Markov jump process](../../../markov-process.md#markov-jump-process) has its stated properties. All [martingale](../../../martingale.md) assertions below concern every finite time interval; no infinite-horizon [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) is claimed.

First put $C=\sup_x|\sigma(x)|$. The solution has the representation $X_t=\int_0^t\sigma(X_s)dB_s$, and the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives

$$
\mathbb EX_t^2=\mathbb E\int_0^t\sigma(X_s)^2ds\le C^2t.
$$

Thus $X$ is a square-integrable [martingale](../../../martingale.md), not just a [local martingale](../../../martingale.md#local-martingale). Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to its square cancels the finite-variation term and gives

$$
Z_t=2\int_0^tX_s\sigma(X_s)dB_s.
$$

The expected squared integrand integral is bounded by

$$
4\mathbb E\int_0^tX_s^2\sigma(X_s)^2ds\le4C^2\int_0^tC^2s\,ds=2C^4t^2.
$$

Therefore **both $X$ and $Z$ are true square-integrable [martingales](../../../martingale.md)**. This is the [bounded diffusion coefficient gives square martingales](../../../stochastic-calculus.md#bounded-diffusion-coefficient-gives-square-martingales) criterion. Only bounded measurability of the coefficient and existence of the stipulated solution have been used.

For the jump process, the [Lévy kernel of a Markov jump process](../../../markov-process.md#levy-kernel-of-a-markov-jump-process) uses displacements: a mark $y$ sends the state $x$ to $x+y$. Let $\Lambda=\sup_x\lambda(x)$ and $V=\sup_xv(x)$. The bounded total rate prevents explosion; the number of jumps on a finite interval is dominated by a rate-$\Lambda$ [Poisson process](../../../probability-theory.md#poisson-process). Let $N(ds,dy)$ record the jump displacements. Its [predictable compensator of a jump measure](../../../markov-process.md#predictable-compensator-of-a-jump-measure) is

$$
\nu(ds,dy)=K(X_{s-},dy)ds.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $\int |y|K(x,dy)\le\sqrt{\lambda(x)v(x)}$, so the zero first moment is absolutely meaningful. Since that moment vanishes,

$$
X_t=\int_0^t\int_{\mathbb R}y\,(N-\nu)(ds,dy),\qquad \mathbb EX_t^2=\mathbb E\int_0^tv(X_{s-})ds\le Vt.
$$

The compensated integral is a square-integrable [martingale](../../../martingale.md): its isometry follows first for bounded marks from conditional compensation and then by truncation in the squared-integrand [norm](../../../functional-analysis.md#norm).

The jump version of the square [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) is $X_t^2=2\int_0^tX_{s-}dX_s+\sum_{s\le t}(\Delta X_s)^2$. Hence

$$
Z_t=2\int_0^tX_{s-}dX_s+\int_0^t\int_{\mathbb R}y^2(N-\nu)(ds,dy).
$$

The first term is square [integrable](../../../measure-theory.md#integrability) because

$$
4\mathbb E\int_0^tX_{s-}^2v(X_{s-})ds\le2V^2t^2.
$$

The second is an [integrable](../../../measure-theory.md#integrability) [martingale](../../../martingale.md): the expected absolute uncompensated jump-square sum is at most $Vt$, and the compensator identity, multiplied by any bounded event known at an earlier time, makes its increments conditionally centered. Values $X_s$ and $X_{s-}$ agree for Lebesgue-almost every time, so the displayed compensation is exactly the one defining $Z$. Thus **$X$ and $Z$ are true [martingales](../../../martingale.md) in the jump case as well**. A fourth moment of the jumps is unnecessary; in particular we have not asserted that this $Z$ must be square [integrable](../../../measure-theory.md#integrability). This is [centered finite-rate jump kernel gives square martingales](../../../markov-process.md#centered-finite-rate-jump-kernel-gives-square-martingales).

## 2

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For $g(x)=\log|x|$ on $\mathbb R^2\setminus\{0\}$,

$$
\nabla g(x)=\frac{x}{|x|^2},\qquad \Delta g(x)=0.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), stopped in a compact [annulus](../../../topology.md#annulus-mathematics), therefore gives

$$
dM_t=\frac{B_t}{|B_t|^2}\mathbin\cdot dB_t.
$$

This proves the [local martingale](../../../martingale.md#local-martingale) property up to a possible hitting of the origin. For the [annulus](../../../topology.md#annulus-mathematics) exit time $T$, $M_{t\wedge T}$ is bounded between $\log r$ and $\log R$, so it is a true [uniformly integrable martingale](../../../martingale.md#uniformly-integrable-martingale).

The exit is finite almost surely. Indeed $|B_t|^2-2t$ is a [martingale](../../../martingale.md), so stopping at $T\wedge t$ gives $2\mathbb E(T\wedge t)=\mathbb E|B_{T\wedge t}|^2-1\le R^2-1$. Letting $t\to\infty$ proves $\mathbb ET<\infty$. Bounded convergence in the logarithmic [martingale](../../../martingale.md) now yields

$$
\boxed{\mathbb E M_T=M_0=0.}
$$

If $p$ is the [probability](../../../probability-theory.md#probability) of reaching radius $r$ before radius $R$, [continuity](../../../calculus.md#continuous-function) gives

$$
p\log r+(1-p)\log R=0,\qquad \boxed{p=\frac{\log R}{\log(R/r)}}.
$$

Hitting zero before reaching radius $R$ would require reaching every positive radius $r$ first. Its [probability](../../../probability-theory.md#probability) is bounded by $p$, which tends to zero as $r\downarrow0$. Any finite-time path hitting zero is bounded before that time and hence hits zero before exiting some integer-radius disk. A countable union over those disks proves **$B_t\ne0$ for every $t\ge0$, almost surely**. This is [planar Brownian motion avoids a fixed point](../../../brownian-motion.md#planar-brownian-motion-avoids-a-fixed-point); it also makes $M$ a globally defined [continuous local martingale](../../../martingale.md#continuous-local-martingale).

To decide whether it is a true [martingale](../../../martingale.md), compute its [expectation](../../../probability-theory.md#expected-value) directly. Condition on $B_0$ if necessary and use rotation to take $B_0=(1,0)$ and write $B_t=B_0+W_t$. Conditional on $\rho=|W_t|$, the angle of $W_t$ is uniform. The [angular average of a logarithmic potential](../../../partial-differential-equation.md#angular-average-of-a-logarithmic-potential) is

$$
\frac1{2\pi}\int_0^{2\pi}\log|1+\rho e^{i\theta}|d\theta=\log\max(1,\rho).
$$

For $\rho<1$ this follows by taking the real part of the convergent [power series](../../../real-analysis.md#power-series) for $\log(1+\rho e^{i\theta})$: each nonconstant Fourier term integrates to zero. For $\rho>1$ factor out $\rho$ and apply the same argument to $1/\rho$. The equality at one follows by the [integrable](../../../measure-theory.md#integrability) limiting logarithmic singularity. All interchanges are valid: the shifted [Gaussian density](../../../probability-and-statistics.md#multivariate-normal-density) is bounded near the origin, where $\int_0^1r|\log r|dr<\infty$, and its [Gaussian](../../../probability-theory.md#normal-distribution) tail controls logarithmic growth.

The radius $\rho$ has density $(\rho/t)e^{-\rho^2/(2t)}$. Consequently, for $t>0$,

$$
\boxed{\mathbb E M_t=\int_1^\infty\log\rho\,\frac{\rho}{t}e^{-\rho^2/(2t)}d\rho=\int_1^\infty\frac{e^{-\rho^2/(2t)}}{\rho}d\rho>0.}
$$

Since $M_0=0$, **$M$ is not a [martingale](../../../martingale.md)**, despite [integrability](../../../measure-theory.md#integrability) at each deterministic time. This is the [logarithmic radius of planar Brownian motion](../../../brownian-motion.md#logarithmic-radius-of-planar-brownian-motion) example.

The optional hint is consistent with this conclusion. The upper-radius exit $T(2,0)$ is finite and never occurs at zero. After that exit the stopped square is $(\log2)^2$; before it, a radius in $[1/2,2]$ also gives a logarithmic square no larger than $(\log2)^2$, while a radius below $1/2$ contributes precisely the extra indicated term. This proves the hinted inequality without assuming that the unstopped process is a true [martingale](../../../martingale.md).

## 3

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [simple predictable process](../../../martingale.md#simple-predictable-process) can be written

$$
H_s=\sum_{j=0}^{m-1}\xi_j\mathbf1_{(t_j,t_{j+1}]}(s),\qquad 0=t_0<t_1<\cdots<t_m\le\infty,
$$

where each $\xi_j$ is bounded and $\mathcal F_{t_j}$-measurable. Define its integral to start at zero:

$$
(H\mathbin\cdot M)_t=\sum_{j=0}^{m-1}\xi_j(M_{t\wedge t_{j+1}}-M_{t\wedge t_j}).
$$

Refining the partition leaves this sum unchanged. Every summand is a [martingale](../../../martingale.md), by conditioning its future increment on the information at $t_j$. Bounded coefficients and the $L^2$ bound on $M$ make the integral an [L2-bounded continuous martingale](../../../martingale.md#l2-bounded-continuous-martingale). Its terminal value is the same sum with $M_\infty$ substituted at any infinite endpoint; $L^2$ [martingale](../../../martingale.md) convergence supplies this limit.

We need the conditional square identity, rather than assuming [independent](../../../random-variable.md#independent-random-variables) increments. The [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) gives $\mathbb E\sup_t|M_t|^2<\infty$. Localize the square identity for $M^2-[M]$ at level and bracket [stopping times](../../../martingale.md#stopping-time). The stopped identity and this maximal bound give $\mathbb E[M]_\infty<\infty$ by [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem). Now

$$
\sup_t|M_t^2-[M]_t|\le\sup_t|M_t|^2+[M]_\infty
$$

is [integrable](../../../measure-theory.md#integrability), so [localization](../../../commutative-algebra.md#localization-of-a-ring) passes to conditional [expectations](../../../probability-theory.md#expected-value) and $M^2-[M]$ is a [uniformly integrable martingale](../../../martingale.md#uniformly-integrable-martingale). Expanding a squared increment and using $\mathbb E(M_t\mid\mathcal F_s)=M_s$ proves

$$
\mathbb E((M_t-M_s)^2\mid\mathcal F_s)=\mathbb E([M]_t-[M]_s\mid\mathcal F_s),\qquad s\le t\le\infty.
$$

The infinite endpoint follows from $L^2$ convergence and [integrability](../../../measure-theory.md#integrability) of the bracket. The initial value $M_0$ need not be zero: the integral itself is zero-starting.

In the square of the terminal integral, all cross terms vanish. For $j<k$, the $j$th increment and both coefficients in its cross term are measurable at $t_k$, whereas the conditional mean of the $k$th increment there is zero. For the diagonal terms, the preceding conditional identity can be multiplied by the bounded $\xi_j^2$. Therefore

$$
\begin{aligned}
\mathbb E(H\mathbin\cdot M)_\infty^2
&=\sum_j\mathbb E\bigl[\xi_j^2(M_{t_{j+1}}-M_{t_j})^2\bigr]\\
&=\sum_j\mathbb E\bigl[\xi_j^2([M]_{t_{j+1}}-[M]_{t_j})\bigr]
=\boxed{\mathbb E(H^2\mathbin\cdot[M])_\infty}.
\end{aligned}
$$

This proves the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) for these simple integrands. Ordered stopping-time intervals also work, replacing the conditional identity by [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale), but deterministic intervals suffice for the approximation requested here.

For that approximation, put $\mu(A)=\mathbb E\int_0^1\mathbf1_A(\omega,s)ds$ on the [predictable sigma-algebra](../../../martingale.md#predictable-sigma-algebra). This is a [finite measure](../../../measure-theory.md#finite-measure). That [sigma-algebra](../../../measure-theory.md#sigma-algebra) is generated, apart from the zero-time slice of measure zero, by rectangles $A\times(s,t]$ with $A\in\mathcal F_s$. The indicator of every such rectangle is a bounded [simple predictable process](../../../martingale.md#simple-predictable-process).

Here is a density proof. Let $V$ be the closed linear span of these indicators in $L^2(\mu)$, and let $\mathcal D$ contain the [predictable](../../../martingale.md#predictable-process) sets whose indicators belong to $V$. The whole space belongs to $\mathcal D$; complements stay in $\mathcal D$; and disjoint countable unions do also, because their finite partial indicator sums converge in $L^2$ under the [finite measure](../../../measure-theory.md#finite-measure). Thus $\mathcal D$ is a [Dynkin system](../../../measure-theory.md#dynkin-system) containing the generating rectangle [pi-system](../../../measure-theory.md#pi-system). The [Pi-lambda theorem](../../../probability-theory.md#pi-lambda-theorem) makes it the entire [predictable sigma-algebra](../../../martingale.md#predictable-sigma-algebra). Bounded [predictable](../../../martingale.md#predictable-process) simple functions therefore belong to $V$. Truncating any $L^2(\mu)$ function and then approximating its truncated range by finitely many levels shows that every such function belongs to $V$. A finite sum of rectangle indicators can be rewritten on one common deterministic time partition, with the coefficient on each interval measurable at its left endpoint; it is exactly an allowed simple process.

Consequently choose $H^n$ of this form with $\|H^n-H\|_{L^2(\mu)}<1/n$. This proves

$$
\boxed{\mathbb E\int_0^1|H_s^n-H_s|^2ds\longrightarrow0.}
$$

It is [density of simple predictable processes for finite measures](../../../martingale.md#density-of-simple-predictable-processes-for-finite-measures), with a proof of the actual approximation step.

Finally apply the preceding isometry to $M_t=B_{t\wedge1}$, whose bracket is $t\wedge1$. The elementary integrals $I_n=\int_0^1H_s^n dB_s$ satisfy

$$
\mathbb E|I_n-I_m|^2=\mathbb E\int_0^1|H_s^n-H_s^m|^2ds\longrightarrow0.
$$

**Define the [Itô integral](../../../stochastic-calculus.md#ito-integral) as the $L^2$ limit of these elementary integrals.** The same identity shows [independence](../../../random-variable.md#independent-random-variables) of the approximating sequence, linearity, mean zero, and $\mathbb E(\int_0^1H_s dB_s)^2=\mathbb E\int_0^1H_s^2ds$. Applying the Doob inequality to the difference processes also gives uniform-in-time $L^2$ convergence on $[0,1]$, with a continuous [martingale](../../../martingale.md) version of the integral.

## 4

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For $\theta>0$, $E_s=\exp(\theta B_s-\theta^2s/2)$ is an [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion), as follows directly from [independent](../../../random-variable.md#independent-random-variables) [Gaussian](../../../probability-theory.md#normal-distribution) increments. Stop it at $\tau_\delta\wedge t$, where $\tau_\delta$ is the first time $B$ reaches $\delta$. On $\{\tau_\delta\le t\}$,

$$
E_{\tau_\delta}\ge\exp(\theta\delta-\theta^2t/2).
$$

The stopped [expectation](../../../probability-theory.md#expected-value) is one and the other contribution is nonnegative, so

$$
\mathbb P(\sup_{s\le t}B_s\ge\delta)\le e^{-\theta\delta+\theta^2t/2}.
$$

For $t>0$, minimize the exponent at $\theta=\delta/t$. Apply the same argument to $-B$ and use the union bound to obtain

$$
\boxed{\mathbb P(\sup_{s\le t}|B_s|>\delta)\le2e^{-\delta^2/(2t)}.}
$$

At $t=0$ the [probability](../../../probability-theory.md#probability) is zero; the right side can be interpreted by its limit. This proves the [Gaussian maximal bound for Brownian motion](../../../brownian-motion.md#gaussian-maximal-bound-for-brownian-motion) without losing an extra factor from a two-sided reflection argument.

Let $L$ be a global Lipschitz constant of $b$. Realize the diffusion with the stated generator by $dX_s^\varepsilon=b(X_s^\varepsilon)ds+\varepsilon dW_s$, where $W$ is a standard $d$-dimensional [Brownian motion](../../../brownian-motion.md). Global Lipschitz [continuity](../../../calculus.md#continuous-function) gives existence and uniqueness; its generator is exactly the printed operator. Couple it with the ordinary differential equation having the same initial value $x(0)=x_0$. Subtraction gives, with $D_t=\sup_{s\le t}|X_s^\varepsilon-x_s|$,

$$
D_t\le\varepsilon\sup_{s\le t}|W_s|+L\int_0^tD_sds.
$$

The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) implies $D_t\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|$. If a [Euclidean norm](../../../functional-analysis.md#euclidean-norm) exceeds $u$, some coordinate has absolute value exceeding $u/\sqrt d$. The scalar bound and a union over the coordinates therefore give

$$
\mathbb P(D_t>\delta)\le2d\exp\!\left(-\frac{\delta^2e^{-2Lt}}{2dt\varepsilon^2}\right),\qquad t>0.
$$

Taking the [logarithm](../../../calculus.md#logarithm) and multiplying by $\varepsilon^2$ yields the explicit answer

$$
\boxed{\limsup_{\varepsilon\downarrow0}\varepsilon^2\log\mathbb P(D_t>\delta)\le-\frac{\delta^2e^{-2Lt}}{2dt}<0.}
$$

For $t=0$ the [probability](../../../probability-theory.md#probability) is zero and the limit is $-\infty$, with $\log0=-\infty$. This is [exponential small-noise concentration for a Lipschitz diffusion](../../../stochastic-calculus.md#exponential-small-noise-concentration-for-a-lipschitz-diffusion).

**Matching the deterministic initial value is necessary.** The printed last line specifies the differential equation but does not separately write this initial condition. Without it, take $b=0$ and a deterministic solution displaced from $x_0$ by $2\delta$ in one fixed direction. The deviation event already holds at time zero, giving logarithmic rate zero instead of a strictly negative rate.

## 5

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Write $f=u+iv$. The [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) give $v_x=-u_y$, $v_y=u_x$ and $\Delta u=\Delta v=0$. Since the two Brownian coordinates are [independent](../../../random-variable.md#independent-random-variables), $[X]_t=[Y]_t=t$ and $[X,Y]_t=0$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) therefore becomes

$$
dU_t=u_x(Z_t)dX_t+u_y(Z_t)dY_t,\qquad dV_t=-u_y(Z_t)dX_t+u_x(Z_t)dY_t.
$$

Stop in balls on which the derivatives are bounded. The stopped integrals are [martingales](../../../martingale.md), proving that $U$ and $V$ are [local martingales](../../../martingale.md#local-martingale). Their coefficient rows have equal squared length and are [orthogonal](../../../linear-algebra.md#orthogonal-vectors). Thus

$$
\boxed{[U]_t=[V]_t=\int_0^t|f'(Z_s)|^2ds,\qquad [U,V]_t=0.}
$$

These are [quadratic covariations of an analytic Brownian image](../../../stochastic-calculus.md#quadratic-covariations-of-an-analytic-brownian-image); [orthogonality](../../../linear-algebra.md#orthogonal-vectors) does not in general imply [independence](../../../random-variable.md#independent-random-variables) of the two transformed coordinates.

For the exit law, put $c=2a^2$. Squaring sends the positive quadrant to the upper half-plane, sends $a+ia$ to $ic$, and the [Möbius transformation](../../../group-theory.md#mobius-transformation) $w\mapsto(w-ic)/(w+ic)$ sends the upper half-plane to the unit disk with the starting point sent to zero. Its composition is the displayed [conformal map](../../../geometry-and-topology.md#conformal-map). The exit time is finite: it is the minimum of the two almost surely finite one-dimensional hitting times of zero. There is no hit at the quadrant's corner, since a [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started away from zero avoids that point.

We can justify the uniform image exit law without assuming a conformal-time-change theorem. For each integer $n\ge1$, the real and imaginary parts of $f(Z_{t\wedge T})^n$ are bounded [martingales](../../../martingale.md) obtained from [harmonic functions](../../../partial-differential-equation.md#harmonic-function). At the start their values are zero. The [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) at the finite exit time gives $\mathbb E f(Z_T)^n=0$. The boundary image has modulus one, and conjugation gives the vanishing negative Fourier moments as well. Trigonometric polynomials are dense among [continuous functions](../../../calculus.md#continuous-function) on the [unit circle](../../../complex-analysis.md#complex-unit-circle), so these moments characterize the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) there.

Consequently the real variable $W=Z_T^2$ is the inverse image of a uniform point $e^{i\Theta}$ under that [Möbius transformation](../../../group-theory.md#mobius-transformation):

$$
W=ic\,\frac{1+e^{i\Theta}}{1-e^{i\Theta}}=-c\cot(\Theta/2).
$$

The Jacobian of this change of variable gives the centered [Cauchy distribution](../../../probability-theory.md#cauchy-distribution) of scale $c$:

$$
p_W(w)=\frac{c}{\pi(w^2+c^2)},\qquad w\in\mathbb R.
$$

Positive $w$ corresponds to exit at $\sqrt w$ on the real axis; negative $w$ corresponds to exit at $i\sqrt{-w}$ on the imaginary axis. Pulling back by $w=\pm r^2$ therefore gives the complete boundary law

$$
\boxed{\mathbb P(Z_T\in dr)=\frac{4a^2r}{\pi(r^4+4a^4)}dr,\qquad \mathbb P(Z_T\in i\,dr)=\frac{4a^2r}{\pi(r^4+4a^4)}dr\quad(r>0).}
$$

Here $dr$ on each axis denotes length along that axis, not two-dimensional area measure. Each density integrates to $1/2$, with no remaining atoms. Equivalently the chosen axis is a fair Bernoulli choice [independent](../../../random-variable.md#independent-random-variables) of the radius, and

$$
\boxed{\mathbb P(|Z_T|\le r)=\frac2\pi\arctan\!\left(\frac{r^2}{2a^2}\right),\quad r\ge0.}
$$

This is [Brownian exit law from a quadrant](../../../brownian-motion.md#brownian-exit-law-from-a-quadrant), obtained as a [harmonic measure](../../../brownian-motion.md#harmonic-measure) and not as an absolutely continuous planar density.

## 6

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Here is a finite-horizon [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) statement with the sign fixed explicitly. Let $B$ be a [Brownian motion](../../../brownian-motion.md) under $P$, and let $\theta$ be [predictable](../../../martingale.md#predictable-process) with $\int_0^T\theta_s^2ds<\infty$ almost surely. If

$$
L_t=\exp\!\left(\int_0^t\theta_s dB_s-\frac12\int_0^t\theta_s^2ds\right),\qquad 0\le t\le T,
$$

is a true [martingale](../../../martingale.md) with $\mathbb EL_T=1$, then the measure $Q$ defined by $dQ=L_TdP$ makes $B_t-\int_0^t\theta_sds$ a [Brownian motion](../../../brownian-motion.md) up to $T$. The sufficient [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) is $\mathbb E\exp(\tfrac12\int_0^T\theta_s^2ds)<\infty$. Merely being a [local martingale](../../../martingale.md#local-martingale) is not a sufficient density condition.

For a deterministic [absolutely continuous function](../../../sobolev-space.md#absolutely-continuous-function) $h$ with $h(0)=0$ and [derivative](../../../calculus.md#derivative) $g\in L^2[0,T]$, take $\theta=g$. [Novikov's condition](../../../stochastic-calculus.md#novikov-s-condition) holds because its exponential is deterministic and finite. Under $Q$, the canonical process has the law of a [Brownian motion](../../../brownian-motion.md) plus $h$. Thus for every bounded measurable path functional $F$,

$$
\boxed{\mathbb E F(B+h)=\mathbb E\left[F(B)\exp\!\left(\int_0^Tg_s dB_s-\frac12\int_0^Tg_s^2ds\right)\right].}
$$

This derives the [Cameron-Martin theorem](../../../brownian-motion.md#cameron-martin-theorem) density formula from the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem), rather than assuming the two measures have the same drift convention. Replacing $h$ by $-h$ changes the sign of the [stochastic integral](../../../stochastic-calculus.md#stochastic-integral).

The question's path space is the whole half-line, not just one finite horizon. When $g\in L^2(0,\infty)$, the density [martingale](../../../martingale.md) satisfies

$$
\mathbb EL_t^2=\exp\!\left(\int_0^tg_s^2ds\right)\le e^{\|g\|_2^2}.
$$

It has a [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) limit $L_\infty=\exp(\int_0^\infty g_s dB_s-\|g\|_2^2/2)$ of mean one, strictly positive almost surely. Integrals here converge in $L^2$ and almost surely. The finite-time identities then identify $L_\infty$ as the density on the full path [sigma-algebra](../../../measure-theory.md#sigma-algebra), since finite-time cylinder events generate it. This is [Cameron-Martin shifts on infinite Wiener path space](../../../brownian-motion.md#cameron-martin-shifts-on-infinite-wiener-path-space). Finite-horizon [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) alone does not imply infinite-horizon [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures).

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

**There is no density on the full infinite path space; the two laws are mutually singular.** Under [Wiener measure](../../../brownian-motion.md#wiener-measure), $B_t/t\to0$ almost surely. Under the shifted law, $(B_t+t)/t\to1$ almost surely, so the same measurable tail event separates the laws.

For completeness the Brownian limit follows from the [Gaussian](../../../probability-theory.md#normal-distribution) bound at integers and the maximal bound on each interval $[n,n+1]$: for every fixed $\eta>0$, both $\sum_n\mathbb P(|B_n|>\eta n)$ and $\sum_n\mathbb P(\sup_{0\le s\le1}|B_{n+s}-B_n|>\eta n)$ are finite. The [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) and [continuity](../../../calculus.md#continuous-function) fill the gaps between integers. Intersect over positive rational $\eta$. This proves the limit and the claimed singularity, which is [infinite-horizon singularity of Brownian motion with constant drift](../../../brownian-motion.md#infinite-horizon-singularity-of-brownian-motion-with-constant-drift).

On every finite horizon there nevertheless is the density $e^{B_T-T/2}$. Its failure to give a global density is exactly the distinction required by the printed half-line path space.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The deterministic shift has [derivative](../../../calculus.md#derivative) $g_s=-\mathbf1_{[0,1]}(s)$ and finite total energy one. The infinite-horizon Cameron-Martin formula therefore gives

$$
\boxed{\frac{d\mathcal L(B-(\,\cdot\,\wedge1))}{d\mathcal L(B)}(w)=\exp(-w(1)-1/2).}
$$

The integral of this density is one by the moment-generating function of $B_1\sim N(0,1)$. It is strictly positive, so **the shifted law and [Wiener measure](../../../brownian-motion.md#wiener-measure) are equivalent on the whole half-line**. The density depends only on the path through time one; after that time the shift is constant.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

**There is no density; scaling by two gives a law singular to [Wiener measure](../../../brownian-motion.md#wiener-measure).** On $[0,1]$ form the pathwise dyadic sums

$$
Q_n(w)=\sum_{k=1}^{2^n}\bigl(w(k2^{-n})-w((k-1)2^{-n})\bigr)^2.
$$

Under [Wiener measure](../../../brownian-motion.md#wiener-measure), [independent](../../../random-variable.md#independent-random-variables) normal increments give $\mathbb EQ_n=1$ and $\operatorname{var}(Q_n)=2^{1-n}$. Chebyshev's inequality and the [Borel-Cantelli lemma](../../../probability-theory.md#borel-cantelli-lemmas) show $Q_n\to1$ almost surely, because the variances are summable. For $2B$, every sum is four times its Brownian counterpart and hence tends to four almost surely. The event that the limit equals one separates the two laws. Unlike the linear-drift case, this obstruction already occurs on a finite interval: it is the [Pathwise quadratic variation distinguishes Brownian speeds](../../../stochastic-calculus.md#pathwise-quadratic-variation-distinguishes-brownian-speeds) argument.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The PDF's subscript is $0$, and the [Brownian motion](../../../brownian-motion.md) starts from zero. Thus $B_0=0$ almost surely and the process is exactly $B$ at every time. **Its law is [Wiener measure](../../../brownian-motion.md#wiener-measure) itself, with density $1$.** There is no random future coefficient or anticipating transformation in this printed case.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
