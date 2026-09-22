<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a finite horizon $T$ and define $\tau_n=\inf\{s\ge0:|B_s|\ge n\}$. These [stopping times](../../../../../../stopping-time.md) increase to infinity almost surely because continuous paths are bounded on each finite interval. Applying the [Itô formula](../../../../../../ito-s-lemma.md) to $B_{t\wedge\tau_n}^k$, for $k\ge2$, gives

$$
B_{t\wedge\tau_n}^k=k\int_0^t\mathbf1_{\{s\le\tau_n\}}B_s^{k-1}\,dB_s+\frac{k(k-1)}2\int_0^t\mathbf1_{\{s\le\tau_n\}}B_s^{k-2}\,ds.
$$

The first integrand is bounded by $kn^{k-1}$, so its integral is square-integrable and has expectation zero. Thus

$$
\mathbb EB_{t\wedge\tau_n}^k=\frac{k(k-1)}2\mathbb E\int_0^t\mathbf1_{\{s\le\tau_n\}}B_s^{k-2}\,ds.
$$

To justify both limits explicitly, let $S_T=\sup_{s\le T}|B_s|$ and choose an integer $q>\max\{k,1\}$. The Gaussian density gives $\mathbb E|B_T|^q<\infty$ by its exponential tail. The [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md) states

$$
\mathbb ES_T^q\le\left(\frac q{q-1}\right)^q\mathbb E|B_T|^q<\infty.
$$

Therefore $S_T^k$ and $1+S_T^{k-2}$ are integrable. The stopped terminal powers converge almost surely to $B_t^k$ and are dominated in absolute value by $S_T^k$. The integrands in the time integral converge almost surely and are bounded by $1+S_T^{k-2}$, so their integrals are dominated by $T(1+S_T^{k-2})$. [Dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) on both sides, and then Fubini justified by the same bound, give the [Brownian moment recursion](../../../../../../brownian-moment-recursion.md)

$$
\boxed{\beta_k(t)=\frac{k(k-1)}2\int_0^t\beta_{k-2}(s)\,ds\qquad(k\ge2).}
$$

This uses only finiteness of Gaussian moments, not the closed moment formula requested in the next part.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
