<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the usual asymptotic convention: the output approaches the desired $m(n)$-copy pure target in [trace distance](../../../../../../trace-distance.md), and any recorded failure probability tends to zero. Define the [binary entropy](../../../../../../binary-entropy.md)

$$
h_2(x)=-x\log_2x-(1-x)\log_2(1-x).
$$

The [entanglement entropies](../../../../../../entanglement-entropy.md) per source and target are $E_\psi=h_2(s)$ and $E_\phi=h_2(t)$. The [asymptotic pure-state entanglement conversion rate](../../../../../../asymptotic-pure-state-entanglement-conversion-rate.md) is

$$
\boxed{R_{\max}=\frac{h_2(\sin^2\alpha)}{h_2(\sin^2\beta)}.}
$$

Both achievability and the upper bound matter here.

For [entanglement concentration](../../../../../../entanglement-concentration.md), expand $n$ sources in their correlated computational basis. Every pair of strings of [Hamming weight](../../../../../../hamming-weight.md) $k$ has the same amplitude $(1-s)^{(n-k)/2}s^{k/2}$. Alice measures only this weight, without resolving the individual string. Bob's string has the same weight automatically. Conditional on $k$, the normalized state is maximally entangled on $D_k=\binom nk$ correlated strings. Its outcome probability is $\binom nk s^k(1-s)^{n-k}$, a [binomial distribution](../../../../../../binomial-distribution.md). By the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md), $k/n\to s$ in probability; [Stirling's formula](../../../../../../stirling-formula.md) then gives $n^{-1}\log_2D_k\to h_2(s)$. A uniform Schmidt vector on $D_k$ entries is majorized by a uniform vector on $2^{\lfloor\log_2D_k\rfloor}$ entries padded with zeros. Thus [Nielsen's pure-state conversion theorem](../../../../../../nielsen-s-pure-state-conversion-theorem.md) converts the conditional state into that many [Bell pairs](../../../../../../bell-pair.md) exactly. For any fixed $\delta>0$, one obtains at least $n(E_\psi-\delta)$ Bell pairs with probability tending to one.

For [entanglement dilution](../../../../../../entanglement-dilution.md), consider the Schmidt strings of $m$ targets with probabilities $q_x$. The [quantum typical subspace](../../../../../../quantum-typical-subspace.md) retains strings satisfying

$$
2^{-m(E_\phi+\delta)}\leq q_x\leq2^{-m(E_\phi-\delta)}.
$$

The retained probability $Q_m$ tends to one by the weak law applied to the independent variables $-\log_2q_{x_j}$. The number of retained strings is at most $2^{m(E_\phi+\delta)}$, because their probabilities sum to at most one. Normalize the target after truncation to those strings. Its squared overlap with the full target is $Q_m\to1$. A uniform Schmidt vector of dimension $2^L$, with $L=\lceil m(E_\phi+\delta)\rceil$, is majorized by the truncated target's Schmidt vector padded with zeros: the sum of its largest $k$ entries is at least $k/2^L$. Hence $L$ Bell pairs prepare the truncated target exactly by [LOCC](../../../../../../local-operations-and-classical-communication.md). Its trace distance from the true target is $\sqrt{1-Q_m}\to0$. Combining concentration and dilution achieves any rate $R<E_\psi/E_\phi$. Choosing margins tending sufficiently slowly to zero attains the ratio as a limiting rate.

For the converse, [average monotonicity of pure-state entanglement entropy](../../../../../../average-monotonicity-of-pure-state-entanglement-entropy.md) follows from [Concavity of Von Neumann entropy](../../../../../../concavity-of-von-neumann-entropy.md): a measurement by one party leaves the other party's reduction unchanged on average, so its average conditional entropy cannot increase. Refine local measurement records, including local discarded systems, to obtain pure output branches $\{p_r,|\chi_r\rangle\}$ on the $m$ output qubits of each party. Iterating the concavity argument gives

$$
\sum_r p_r E(\chi_r)\leq nE_\psi.
$$

Let $|\Phi_m\rangle=|\phi\rangle^{\otimes m}$ and let the squared-overlap error of the average output $\rho_{\rm out}$ be $\varepsilon=1-\langle\Phi_m|\rho_{\rm out}|\Phi_m\rangle\to0$. Define $d_r=\sqrt{1-|\langle\Phi_m|\chi_r\rangle|^2}$, the pure-state [trace distance](../../../../../../trace-distance.md). Concavity of the square root gives $\sum_rp_rd_r\leq\sqrt\varepsilon$. Partial trace cannot increase trace distance, so the reduced states are also within $d_r$. The [continuity bound for quantum conditional entropy](../../../../../../continuity-bound-for-quantum-conditional-entropy.md), with trivial conditioning and local dimension $2^m$, implies

$$
|E(\chi_r)-mE_\phi|\leq2m d_r+g(d_r),\qquad
g(d)=(1+d)h_2\!\left(\frac d{1+d}\right)\leq2.
$$

Consequently

$$
nE_\psi\geq mE_\phi-2m\sqrt\varepsilon-2,
$$

which excludes a limiting rate exceeding $E_\psi/E_\phi$.

The vanishing-error convention is essential. If exact deterministic conversion were required for every finite block, [majorization](../../../../../../majorization.md) would also require the largest squared Schmidt coefficient to satisfy $(1-s)^n\leq(1-t)^m$, hence

$$
\frac mn\leq\frac{-\log(1-s)}{-\log(1-t)}.
$$

This can be strictly smaller than the entropy ratio: at $s=0.1,t=0.2$, the two bounds are approximately $0.4722$ and $0.6496$. Thus the boxed rate answers the standard asymptotic task, rather than imposing unmentioned exact zero-error conditions on every finite block.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
