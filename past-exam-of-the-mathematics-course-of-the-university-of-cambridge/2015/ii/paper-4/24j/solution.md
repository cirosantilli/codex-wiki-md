<h1 id="24j/solution">Solution</h1>

↑ **Parent:** [24J](../24j.md)

The nonparametric [bootstrap sample](../../../../../bootstrap-sample.md) is a sample of size $n$ drawn independently with replacement from the [empirical distribution](../../../../../type-information-theory.md) $\widehat F_n=n^{-1}\sum_i\delta_{X_i}$, conditional on the observed data. To simulate it, take independent uniform $U_j$ and set $X_j^b=X_{1+\lfloor nU_j\rfloor}$, assigning $U_j=1$ to the last index if it occurs in a finite-precision generator.

Let $G_n^b$ be the conditional [cumulative distribution function](../../../../../cumulative-distribution-function.md) of $\sqrt n(\bar X_n^b-\bar X_n)$, and let $q_n(p)=\inf\{t:G_n^b(t)\geq p\}$. A basic [bootstrap confidence interval](../../../../../bootstrap-confidence-interval.md) is

$$
\boxed{C_n=[\bar X_n-q_n(1-\alpha/2)/\sqrt n,\ \bar X_n-q_n(\alpha/2)/\sqrt n].}
$$

In practice the conditional quantiles are estimated from many simulated bootstrap means; the asymptotic argument below describes exact bootstrap quantiles or a simulation count tending to infinity.

For the required uniform-convergence fact, given $\epsilon>0$ choose $a<b$ with $F(a)<\epsilon$ and $1-F(b)<\epsilon$. By continuity, choose a finite mesh on $[a,b]$ with successive increases of $F$ less than $\epsilon$. Pointwise convergence at the mesh points makes $|F_n-F|<\epsilon$ there for large $n$. Monotonicity sandwiches both functions between their neighbouring mesh values, so $|F_n(t)-F(t)|<2\epsilon$ throughout $[a,b]$. The same monotonicity and the chosen tail bounds control the two exterior rays by $2\epsilon$. Hence $\sup_t|F_n(t)-F(t)|\to0$.

The [bootstrap consistency theorem for the sample mean](../../../../../bootstrap-consistency-theorem-for-the-sample-mean.md) states that, for iid observations with $0<\sigma^2<\infty$, the conditional law of $\sqrt n(\bar X_n^b-\bar X_n)$ converges weakly, in probability, to $N(0,\sigma^2)$. By continuity of that limiting distribution and the preceding monotonicity argument, the convergence of conditional distribution functions is uniform in probability. Since the limit is strictly increasing, $q_n(p)\to\sigma\Phi^{-1}(p)$ in probability for $0<p<1$. The coverage event is

$$
q_n(\alpha/2)\leq\sqrt n(\bar X_n-\mu)\leq q_n(1-\alpha/2).
$$

The [central limit theorem](../../../../../central-limit-theorem.md), quantile convergence and [Slutsky theorem](../../../../../slutsky-theorem.md) therefore give $\boxed{\mathbb P^{\mathbb N}(\mu\in C_n)\to1-\alpha}$.

**Positive variance is needed for this exact coverage conclusion.** If the finite variance allowed in the wording is zero, all observations equal $\mu$ almost surely and the interval collapses to $\{\mu\}$, with coverage one. The bootstrap distribution is still consistent with the degenerate limit, but a nonrandomized usual interval cannot then have limiting coverage $1-\alpha$ for $0<\alpha<1$.

## ↑ Ancestors (10)

1. [24J](../24j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
