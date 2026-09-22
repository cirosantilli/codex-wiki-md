<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To avoid confusing the [continuous-time bank account](../../../../../../continuous-time-bank-account.md) with the coefficient of $r_t$, denote the latter by $b(\tau)$ and the other coefficient by $a(\tau)$, where $\tau=T-t$. Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $D_t[a(\tau)+b(\tau)r_t]$. Since the expression is affine in $r$, its second rate derivative is zero. Its drift is

$$
D_t\left[-a'(\tau)-b'(\tau)r_t+b(\tau)r_t(r_t-1)
-r_t(a(\tau)+b(\tau)r_t)\right]dt.
$$

The quadratic terms cancel. The remaining expression is

$$
D_t\{-a'(\tau)+[-b'(\tau)-a(\tau)-b(\tau)]r_t\}\,dt.
$$

It vanishes when $a'=0$ and $b'=-a-b$. For a unit bond payoff choose terminal conditions $a(0)=1$, $b(0)=0$, giving

$$
\boxed{a(\tau)=1,\qquad b(\tau)=e^{-\tau}-1.}
$$

The resulting [local martingale](../../../../../../local-martingale.md) is $D_t[1-(1-e^{-\tau})r_t]$. The allowed bound $0\leq r_t\leq1$ puts it between zero and one, so the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes it a true [martingale](../../../../../../martingale-split.md). At maturity it equals $D_T$. Comparing with part (a) therefore gives

$$
\boxed{P(t,T)=1-(1-e^{-(T-t)})r_t.}
$$

In particular $e^{-(T-t)}\leq P(t,T)\leq1$, and $P(T,T)=1$. This is [linear bond pricing in a bounded short-rate diffusion](../../../../../../linear-bond-pricing-in-a-bounded-short-rate-diffusion.md); choosing zero coefficients would produce a [local martingale](../../../../../../local-martingale.md) but would not price the required terminal payoff.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
