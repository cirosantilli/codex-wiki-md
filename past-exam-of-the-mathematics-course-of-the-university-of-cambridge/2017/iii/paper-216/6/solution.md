<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the extended target [probability density function](../../../../../probability-density-function.md)

$$
\rho(x,p)=\mu(x)(2\pi)^{-d/2}e^{-\|p\|^2/2}.
$$

The desired [stationary distribution](../../../../../stationary-distribution.md) for positions is $\mu$; the full position-momentum [joint probability distribution](../../../../../joint-probability-distribution.md) is $\rho$, not $\mu$ alone. Gaussian momentum refreshment preserves $\rho$, since it redraws its momentum [marginal distribution](../../../../../marginal-distribution.md) independently while keeping the position fixed.

Let $R(x,p)=(x,-p)$ and $T=T_{\varepsilon,L}$ be the surrogate [leapfrog integration](../../../../../leapfrog-integration.md) map. The proposal in the paper is $S=R\circ T$: its notation $(X',-P')=T(x,p)$ includes the final momentum flip. Reversibility gives $RTR=T^{-1}$, so $S^2=I$. Both $R$ and $T$ preserve volume. Thus $S$ is an [involutive Metropolis proposal](../../../../../involutive-metropolis-proposal.md), and the required acceptance [probability](../../../../../probability.md) is

$$
\boxed{\alpha(x,p,x',p')=1\wedge
\frac{\mu(x')e^{-\|p'\|^2/2}}{\mu(x)e^{-\|p\|^2/2}}.}
$$

Equivalently, in terms of the surrogate [Hamiltonian](../../../../../hamiltonian.md) $H_\nu$,

$$
\alpha=1\wedge\left\{
 e^{H_\nu(x,p)-H_\nu(x',p')}
 \frac{\mu(x')\nu(x)}{\mu(x)\nu(x')}
\right\}.
$$

Only evaluations of the true target [probability density function](../../../../../probability-density-function.md) are needed at endpoints; the trajectory uses the surrogate [gradient](../../../../../gradient.md). Target and surrogate [normalizing constants](../../../../../normalizing-constant.md) cancel.

For $z=(x,p)$, the accepted flux satisfies

$$
\rho(z)\alpha(z)=\min\{\rho(z),\rho(Sz)\}=\rho(Sz)\alpha(Sz).
$$

Changing variables $z\mapsto Sz$ has unit absolute [Jacobian determinant](../../../../../jacobian-determinant.md), so this identity proves [detailed balance](../../../../../detailed-balance.md) for accepted moves. The rejection mass stays at the same point and is also reversible. The accept/reject step therefore preserves $\rho$. Since momentum refreshment also preserves $\rho$, their composition and either phase of the alternating process preserve $\rho$. Projecting onto positions proves **the position [stationary distribution](../../../../../stationary-distribution.md) is exactly the original target**. Stationarity alone does not establish uniqueness or convergence from every start; those require additional [irreducible Markov chain](../../../../../irreducible-markov-chain.md) and [aperiodic Markov chain](../../../../../aperiodic-markov-chain.md) hypotheses.

There is a genuine defect in the printed smoothing claim. For the positive, nondifferentiable [Laplace distribution](../../../../../laplace-distribution.md) $\mu(y)=e^{-|y|}/2$ on the real line, direct minimization gives, for every $\lambda>0$,

$$
\min_y\{\log\mu(y)+\lambda(x-y)^2\}
=-\log2-|x|-\frac1{4\lambda}.
$$

For $x>0$ the minimizer is $y=x+1/(2\lambda)$; for $x<0$ it is $y=x-1/(2\lambda)$; at zero both signs minimize. Hence normalization leaves $\nu=\mu$, still nondifferentiable at zero. The displayed construction does not in general produce the asserted smooth surrogate. For example, the also nondifferentiable target $\mu(y)\propto e^{-y^4-|y|}$ makes that infimum $-\infty$ for every $x$, since the negative quartic term dominates the quadratic penalty. The invariance proof above is valid conditional on actually having a usable smooth surrogate, as the subsequent algorithm assumes.

A corrected sufficient construction is [Moreau smoothing of a negative log-density](../../../../../moreau-smoothing-of-a-negative-log-density.md). For a [proper convex function](../../../../../proper-convex-function.md) with [sequential lower semicontinuity](../../../../../sequential-lower-semicontinuity.md) $U=-\log\mu$, set

$$
U_\lambda(x)=\min_y\{U(y)+\lambda\|x-y\|^2\},\qquad
\log\nu(x)=C-U_\lambda(x).
$$

The [Moreau envelope](../../../../../moreau-envelope.md) is differentiable, with $\nabla U_\lambda(x)=2\lambda(x-\operatorname{prox}_{U/(2\lambda)}(x))$; require $e^{-U_\lambda}$ to be integrable to normalize it. The signs differ from the printed formula. For the [Laplace distribution](../../../../../laplace-distribution.md), this gives

$$
U_\lambda(x)-\log2=
\begin{cases}
\lambda x^2,&|x|\leq1/(2\lambda),\\
|x|-1/(4\lambda),&|x|>1/(2\lambda),
\end{cases}
$$

a genuinely differentiable potential with integrable exponential tails. Using that surrogate with the boxed acceptance [probability](../../../../../probability.md) still targets the original [Laplace distribution](../../../../../laplace-distribution.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 216](../../paper-216-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
