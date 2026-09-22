<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [effective bandwidth](../../../../../effective-bandwidth.md) converts a traffic distribution and a quality-of-service requirement into a capacity requirement, penalizing bursts as well as mean load. Let $X\geq0$ be the traffic generated in one observation interval and assume its [moment-generating function](../../../../../moment-generating-function.md) is finite for some positive parameters. Write $\Lambda(s)=\log\mathbb E[e^{sX}]$. The [Chernoff bound](../../../../../chernoff-bound.md) follows immediately from [Markov's inequality](../../../../../markov-inequality.md) applied to $e^{sX}$:

$$
\mathbb P(X\geq b)\leq e^{-sb}\mathbb E[e^{sX}]=e^{-s[b-\alpha(s)]},\qquad \alpha(s)=\frac{\Lambda(s)}s,\quad s>0.
$$

Optimizing gives **$\boxed{\mathbb P(X\geq b)\leq\exp[-\sup_{s>0}\{sb-\Lambda(s)\}]}$**, where the supremum is restricted to finite exponential moments. This exhibits the [effective bandwidth](../../../../../effective-bandwidth.md) as the load appropriate to exponential tail control, not an extra physical stream of traffic.

For the [mean and peak limits of effective bandwidth](../../../../../mean-and-peak-limits-of-effective-bandwidth.md), if exponential moments exist near zero, the [cumulant-generating function](../../../../../cumulant-generating-function.md) expansion is

$$
\alpha(s)=\mathbb E X+\frac{s}{2}\operatorname{Var}(X)+\frac{s^2}{6}\kappa_3(X)+O(s^3).
$$

**For small $s$, $\boxed{\alpha(s)\to\mathbb E X}$**, with the [variance](../../../../../variance-split.md) giving the first burstiness correction. [convexity](../../../../../convex-function.md) of $\Lambda$ and $\Lambda(0)=0$ show that its secant slope $\alpha(s)$ is nondecreasing; [Jensen's inequality](../../../../../jensen-s-inequality.md) also gives $\alpha(s)\geq\mathbb E X$.

If $X$ is bounded with [essential supremum](../../../../../essential-supremum.md) $M$, then $\alpha(s)\leq M$. For any $a<M$, the probability $p_a=\mathbb P(X>a)$ is positive and

$$
\alpha(s)\geq a+\frac{\log p_a}{s}.
$$

Let $s\to\infty$ and then $a\uparrow M$. **For large $s$, $\boxed{\alpha(s)\to\operatorname{ess\,sup}X}$**, so very stringent exponential tail control approaches peak provisioning. If traffic is unbounded and every positive exponential moment is finite, the same lower-bound argument gives $\alpha(s)\to\infty$. If exponential moments cease to exist beyond a finite parameter, $\alpha$ is infinite there; one cannot assign a finite large-$s$ peak interpretation to that traffic.

For example, deterministic traffic $X=d$ has $\alpha(s)=d$. A burst of size $b$ with [Bernoulli distribution](../../../../../bernoulli-distribution.md) probability $p$ gives

$$
\alpha(s)=\frac1s\log(1-p+pe^{sb}),
$$

which moves from $pb$ to $b$. For Poisson packet count of mean $\lambda$ and packet size $b$, $\alpha(s)=\lambda(e^{sb}-1)/s$, showing a mean limit $\lambda b$ but no finite peak limit.

For independent traffic sources, logarithmic generating functions add, so [effective bandwidths](../../../../../effective-bandwidth.md) add. For arrivals $A_r(t)$ in a window of length $t$, use the rate-valued definition $\alpha_r(s,t)=\log\mathbb E[e^{sA_r(t)}]/(st)$. A resource with rate capacity $C$ then satisfies

$$
\mathbb P\left(\sum_r A_r(t)\geq Ct\right)\leq\exp\left[-st\left(C-\sum_r\alpha_r(s,t)\right)\right].
$$

Thus a sufficient admission condition for a target probability $\varepsilon$ is $\sum_r\alpha_r(s,t)\leq C-\log(1/\varepsilon)/(st)$ for some $s>0$. Independence is needed for this additive form; correlated sources require the joint exponential moment.

A queue involves a supremum over time windows, not merely one fixed window. For independent identically distributed discrete-time traffic increments $X_i$, constant service $C>\mathbb EX$, and stationary workload

$$
W=\sup_{n\geq0}\left(\sum_{i=1}^nX_i-nC\right),
$$

the [workload Chernoff bound for independent increments](../../../../../workload-chernoff-bound-for-independent-increments.md) follows from a [union bound](../../../../../boole-s-inequality.md):, whenever $a(s)=e^{\Lambda(s)-sC}<1$,

$$
\mathbb P(W>B)\leq e^{-sB}\sum_{n\geq1}a(s)^n=e^{-sB}\frac{a(s)}{1-a(s)}.
$$

The requirement is precisely $\alpha(s)<C$. This explains why [effective bandwidth](../../../../../effective-bandwidth.md) is useful for buffer and delay design: the relevant time scale and tail parameter depend on the service rule and target overflow risk. A single-window bound cannot be silently substituted for an infinite-horizon workload bound.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
