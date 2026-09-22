<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the independent-mark interpretation: the [Brownian motions](../../../../../../brownian-motion-split.md) attached to the atoms are [independent](../../../../../../independent-random-variables.md) of one another and of the initial [Poisson random measure](../../../../../../poisson-random-measure.md). Fix $t$ and define

$$
p_t(x)=\mathbb P\bigl(\exists s\in[0,t]:|x+\xi(s)-f(s)|\leq1\bigr).
$$

Conditionally on the initial atoms, each atom is retained as a dangerous atom if its own path meets the target by time $t$. These tests are [independent](../../../../../../independent-random-variables.md), with position-dependent retention [probability](../../../../../../probability.md) $p_t(x)$. The permitted [Poisson thinning](../../../../../../poisson-thinning.md) property makes the dangerous atoms a [Poisson random measure](../../../../../../poisson-random-measure.md) of intensity $p_t(x)\,dx$.

Its total intensity is computed without invoking a marking or displacement theorem. The event in the definition of $p_t(x)$ says that $x$ belongs to

$$
W_-(t)=\bigcup_{0\leq s\leq t}\mathcal B(f(s)-\xi(s),1).
$$

By the [Tonelli theorem](../../../../../../tonelli-theorem.md),

$$
\int_{\mathbb R^d}p_t(x)\,dx=\mathbb E\int_{\mathbb R^d}\mathbf1_{\{x\in W_-(t)\}}\,dx=\mathbb E\operatorname{vol}(W_-(t)).
$$

Symmetry of [Brownian motion](../../../../../../brownian-motion-split.md) gives $-\xi\stackrel d=\xi$ as processes. It therefore identifies the last [expectation](../../../../../../expected-value.md) with $\mathbb E\operatorname{vol}(W(t))$, where the sign of the deterministic path $f$ is unchanged. This swept set is a [Wiener sausage](../../../../../../wiener-sausage.md) with an added deterministic path.

The total intensity is finite on each bounded time interval. To see this explicitly, write $K_t=1+\sup_{s\leq t}|f(s)|$ and $R_t=\sup_{s\leq t}|\xi(s)|$. The sausage is contained in a ball of radius $K_t+R_t$. On a finite time grid, splitting according to the first crossing of a positive level $u$ by a one-dimensional [Brownian motion](../../../../../../brownian-motion-split.md) shows that the chance of ending above $u$, conditional on the crossing, is at least $1/2$: the remaining [independent](../../../../../../independent-random-variables.md) increment is symmetric. Thus the grid maximum exceeds $u$ with [probability](../../../../../../probability.md) at most twice the final Gaussian upper tail. Dense grids and continuity give the same bound for the path maximum. Applying this to each coordinate and its negative gives

$$
\mathbb P(R_t>u)\leq4d\,\mathbb P(N(0,t)>u/\sqrt d)\leq4d\,e^{-u^2/(2dt)}\qquad(t>0).
$$

The last inequality follows from $\mathbb E e^{\theta N(0,t)}=e^{\theta^2t/2}$ and minimizing the exponential Markov bound. Integration of this tail gives finite moments of $R_t$ of every positive order, so $\mathbb E\operatorname{vol}(W(t))<\infty$.

There are consequently only finitely many dangerous atoms on each compact time interval, almost surely. For closed balls, continuity of the paths makes each finite hitting-time infimum attained. The event $T>t$ is therefore the absence of dangerous atoms up to time $t$.

The open-ball convention has the same survival [probability](../../../../../../probability.md) at each fixed $t$. Indeed for any compact path range $K$, the difference between its closed and open radius-one neighborhoods is the shell $\{x:\operatorname{dist}(x,K)=1\}$, which has zero [Lebesgue measure](../../../../../../lebesgue-measure.md). To see this, choose a nearest $y\in K$ for a shell point $x$. For every sufficiently small $\varepsilon>0$, the ball of radius $\varepsilon/2$ centered at $x-\varepsilon(x-y)$ lies in the open neighborhood and inside the ball of radius $3\varepsilon/2$ about $x$. Thus the shell has a fixed proportional hole at every scale; the [Lebesgue density theorem](../../../../../../lebesgue-s-density-theorem.md) forces its measure to be zero. By the [Tonelli theorem](../../../../../../tonelli-theorem.md), closed-touch and open-entry retention probabilities have equal integrals. Independent thinning therefore gives no atom that touches only the boundary before this fixed horizon, almost surely. This also excludes a difference at an open-entry infimum equal to $t$.

 The zero-count [probability](../../../../../../probability.md) of a [Poisson distribution](../../../../../../poisson-distribution.md) is $e^{-\lambda}$, and hence

$$
\boxed{\mathbb P(T>t)=\exp\{-\mathbb E\operatorname{vol}(W(t))\}.}
$$

This [survival among independently moving Poisson traps](../../../../../../survival-among-independently-moving-poisson-traps.md) formula has been derived using only [independent](../../../../../../independent-random-variables.md) thinning and the defining Poisson zero-count [probability](../../../../../../probability.md), with the [expectation](../../../../../../expected-value.md)/volume step supplied by Tonelli's theorem.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
