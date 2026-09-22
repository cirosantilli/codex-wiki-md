<h1 id="b/8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At maturity debt receives the smaller of face value and firm assets:

$$
D_T=\min(F,V_T)=F-(F-V_T)_+.
$$

Thus it is equivalent to a zero-coupon payment $F$ minus a [European put option](../../../../../european-put-option.md) on the firm value. Its time-$t$ price is

$$
\boxed{D_t=Fe^{-r(T-t)}-P^E(t,V_t;F).}
$$

Equity receives the residual $(V_T-F)_+$, hence is a [European call option](../../../../../european-call-option.md):

$$
\boxed{E_t=C^E(t,V_t;F).}
$$

[put-call parity](../../../../../put-call-parity.md) verifies $E_t+D_t=V_t$, consistent with the stated balance-sheet identity. As with the replication arguments elsewhere, the physical drift $\mu$ does not enter these option prices.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
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
