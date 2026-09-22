<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The sampling rule in the PDF is with replacement. Thus conditional on the current proportion $y=j/n$, the next count is $W\sim\operatorname{Bin}(n,y)$. Put $\Delta=W/n-y$ and $q=y(1-y)$. Direct binomial moments give

$$
\mathbb E\Delta=0,\quad\mathbb E\Delta^2=q/n,\quad\mathbb E\Delta^4=3q^2/n^2+q(1-6q)/n^3\leq C/n^2.
$$

The [fourth centered moment of a binomial distribution](../../../../../../fourth-centered-moment-of-a-binomial-distribution.md) implies $\mathbb E|\Delta|^3\leq(\mathbb E\Delta^2\,\mathbb E\Delta^4)^{1/2}\leq Cn^{-3/2}$. The accelerated generator of the [Wright–Fisher binomial sampling chain](../../../../../../wright-fisher-binomial-sampling-chain.md) is

$$
A_nf(y)=n\mathbb E[f(y+\Delta)-f(y)].
$$

For $f\in C^3([0,1])$, Taylor's formula uniformly yields

$$
\boxed{\sup_{y\in\{0,1/n,\ldots,1\}}|A_nf(y)-\tfrac12y(1-y)f''(y)|\leq C_f n^{-1/2}\longrightarrow0.}
$$

The initial condition is $Z_0^n=\lfloor xn\rfloor$, so $X_0^n\to x$. The endpoints are absorbing.

We give the path-space argument, rather than only a formal generator calculation. Regard $X^n$ as a càdlàg process in $D([0,1],[0,1])$ with the Skorokhod $J_1$ topology. The chain proportion is a bounded [martingale](../../../../../../martingale-split.md), with predictable square compensator $V_t^n=n^{-1}\sum_{k<\lfloor nt\rfloor}X_{k/n}^n(1-X_{k/n}^n)$. For bounded [stopping times](../../../../../../stopping-time.md) $\tau_n\leq\sigma_n\leq\tau_n+\delta_n$, optional sampling gives $\mathbb E|X^n_{\sigma_n}-X^n_{\tau_n}|^2=\mathbb E(V^n_{\sigma_n}-V^n_{\tau_n})\leq(\delta_n+n^{-1})/4$. This bound uses the deterministic number of grid jumps in an interval of length at most $\delta_n$. Compact containment is automatic. The [Aldous tightness criterion](../../../../../../aldous-tightness-criterion.md) therefore proves tightness.

Furthermore, the fourth-moment bound and a union bound give

$$
\mathbb P\left(\max_{k<n}|X^n_{(k+1)/n}-X^n_{k/n}|>\epsilon\right)\leq C/(n\epsilon^4)\longrightarrow0.
$$

Every subsequential limit is continuous. For each smooth $f$, the discrete compensated process

$$
f(X_t^n)-f(X_0^n)-\frac1n\sum_{k<\lfloor nt\rfloor}A_nf(X_{k/n}^n)
$$

is a [martingale](../../../../../../martingale-split.md). Generator convergence and continuity of any limiting path turn the sum into $\int_0^t\tfrac12X_s(1-X_s)f''(X_s)ds$. These compensated processes are uniformly bounded on $[0,1]$, so their [martingale](../../../../../../martingale-split.md) identities pass to the limit against bounded continuous functions of past coordinates. A [Monotone class theorem](../../../../../../monotone-class-theorem.md) argument extends the identities to the natural filtration. Smooth approximation in the $C^2$ norm extends the test class. Thus every limit solves the [martingale](../../../../../../martingale-split.md) problem for $Lf(y)=\tfrac12y(1-y)f''(y)$ on $[0,1]$.

To identify this problem with the stated SDE, tests equal to $y$ and $y^2$ on $[0,1]$ (using bounded smooth extensions) give a continuous [martingale](../../../../../../martingale-split.md) with bracket $\int_0^tX_s(1-X_s)ds$. On an enlargement carrying independent [Brownian motion](../../../../../../brownian-motion-split.md) $W$, set

$$
B_t=\int_0^t\frac{\mathbf1_{\{X_s(1-X_s)>0\}}}{\sqrt{X_s(1-X_s)}}\,dX_s+\int_0^t\mathbf1_{\{X_s(1-X_s)=0\}}\,dW_s.
$$

Its bracket is $t$, and the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes it Brownian. The zero-coefficient portion of $dX$ has zero bracket, so $dX_t=\sqrt{X_t(1-X_t)}\,dB_t$. Conversely Itô's formula shows that any such SDE solution solves the limiting [martingale](../../../../../../martingale-split.md) problem. The allowed uniqueness of the SDE, understood at least as uniqueness in law, therefore makes every subsequential limit have the same law. Consequently

$$
\boxed{X^n\Rightarrow X\text{ in }D([0,1],[0,1]),\qquad dX_t=\sqrt{X_t(1-X_t)}\,dB_t,\quad X_0=x.}
$$

The limit is the [Wright–Fisher diffusion](../../../../../../wright-fisher-diffusion.md). Linear interpolation has the same weak limit in the uniform topology because the maximum jump tends to zero. The results applied are Aldous tightness, the vanishing-jump continuous-limit criterion, passage of uniformly bounded [martingale](../../../../../../martingale-split.md) identities under weak convergence, Lévy characterization, and uniqueness in law; the estimates above verify their hypotheses.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
