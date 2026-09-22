<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $X$ is a P-[Brownian motion](../../../../../../brownian-motion-split.md), its starting value is deterministic, so Q5(a) applies. The correction $[X,M]$ has [finite variation](../../../../../../total-variation-of-a-function.md) and does not alter [quadratic variation](../../../../../../quadratic-variation.md); Q1(b) gives $[\widetilde X]_t=t$ under Q. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) therefore identifies $\widetilde X$ as a Q-Brownian motion with the same starting value.

For the likelihood, use [Wiener measure](../../../../../../wiener-measure.md) $\mathbb Q^x$ as the reference measure and write its coordinate as $\omega_t=x+W_t$. Set

$$
M_t=-\mu\int_0^t\omega_s\,dW_s=-\mu\int_0^t\omega_s\,d\omega_s,
\qquad [M]_t=\mu^2\int_0^t\omega_s^2ds,
$$

and let $L=\mathcal E(M)$ be its [stochastic exponential](../../../../../../doleans-dade-exponential.md). We must prove it is a true [martingale](../../../../../../martingale-split.md); unverified large-horizon Novikov estimates would not suffice.

Fix $T$ and stop at $\tau_n=\inf\{s:|\omega_s|\ge n\}$, with $n>|x|$. The bounded integrand satisfies the [Novikov condition](../../../../../../novikov-s-condition.md), so $L_{T\wedge\tau_n}$ defines a probability $P_n$ on $\mathcal F_T$. By the result just established,

$$
W_s^{(n)}=W_s+\mu\int_0^{s\wedge\tau_n}\omega_rdr
$$

is Brownian under $P_n$ on this horizon. Therefore $d\omega_s=dW_s^{(n)}-\mu\mathbf1_{\{s\le\tau_n\}}\omega_sds$. The [Gronwall inequality](../../../../../../gronwall-inequality.md) gives

$$
\sup_{s\le T}|\omega_s|\le e^{|\mu|T}\left(|x|+\sup_{s\le T}|W_s^{(n)}|\right).
$$

The [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) then bounds its squared [expectation](../../../../../../expected-value.md) by $C_T=2e^{2|\mu|T}(x^2+4T)$, uniformly in $n$. In particular $P_n(\tau_n\le T)\le C_T/n^2$. On $\{\tau_n>T\}$ the stopped and unstopped densities agree, so

$$
\mathbb E_{\mathbb Q^x}\bigl[L_T\mathbf1_{\{\tau_n>T\}}\bigr]
=1-P_n(\tau_n\le T)\longrightarrow1.
$$

Continuous Brownian paths are bounded on $[0,T]$, and the indicators increase to one. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) proves $\mathbb E L_T=1$. Since a nonnegative [local martingale](../../../../../../local-martingale.md) is a supermartingale, constant [expectation](../../../../../../expected-value.md) at every time makes $L$ a true [martingale](../../../../../../martingale-split.md).

Under its tilted measure, $\widehat W_t=W_t+\mu\int_0^t\omega_sds$ is Brownian and $d\omega_t=d\widehat W_t-\mu\omega_tdt$. The explicit linear solution gives uniqueness of this law, identifying it with $\mathbb P^x$. Consequently the [Ornstein-Uhlenbeck likelihood relative to Wiener measure](../../../../../../ornstein-uhlenbeck-likelihood-relative-to-wiener-measure.md) is

$$
\boxed{\left.\frac{d\mathbb P^x}{d\mathbb Q^x}\right|_{\mathcal F_t}
=\exp\!\left(-\mu\int_0^t\omega_s\,d\omega_s-\frac{\mu^2}{2}\int_0^t\omega_s^2ds\right).}
$$

This is a finite-horizon density statement; it does not assert absolute continuity of the full infinite-horizon path laws.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
