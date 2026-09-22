# Replicating portfolio in a binomial market

↑ **Parent:** [Discrete-time binomial market](discrete-time-binomial-market.md)

Let $c_0$ be the initial monetary balance in the [bank account](bank-account.md), negative for borrowing. Matching successor [financial payoffs](contingent-claim-payoff.md) gives the [linear system](system-of-linear-equations.md)

$$
\Delta S_u+Rc_0=V_u,\qquad \Delta S_d+Rc_0=V_d.
$$

Subtracting determines the stock holding $\Delta$ in the header; substitution determines $c_0$. The initial cost is $V_0=\Delta S_0+c_0$. For the [European call option](european-call-option.md) with $S_u=120$, $S_d=80$, [strike price](strike-price.md) 100 and payoffs 20 and zero,

$$
\Delta=\frac{20-0}{120-80}=\frac12,\qquad c_0=\frac{0-(1/2)80}{21/20}=-\frac{800}{21},\qquad V_0=50-\frac{800}{21}=\frac{250}{21}.
$$

The debt becomes 40 at maturity: half a share minus 40 yields $60-40=20$ in the up state and $40-40=0$ in the down state. Holding these positions until maturity is [self-financing](self-financing-portfolio.md). Repeating this two-equation construction at earlier nodes gives [backward option pricing](backward-option-pricing.md) and the unique price in the [complete market](complete-market.md).

<a id="image-a-half-share-position-and-a-debt-of-800-21-reproduce-the-call-payoff-in-both-states"></a>
![](binomial-option-replication.png)

**[Figure 2](#image-a-half-share-position-and-a-debt-of-800-21-reproduce-the-call-payoff-in-both-states). A half-share position and a debt of 800/21 reproduce the call payoff in both states**.

The discrete replication method was developed in Cox, Ross and Rubinstein's 1979 paper, whose Sections 2–3 explain borrowing, statewise matching and why physical [probability](probability.md) drops out of relative option valuation. Their symbols for physical and pricing [probabilities](probability.md) differ from the $p,q$ convention here. [Cox, Ross and Rubinstein, Option Pricing: A Simplified Approach (1979), Sections 2–3](https://bpb-us-w2.wpmucdn.com/u.osu.edu/dist/7/36891/files/2017/07/CRR79-1yy8av8.pdf)

**Table of contents**

- [Convex-payoff delta monotonicity in a binomial market](convex-payoff-delta-monotonicity-in-a-binomial-market.md)
- [Backward option pricing](backward-option-pricing.md)

## ↑ Ancestors (7)

1. [Discrete-time binomial market](discrete-time-binomial-market.md)
2. [Binomial options pricing model](binomial-options-pricing-model.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (9)

- [American quadratic-payoff option in a binomial market](american-quadratic-payoff-option-in-a-binomial-market.md)
- [Convex-payoff delta monotonicity in a binomial market](convex-payoff-delta-monotonicity-in-a-binomial-market.md)
- [Mathematical finance](mathematical-finance-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/29k/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/29k/b/solution.md)
