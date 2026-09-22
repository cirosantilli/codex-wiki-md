<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The expected [check loss](../../../../../check-loss.md) is finite because $\rho_\tau(u)\leq |u|$. It is also Lipschitz in its location argument, with constant at most one. For any fixed $q$, the continuous [distribution function](../../../../../cumulative-distribution-function.md) makes $\mathbb P(Y=q)=0$. The derivative of $\rho_\tau(Y-q)$ with respect to $q$, away from that null event, is $\mathbf1_{\{Y<q\}}-\tau$. Difference quotients are bounded by one, so the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives

$$
\frac{d}{dq}\mathbb E\rho_\tau(Y-q)=F(q)-\tau.
$$

The continuous, strictly increasing [distribution function](../../../../../cumulative-distribution-function.md) has limits zero and one. Its derivative expression changes sign exactly once, from negative to positive, and hence

$$
\boxed{q_\tau=F^{-1}(\tau).}
$$

Equivalently the difference between the expected losses at $q$ and $q_\tau$ is $\int_{q_\tau}^q(F(t)-\tau)\,dt$, positive whenever $q\ne q_\tau$. This proves [population quantiles minimize check loss](../../../../../population-quantiles-minimize-check-loss.md) directly.

For the regression argument, define the [population risk](../../../../../population-risk.md) $M(\theta)=\mathbb E\rho_\tau(Y-g(X,\theta))$ and its empirical version $M_n(\theta)$. Boundedness of $g$ and integrability of the error give integrability of $Y$ and of all these losses. Conditional on $X=x$, the [conditional distribution](../../../../../conditional-distribution.md) of the error has unique $\tau$-[quantile](../../../../../quantile-function.md) zero. Applying the preceding calculation conditionally shows that its expected loss is uniquely minimized when the fitted displacement $g(x,\theta)-g(x,\theta_0)$ equals zero. Thus

$$
M(\theta)-M(\theta_0)\geq0,
$$

with strict inequality whenever that displacement is nonzero on an event of positive probability. The stated [identifiability](../../../../../identifiability.md) assumption therefore makes $\theta_0$ the unique population minimizer. This is [conditional quantile identification](../../../../../conditional-quantile-identification.md).

The Lipschitz property of the [check loss](../../../../../check-loss.md) gives

$$
|\rho_\tau(Y-g(X,\theta))-\rho_\tau(Y-g(X,\eta))|\leq |g(X,\theta)-g(X,\eta)|.
$$

Continuity of $g$ and its uniform bound, followed by [dominated convergence](../../../../../dominated-convergence-theorem.md), show that $M$ is continuous on $\Theta$.

For the intended estimator constrained to $\Theta$, here is the entire [argmin consistency under uniform convergence in probability](../../../../../argmin-consistency-under-uniform-convergence-in-probability.md) argument, rather than an invocation of an [M-estimator](../../../../../m-estimator.md) theorem. For a fixed $\varepsilon>0$, let $C_\varepsilon=\{\theta\in\Theta:\|\theta-\theta_0\|_2\geq\varepsilon\}$. If this set is empty, there is nothing to prove. Otherwise it is compact, and continuity and uniqueness give a strictly positive gap

$$
d_\varepsilon=\min_{\theta\in C_\varepsilon}(M(\theta)-M(\theta_0))>0.
$$

Let $D_n=\sup_{\theta\in\Theta}|M_n(\theta)-M(\theta)|$. If $\widehat\theta_n\in\Theta$ minimizes $M_n$, then

$$
M(\widehat\theta_n)\leq M_n(\widehat\theta_n)+D_n\leq M_n(\theta_0)+D_n\leq M(\theta_0)+2D_n.
$$

Consequently

$$
\mathbb P(\|\widehat\theta_n-\theta_0\|_2\geq\varepsilon)\leq\mathbb P(2D_n\geq d_\varepsilon)\longrightarrow0.
$$

**The constrained estimator is consistent.** Existence of a constrained minimum follows from continuity of the sample criterion and compactness. The argument applies to any measurable choice of minimizer.

There is an actual domain defect in the printed definition: its minimization is over all of $\mathbb R^p$, whereas the assumed [uniform convergence in probability](../../../../../uniform-convergence-in-probability.md) is only on $\Theta$. **That literal unconstrained consistency claim is false.** The preceding conclusion needs minimization over $\Theta$, or another assumption that confines the selected minimizers to a set where the convergence and separation arguments apply. No change of question heading is needed to make this qualification explicit.

Here is a counterexample satisfying even [identifiability](../../../../../identifiability.md) over the whole line. Take a constant covariate, independent standard normal errors, $\tau=1/2$, $\theta_0=0$, $\Theta=[-1,1]$, and

$$
g(x,\theta)=a(\theta)=\frac{\theta^2}{1+\theta^4}.
$$

This is bounded and continuous, has range $[0,1/2]$, and vanishes only at zero. The conditional error [distribution function](../../../../../cumulative-distribution-function.md) is continuous and strictly increasing with median zero. The compact-set [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md) also holds: the loss is $|Y-q|/2$, Lipschitz in $q$, so a finite grid in $[0,1/2]$ reduces its uniform difference to finitely many integrable sample averages plus an arbitrarily small grid error. The [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) then gives the asserted convergence.

Let $m_n$ be a [sample median](../../../../../sample-median.md), and put $c_n=\min(1/2,\max(0,m_n))$. Absolute loss over the range $[0,1/2]$ is minimized at $c_n$. Choose the following global empirical minimizer:

$$
\widehat\theta_n=\begin{cases}
0,&c_n=0,\\
\displaystyle\sqrt{\frac{1+\sqrt{1-4c_n^2}}{2c_n}},&0<c_n\leq1/2.
\end{cases}
$$

Solving the quadratic in $\theta^2$ shows $a(\widehat\theta_n)=c_n$, so this really minimizes the criterion over the whole line. For odd $n$, symmetry and continuity give $\mathbb P(m_n>0)=1/2$. Moreover $m_n\to0$ in probability: for each fixed positive $\delta$, the proportion of observations below $\delta$ converges to a number greater than one half, and the analogous proportion below $-\delta$ converges to a number less than one half. Therefore

$$
\mathbb P(\widehat\theta_n>1)\geq\mathbb P(0<m_n<1/2)\longrightarrow\frac12
$$

along odd $n$. The selected unconstrained estimator is not consistent. This illustrates why a [global argmin may escape a compact convergence set](../../../../../global-argmin-may-escape-a-compact-convergence-set.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
