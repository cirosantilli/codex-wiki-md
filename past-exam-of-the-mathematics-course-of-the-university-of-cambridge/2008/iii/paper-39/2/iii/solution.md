<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $Q$ be the unique [equivalent martingale measure](../../../../../../risk-neutral-measure.md). The [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) formula is

$$
C(T,K)=B_0\mathbb E_Q\left[\frac{(S_T-K)^+}{B_T}\right]=B_0\mathbb E_Q[(M_T-K/B_T)^+],\qquad M_t=S_t/B_t.
$$

For the usual nonnegative strike $K$ and maturities $u\geq t$, the monotonic [bank account](../../../../../../bank-account.md) gives $K/B_u\leq K/B_t$. Therefore

$$
\begin{aligned}\mathbb E_Q[(M_u-K/B_u)^+\mid\mathcal F_t]&\geq\mathbb E_Q[(M_u-K/B_t)^+\mid\mathcal F_t]\\&\geq(\mathbb E_Q[M_u\mid\mathcal F_t]-K/B_t)^+\\&=(M_t-K/B_t)^+.
\end{aligned}
$$

The second inequality follows directly since the [conditional expectation](../../../../../../conditional-expectation.md) of a [positive part](../../../../../../positive-part-of-a-real-valued-function.md) is at least both zero and the [conditional expectation](../../../../../../conditional-expectation.md) of its argument; it is also conditional [Jensen's inequality](../../../../../../jensen-s-inequality.md). Taking [expectations](../../../../../../expected-value.md) proves $C(u,K)\geq C(t,K)$, the [maturity monotonicity of calls with nonnegative strikes](../../../../../../maturity-monotonicity-of-calls-with-nonnegative-strikes.md).

If $K_1\leq K_2$, then $(S_T-K_1)^+\geq(S_T-K_2)^+$ pointwise; positive discounting and [expectation](../../../../../../expected-value.md) prove [monotonicity of a European call price in strike](../../../../../../monotonicity-of-a-european-call-price-in-strike.md). For $0\leq a\leq1$, the pointwise inequality

$$
(S_T-aK_1-(1-a)K_2)^+\leq a(S_T-K_1)^++(1-a)(S_T-K_2)^+
$$

gives [convexity of a European call price in strike](../../../../../../convexity-of-a-european-call-price-in-strike.md) after the same operations. Hence

$$
\boxed{C(T,K)\text{ is nondecreasing in }T,\text{ nonincreasing and convex in }K.}
$$

The maturity assertion uses $K\geq0$; it need not hold for a negative strike. For example, in the deterministic [complete market](../../../../../../complete-market.md) $S_t=B_t=e^{rt}$ with $r>0$, a negative-strike call has price $1-Ke^{-rT}$, which decreases with $T$. The monotonicity assertions are non-strict, as equality can occur.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
