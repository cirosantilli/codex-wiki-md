<h1 id="b/7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At an entry date the holder chooses between entering the at-the-money call immediately and retaining the right to choose at the next date. The [Snell envelope](../../../../../snell-envelope.md) therefore gives, under [risk-neutral valuation](../../../../../risk-neutral-pricing.md),

$$
B^{FSC}(T_i,s)=\max\left\{s\,c(T-T_i),
e^{-r(T_{i+1}-T_i)}
\mathbb E[B^{FSC}(T_{i+1},S_{T_{i+1}})\mid S_{T_i}=s]\right\},
$$

with terminal value zero if entry has never occurred.

[homogeneous function](../../../../../homogeneous-function.md) makes $B^{FSC}(T_i,s)=s b_i$. The discounted stock [expected value](../../../../../expected-value-split.md) is $s$, so the recursion reduces to

$$
\boxed{b_{N+1}=0,\qquad
b_i=\max\{c(T-T_i),b_{i+1}\}
=\max_{j\geq i}c(T-T_j).}
$$

In the positive-rate case in the hint, put $\gamma=r/\sigma$ and $\beta=\sigma/2$. Then $c(u)$ is exactly its increasing function. The largest remaining maturity is $T-T_i$, so $b_i=c(T-T_i)$: immediate entry is optimal at every date while unentered.

At time zero this yields

$$
\boxed{B^{FSC}(0,S_0)=S_0c(T)
=C(0,S_0;T,S_0).}
$$

Thus the Bermudan choice of start date adds no value over the ordinary at-the-money [European call option](../../../../../european-call-option.md) in this setting. The maximum formula remains the general recursion; using monotonicity to select immediate entry uses the rate assumption supplied with the hint. This is [immediate entry for a Bermudan forward-start call](../../../../../immediate-entry-for-a-bermudan-forward-start-call.md).

## ↑ Ancestors (13)

1. [D](../d.md)
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
