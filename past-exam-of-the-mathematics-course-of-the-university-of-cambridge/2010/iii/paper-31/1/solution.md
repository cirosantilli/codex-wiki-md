<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [empirical distribution function](../../../../../empirical-distribution-function.md) is

$$
\boxed{F_n(t)=\frac1n\sum_{i=1}^n\mathbf1_{\{X_i\leq t\}},\qquad t\in\mathbb R.}
$$

If $W$ is a standard [Brownian motion](../../../../../brownian-motion-split.md) on $[0,1]$, the standard [Brownian bridge](../../../../../brownian-bridge.md) is $\mathbb G(u)=W(u)-uW(1)$. It is a centred [Gaussian process](../../../../../gaussian-process.md) with continuous paths, endpoints zero, and [covariance](../../../../../covariance.md)

$$
\mathbb E[\mathbb G(u)\mathbb G(v)]=\min(u,v)-uv.
$$

The [F-Brownian bridge](../../../../../f-brownian-bridge.md) is the time-changed [Gaussian process](../../../../../gaussian-process.md) $\mathbb G_F(t)=\mathbb G(F(t))$. Its [covariance](../../../../../covariance.md) is $F(\min(s,t))-F(s)F(t)$, exactly the covariance of the [empirical distribution process](../../../../../empirical-distribution-process.md) $\alpha_n=\sqrt n(F_n-F)$.

The [Donsker theorem for empirical distribution functions](../../../../../donsker-theorem-for-empirical-distribution-functions.md) states that for every [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F$,

$$
\boxed{\sqrt n(F_n-F)\ \rightsquigarrow\ \mathbb G_F\quad\text{in }\ell^\infty(\mathbb R),\text{ with the supremum norm}.}
$$

Thus this is a function-space [central limit theorem](../../../../../central-limit-theorem.md), not merely convergence of each finite collection of evaluations. The limit is a tight centred [Gaussian process](../../../../../gaussian-process.md). No continuity of $F$ is required for this statement; a jump of $F$ can give a jump of $\mathbb G_F$.

For precision, $\ell^\infty(\mathbb R)$ is generally nonseparable, and the finite-sample process need not be a Borel-measurable random element for its norm topology. The displayed [convergence in distribution](../../../../../convergence-in-distribution.md) has the usual empirical-process interpretation: for every bounded continuous real functional $H$, the [outer expectation](../../../../../outer-expectation.md) and inner expectation of $H(\alpha_n)$ converge to $\mathbb EH(\mathbb G_F)$. The [outer expectation](../../../../../outer-expectation.md) is the infimum of expectations of measurable majorants, and the inner expectation is its negative applied to $-H(\alpha_n)$. For measurable real statistics this gives ordinary [convergence in distribution](../../../../../convergence-in-distribution.md). The limit is tight and separably supported: $g\mapsto g\circ F$ maps the separable space of continuous bridge paths continuously into $\ell^\infty(\mathbb R)$.

The map $z\mapsto\|z\|_\infty$ is Lipschitz, since

$$
\bigl|\|z\|_\infty-\|w\|_\infty\bigr|\leq\|z-w\|_\infty.
$$

Consequently the [continuous mapping theorem](../../../../../continuous-mapping-theorem.md) applied to the [Donsker theorem for empirical distribution functions](../../../../../donsker-theorem-for-empirical-distribution-functions.md) gives $\|\alpha_n\|_\infty\xrightarrow d\|\mathbb G_F\|_\infty$. The statistic on the left is measurable: both $F_n$ and $F$ are right-continuous, so its supremum equals the supremum over rational $t$.

If $F$ is continuous, its limits at $-\infty$ and $+\infty$ are zero and one. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) therefore shows that $F(\mathbb R)$ contains $(0,1)$, even when $F$ is not strictly increasing. A continuous [Brownian bridge](../../../../../brownian-bridge.md) is zero at its endpoints, so pathwise

$$
\sup_{t\in\mathbb R}|\mathbb G(F(t))|=\sup_{0<u<1}|\mathbb G(u)|=\max_{0\leq u\leq1}|\mathbb G(u)|.
$$

We obtain the [Kolmogorov-Smirnov theorem](../../../../../kolmogorov-smirnov-theorem.md) in the required form:

$$
\boxed{\sqrt n\sup_{t\in\mathbb R}|F_n(t)-F(t)|\xrightarrow d Z,\qquad Z=\max_{0\leq u\leq1}|\mathbb G(u)|.}
$$

Continuity of $F$ is what makes the limit independent of the unknown [cumulative distribution function](../../../../../cumulative-distribution-function.md).

Choose $c_\alpha$ with $\mathbb P(Z\leq c_\alpha)=1-\alpha$. The law of $Z$ has no atoms. For example, the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) and conditioning a [Brownian motion](../../../../../brownian-motion-split.md) on its endpoint give $\mathbb P(\max\mathbb G>a)=e^{-2a^2}$ for $a>0$: the reflected endpoint density at zero is the normal density at $2a$, divided by its value at zero. Hence both one-sided maxima have continuous laws, and an atom of $Z$ would require an atom of one of them. Also $\mathbb P(Z=0)=0$, since $\mathbb G(1/2)$ is nondegenerate. Thus such quantiles give the desired limiting coverage.

An asymptotic simultaneous [confidence band](../../../../../confidence-band.md) is

$$
\boxed{L_n(t)=\max\{0,F_n(t)-c_\alpha/\sqrt n\},\qquad U_n(t)=\min\{1,F_n(t)+c_\alpha/\sqrt n\}.}
$$

Indeed, because $0\leq F\leq1$, the event that $L_n(t)\leq F(t)\leq U_n(t)$ for every $t$ is precisely $\sqrt n\|F_n-F\|_\infty\leq c_\alpha$. Its [probability](../../../../../probability.md) tends to $1-\alpha$. This is simultaneous coverage over all real $t$, rather than separate pointwise [confidence intervals](../../../../../confidence-interval.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
