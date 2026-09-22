<h1 id="b/7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[put-call parity](../../../../../put-call-parity.md) and nonnegativity of the [European put option](../../../../../european-put-option.md) give

$$
C^E=P^E+S-Ke^{-r\tau}\geq\boxed{S-Ke^{-r\tau}}.
$$

For $r\geq0$ this is at least $S-K$, and the call value is also nonnegative, so $C^E$ dominates the immediate call exercise [contingent claim payoff](../../../../../contingent-claim-payoff.md). Its discounted price is a [martingale](../../../../../martingale-split.md). At any admissible exercise time, [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) therefore bounds the expected discounted [call option](../../../../../call-option.md) by the [European call option](../../../../../european-call-option.md) price. Exercising at maturity attains that price. Hence **American and European calls coincide** for this non-dividend model with nonnegative rates.

For the strict put comparison assume $r>0$, $\sigma>0$, $S>0$ and $t<T$. Choose $u$ strictly between $t$ and $T$. A [European put option](../../../../../european-put-option.md) at $u$ has value at most $Ke^{-r(T-u)}$. On the event

$$
S_u<K(1-e^{-r(T-u)}),
$$

immediate exercise gives $K-S_u>Ke^{-r(T-u)}\geq P^E(u,S_u)$. This event has positive probability because the [lognormal](../../../../../log-normal-distribution.md) stock density is positive on $(0,\infty)$. Exercise there at time $u$, and otherwise hold to maturity. This strategy strictly improves the [European put option](../../../../../european-put-option.md) [expected value](../../../../../expected-value-split.md), proving

$$
\boxed{P^A(t,S)>P^E(t,S)}
$$

under these positive-rate, pre-maturity assumptions.

The source's strict statement needs those qualifications. At maturity the prices agree, and at $r=0$ the [put option](../../../../../put-option.md) is a [convex function](../../../../../convex-function.md) of the [martingale](../../../../../martingale-split.md) stock and therefore is a [submartingale](../../../../../submartingale.md), so waiting to maturity is optimal and the American and European puts coincide. Negative rates also invalidate the nonnegative-rate call argument. These are mathematical assumptions of the comparison, rather than changes to the printed question.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
