# Four-cycle partition function

↑ **Parent:** [Stationary law of a proportionally fair four-cycle](stationary-law-of-a-proportionally-fair-four-cycle.md)

For offered loads on consecutive routes $a,b,c,d$ of the reversible [proportionally fair allocation on a four-cycle](proportionally-fair-allocation-on-a-four-cycle.md), the normalizing sum of the [stationary distribution](stationary-distribution.md) is

$$
B=\frac{(1-a)(1-b)(1-c)(1-d)-abcd}{(1-a-b)(1-a-d)(1-c-b)(1-c-d)}.
$$

This formula applies in the [stability region for the reversible four-cycle flow network](stability-region-for-the-reversible-four-cycle-flow-network.md). Grouping populations on opposite routes gives $\sum_{s,t}\binom{s+t}{s}h_s(a,c)h_t(b,d)$, where $h_s(a,c)=\sum_{i=0}^sa^ic^{s-i}$. For distinct opposite loads, substituting $h_s=(a^{s+1}-c^{s+1})/(a-c)$ and summing the four geometric generating series proves the formula; [continuity](continuous-function.md) covers coincident loads. If all four loads equal $z<1/2$, it reduces to $(1-2z+2z^2)/(1-2z)^3$.

## ↑ Ancestors (10)

1. [Stationary law of a proportionally fair four-cycle](stationary-law-of-a-proportionally-fair-four-cycle.md)
2. [Balance function of a flow-level network](balance-function-of-a-flow-level-network.md)
3. [Flow-level network model](flow-level-network-model.md)
4. [Stochastic network](stochastic-network.md)
5. [Queueing theory](queueing-theory-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34/4/solution.md)
