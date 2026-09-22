<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $Ph=\mathbb E h(X)$ and $P_nh=n^{-1}\sum_i h(X_i)$ for the [expectation](../../../../../expected-value.md) and [empirical measure](../../../../../empirical-measure.md). A sufficient [bracketing of a function class](../../../../../bracketing-of-a-function-class.md) condition is that, for every $\varepsilon>0$, finitely many brackets $[l_j,u_j]$ cover $\mathcal H$, with measurable integrable endpoints and $P(u_j-l_j)<\varepsilon$. The [uniform strong law from finite L1 bracketing](../../../../../uniform-strong-law-from-finite-l1-bracketing.md) then gives

$$
\boxed{\sup_{h\in\mathcal H}|P_nh-Ph|\longrightarrow0\quad\text{almost surely}.}
$$

Here the observations are [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md). For an uncountable class, one either assumes a measurable supremum, for example through a [pointwise separable function class](../../../../../pointwise-separable-function-class.md), or formulates the conclusion as a pathwise bound on a common probability-one event.

For the parameterized class, the [Heine-Borel theorem](../../../../../heine-borel-theorem.md) makes $\Theta$ [compact](../../../../../compact-space.md). Put $M(x)=\sup_{\theta\in\Theta}|q(\theta,x)|$. A countable dense subset of $\Theta$ gives the same supremum because of [continuity](../../../../../continuous-function.md), so $M$ is measurable. Define the modulus

$$
w_\delta(x)=\sup_{\substack{\theta,\theta'\in\Theta\\|\theta-\theta'|\le\delta}}|q(\theta,x)-q(\theta',x)|.
$$

The supremum is measurable by taking a countable dense subset of the [compact](../../../../../compact-space.md) set of admissible pairs. For each $x$, [uniform continuity](../../../../../uniform-continuity.md) on $\Theta$ gives $w_\delta(x)\to0$. Also $w_\delta\le2M$, and $PM<\infty$. Thus the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives $Pw_\delta\to0$.

Choose a [finite net](../../../../../finite-net.md) of radius $\delta$ $\theta_1,\ldots,\theta_N$ in $\Theta$. The lower and upper envelopes of $q(\theta,\cdot)$ over each closed ball $\Theta\cap\overline B(\theta_j,\delta)$ are measurable integrable [function brackets](../../../../../bracketing-of-a-function-class.md); the same countable-dense-set argument applies within each such [compact](../../../../../compact-space.md) ball. Their widths are at most $w_{2\delta}$. They cover the whole class, so its [bracketing of a function class](../../../../../bracketing-of-a-function-class.md) condition follows. Moreover, [dominated convergence](../../../../../dominated-convergence-theorem.md) shows that $\theta\mapsto Pq(\theta,\cdot)$ is continuous. Both empirical and population functions therefore have a supremum over a common countable dense parameter set. Applying the [uniform strong law from finite L1 bracketing](../../../../../uniform-strong-law-from-finite-l1-bracketing.md) proves **uniform almost-sure convergence over the entire [compact](../../../../../compact-space.md) parameter set**, rather than merely convergence at each fixed parameter.

For the [exponential family](../../../../../exponential-family-split.md),

$$
\log f(\theta,x)=\theta x-K(\theta)+\log f_0(x),\qquad
\sup_\theta|\log f(\theta,X)|\le A|X|+B+|\log f_0(X)|,
$$

where $A=\sup_\Theta|\theta|$ and $B=\sup_\Theta|K(\theta)|$. Thus a weak sufficient condition is **bounded $K$ on $\Theta$, $f_0(X)>0$ almost surely, and [integrability](../../../../../integrability.md) of $|X|+|\log f_0(X)|$ under the sampling law**. No positive lower bound on $f_0$ over the whole real line is required. Zeros off the sampling support are harmless: choose arbitrary finite versions of the log-densities on that common null set when applying the function-class theorem.

If the sampling law is $f(\theta_0,\cdot)$, one convenient assumption is that $\Theta$ is a [compact](../../../../../compact-space.md) subset of the interior of the finite domain of the [cumulant function of an exponential family](../../../../../cumulant-function-of-an-exponential-family.md), and

$$
\int e^{\theta_0x}f_0(x)|\log f_0(x)|\,dx<\infty.
$$

On that interior, $K$ is continuous, hence bounded on $\Theta$. Finiteness of $K$ at $\theta_0\pm a$ for some $a>0$ implies $\mathbb E_{\theta_0}e^{a|X|}<\infty$, hence $\mathbb E_{\theta_0}|X|<\infty$. The displayed integral gives the remaining [integrability](../../../../../integrability.md). If the observations come from an arbitrary unrelated law, assumptions on $K$ and $f_0$ alone cannot control that law's tails; the sampling-law [integrability](../../../../../integrability.md) must then be stated explicitly.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
