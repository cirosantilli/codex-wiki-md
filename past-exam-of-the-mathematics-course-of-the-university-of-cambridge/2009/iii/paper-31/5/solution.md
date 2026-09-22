<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [martingale](../../../../../martingale-split.md) describes an observable after its predictable drift has been removed. For a [Markov chain](../../../../../markov-chain.md) the drift is the change produced by its transition operator; for [Brownian motion](../../../../../brownian-motion-split.md) it is one half of the [Laplacian](../../../../../laplacian.md). Requiring the resulting processes to be [martingales](../../../../../martingale-split.md) for a sufficiently rich class of observables determines the transition law itself. The same identities, combined with [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md), determine hitting probabilities, expected exit times and recurrence or transience. The duplicated Q5 paragraph in the PDF is a repeated printing of this one essay request.

For a finite or countable-state [Markov chain](../../../../../markov-chain.md) with [transition matrix](../../../../../stochastic-matrix.md) $P$, define $(Pf)(x)=\sum_yP(x,y)f(y)$ for a bounded test function $f$. The [Markov property](../../../../../markov-property.md) says $\mathbb E[f(X_{n+1})\mid\mathcal F_n]=(Pf)(X_n)$. Consequently

$$
M_n^f=f(X_n)-f(X_0)-\sum_{j=0}^{n-1}\bigl((Pf)(X_j)-f(X_j)\bigr)
$$

is a [martingale](../../../../../martingale-split.md), since each increment has conditional [expected value](../../../../../expected-value.md) zero. Conversely, if these processes are [martingales](../../../../../martingale-split.md) for every bounded $f$, taking the conditional expectation of an increment recovers that identity. With $f=\mathbf1_{\{y\}}$ it gives $\mathbb P(X_{n+1}=y\mid\mathcal F_n)=P(X_n,y)$ for every state $y$. Thus, given the initial law, **these identities characterize the [Markov chain](../../../../../markov-chain.md)**, not merely a few of its moments. This is the [discrete-time Markov chain martingale characterization](../../../../../discrete-time-markov-chain-martingale-characterization.md).

The drift operator is $P-I$. If $(P-I)h=0$ away from a target set, $h(X_{n\wedge T})$ is a [stopped martingale](../../../../../stopped-martingale.md), where $T$ is the first hit of that set. Under boundedness or suitable [uniform integrability](../../../../../uniform-integrability.md), the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) expresses $h$ in terms of boundary hitting probabilities. Similarly, if $(P-I)v=-1$ away from the target and $v=0$ on it, then $v(X_{n\wedge T})+(n\wedge T)$ is a [martingale](../../../../../martingale-split.md), giving $v(x)=\mathbb E_xT$ when the terminal limit is justified.

For a concrete calculation, take a [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md) on $\{0,1,\ldots,N\}$ stopped at $T$, its first hit of $0$ or $N$. In the interior, $h(i)=i$ has zero drift, while $v(i)=i(N-i)$ satisfies

$$
\frac12v(i-1)+\frac12v(i+1)-v(i)=-1.
$$

