<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [barrier-triggered put](../../../../../barrier-triggered-put.md) exercises at the particular [stopping time](../../../../../stopping-time.md) $\tau_B\wedge T$. The [American put option](../../../../../american-put-option.md) optimizes over all allowed exercise times, so

$$
\boxed{E_B(S,t)\leq A(S,t;K).}
$$

It can be strictly smaller, but can never exceed the American value. Equality is possible if immediate exercise is already triggered and optimal; a fixed barrier is not generally the optimal finite-maturity exercise rule.

The comparison with the [European put option](../../../../../european-put-option.md) can go in either direction. By the [early exercise premium for a fixed barrier](../../../../../early-exercise-premium-for-a-fixed-barrier.md),

$$
E_B(S,t)-P(S,t;K)=\mathbb E_{\mathbb Q}\!\left[e^{-r(\tau_B-t)}
\{K-B-P(B,\tau_B;K)\}\mathbf1_{\{\tau_B\leq T\}}\mid S_t=S\right].
$$

Thus an early payment gains interest but sacrifices remaining put time value; the expression inside braces need not have a fixed sign for arbitrary barriers.

For a concrete general construction take current spot $S\geq K$, $r>0$, $\sigma>0$, and $t<T$. Set $\gamma=2r/\sigma^2$ and $b_\infty=K\gamma/(1+\gamma)$, the [perpetual put option](../../../../../perpetual-put-option.md) exercise boundary. For $0<B<b_\infty$, the perpetual value at $B$ equals $K-B$ and strictly dominates the finite-maturity European value. The premium formula and positive probability of hitting $B$ therefore give **$E_B>P$**. Strictness follows from the perpetual verification argument: before a fixed positive expiry, its discounted value loses drift $rK$ whenever the stock is below $b_\infty$, with positive expected occupation time when started at $B<b_\infty$.

Conversely, for $B<K$ sufficiently close to $K$, every possible payment of the exploding put is at most $K-B$, whether paid at touch or on surviving to expiry. Hence $0\leq E_B\leq K-B\to0$, while $P(S,t;K)>0$. This gives **$E_B<P$** for such barriers, and also strict inequality below the American value.

These examples establish both possibilities in general, not a claim that every fixed initial state admits both. If $S<b_\infty$ and only alive barriers $B<S$ are allowed, all those barriers are in the same perpetual stopping region and the premium comparison is nonnegative.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