The stopped identity gives $\mathbb E_i(T\wedge n)=v(i)-\mathbb E_iv(X_{T\wedge n})\le v(i)$, proving $T$ finite with finite mean. Bounded convergence in both stopped identities now yields the **[gambler's ruin](../../../../../gambler-s-ruin.md) answers**

$$
\boxed{\mathbb P_i(X_T=N)=i/N,\qquad\mathbb E_iT=i(N-i).}
$$

This illustrates why the integrability justification is part of using a [martingale](../../../../../martingale-split.md), rather than an automatic consequence of writing an equation.

For a finite-state [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) with generator matrix $Q=(q_{ij})$, the corresponding [martingale problem for a continuous-time Markov chain](../../../../../martingale-problem-for-a-continuous-time-markov-chain.md) uses

$$
M_t^f=f(X_t)-f(X_0)-\int_0^t(Qf)(X_s)\,ds,\qquad (Qf)(i)=\sum_{j\ne i}q_{ij}(f(j)-f(i)).
$$

These are [martingales](../../../../../martingale-split.md). Conversely, suppose an adapted [càdlàg](../../../../../cadlag.md) finite-state process satisfies these identities. Let $P_t=e^{tQ}$, fix $T$, and set $g(s,i)=(P_{T-s}f)(i)$. Then $\partial_sg+Qg=0$. Apply deterministic integration by parts to the finite collection of indicator [martingales](../../../../../martingale-split.md) to obtain the time-dependent [Dynkin formula](../../../../../dynkin-s-formula.md): $g(s,X_s)-g(0,X_0)-\int_0^s(\partial_rg+Qg)(r,X_r)dr$ is a [martingale](../../../../../martingale-split.md). Therefore

$$
\mathbb E[f(X_T)\mid\mathcal F_s]=(P_{T-s}f)(X_s).
$$

This recovers the [Markov property](../../../../../markov-property.md) and the entire semigroup, proving the characterization. On countable spaces one uses nonexplosion and localization to justify the analogous unbounded-rate formulas.

For $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md), the [Itô formula](../../../../../ito-s-lemma.md) shows that, for $f\in C_c^\infty(\mathbb R^d)$,

$$
f(B_t)-f(B_0)-\frac12\int_0^t\Delta f(B_s)\,ds=\int_0^t\nabla f(B_s)\cdot dB_s
$$

is a true [martingale](../../../../../martingale-split.md), since its bounded derivatives make the integral square-integrable on each bounded horizon. This is the [martingale problem for Brownian motion](../../../../../martingale-problem-for-brownian-motion.md) with generator $L=\tfrac12\Delta$.

Here is why it also characterizes [Brownian motion](../../../../../brownian-motion-split.md). Suppose a continuous adapted process $X$, with $X_0=x$, satisfies that [martingale problem](../../../../../martingale-problem.md). Use smooth cutoff test functions equal to $x_i$ and $x_ix_j$ inside successively larger balls, and stop before leaving those balls. The coordinate tests show that $X^i-x_i$ are continuous [local martingales](../../../../../local-martingale.md); the product tests show that $X^iX^j-x_ix_j-\delta_{ij}t$ are local martingales. The [Itô product rule](../../../../../ito-product-rule.md) consequently gives

$$
[X^i,X^j]_t=\delta_{ij}t:
$$

the difference between the two proposed compensators is a continuous finite-variation local martingale, hence constant and zero at time zero. For each $u\in\mathbb R^d$, another application of the [Itô formula](../../../../../ito-s-lemma.md) gives the exponential [local martingale](../../../../../local-martingale.md)

$$
Z_t^u=\exp\!\left(iu\cdot(X_t-x)+\tfrac12|u|^2t\right).
$$

Its modulus is the deterministic quantity $e^{|u|^2t/2}$, so it is a true [martingale](../../../../../martingale-split.md) on every bounded time interval. Taking its [conditional expectation](../../../../../conditional-expectation.md) and dividing by its known value at time $s$ gives

$$
\mathbb E[e^{iu\cdot(X_t-X_s)}\mid\mathcal F_s]=e^{-|u|^2(t-s)/2}.
$$

The [conditional characteristic function](../../../../../conditional-characteristic-function.md) identifies a centered [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) of covariance $(t-s)I$, independent of the past. Together with continuity, this is the defining law of [Brownian motion](../../../../../brownian-motion-split.md). This proves the [Lévy characterization of multidimensional Brownian motion](../../../../../levy-characterization-of-multidimensional-brownian-motion.md) in the form needed for the generator characterization.

The analytic use of these [martingales](../../../../../martingale-split.md) parallels the chain case. A [harmonic function](../../../../../harmonic-function.md) $h$ satisfies $\Delta h=0$, so it yields a stopped [local martingale](../../../../../local-martingale.md) until the process leaves its domain of harmonicity. Bounded stopped observables permit [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) and solve boundary hitting problems. A solution of $\tfrac12\Delta v=-1$ with zero boundary values gives an expected exit time. For example, in the ball of radius $R$, $v(x)=(R^2-|x|^2)/d$ gives $\mathbb E_xT_R=(R^2-|x|^2)/d$; stopping $|B_t|^2-dt$ first at $T_R\wedge n$ proves finiteness and justifies the limiting calculation. The [Brownian local time](../../../../../brownian-local-time.md) construction in Q4 is another example: the predictable compensators of approximations to $|B_t|$ recover its increasing occupation term.

We now prove the required three-dimensional [transience of Brownian motion in dimension at least three](../../../../../transience-of-brownian-motion-in-dimension-at-least-three.md), in the strong sense $|B_t|\to\infty$ [almost surely](../../../../../almost-sure-convergence.md). Start first at a point $x$ with $r<|x|<R$, and let $T$ be the first exit from this annulus. The [radial Laplacian](../../../../../radial-laplacian.md) in dimension three gives

$$
\Delta\frac1{|x|}=\frac2{|x|^3}-\frac2{|x|^3}=0\qquad(x\ne0).
$$

Thus $|B_{t\wedge T}|^{-1}$ is a bounded [martingale](../../../../../martingale-split.md). The exit time is finite: stopping $|B_t|^2-3t$ gives $3\mathbb E(t\wedge T)\le R^2-|x|^2$. At exit, continuity puts $|B_T|$ at either $r$ or $R$. The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) therefore yields

$$
\frac1{|x|}=\frac1r\mathbb P_x(\tau_r<\tau_R)+\frac1R\mathbb P_x(\tau_R<\tau_r),
$$

and hence the [Brownian sphere-hitting probability in dimension three](../../../../../brownian-sphere-hitting-probability-in-dimension-three.md)

$$
\mathbb P_x(\tau_r<\tau_R)=\frac{|x|^{-1}-R^{-1}}{r^{-1}-R^{-1}}.
$$

As $R\to\infty$, the events $\{\tau_r<\tau_R\}$ increase to $\{\tau_r<\infty\}$: a continuous path is bounded on the finite interval preceding any finite inner hit. This argument assumes no transience. Consequently

$$
\boxed{\mathbb P_x(\tau_r<\infty)=r/|x|\quad(|x|>r).}
$$

To pass from a positive escape probability to almost-sure eventual escape, take [Brownian motion](../../../../../brownian-motion-split.md) started at zero. Let $\sigma_R$ be its first hit of the sphere of radius $R$. Stopping the squared-norm [martingale](../../../../../martingale-split.md) proves $\mathbb E\sigma_R=R^2/3<\infty$. At $\sigma_R$, the [Strong Markov property](../../../../../strong-markov-property.md) and the preceding hitting formula give

$$
\mathbb P(\exists t\ge\sigma_R:|B_t|\le r)=r/R\qquad(R>r).
$$

The [Strong Markov property](../../../../../strong-markov-property.md) here follows from independent Brownian increments by approximating a stopping time from above with dyadic-valued stopping times and using path continuity. Choose $R_m=2^m r$. The exit times $\sigma_{R_m}$ increase to infinity, since a continuous path is bounded on every compact time interval. The events of a return to the closed ball of radius $r$ after $\sigma_{R_m}$ decrease and have [probabilities](../../../../../probability.md) $2^{-m}$. Their intersection has [probability](../../../../../probability.md) zero. Thus almost surely there is some finite exit time after which the path never again enters that ball. Apply this simultaneously to all positive integer $r$. This proves the [last visit to a bounded ball for three-dimensional Brownian motion](../../../../../last-visit-to-a-bounded-ball-for-three-dimensional-brownian-motion.md) conclusion and therefore

$$
\boxed{|B_t|\longrightarrow\infty\quad\text{almost surely in dimension three}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
