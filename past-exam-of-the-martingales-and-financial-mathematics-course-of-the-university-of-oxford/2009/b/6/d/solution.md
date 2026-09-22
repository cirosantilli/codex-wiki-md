<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [exchange option](../../../../../exchange-option.md) has terminal payoffs determined by the two successive up/down moves:

$$
\begin{array}{c|c|c|c}
\text{path}&S_1(2)&S_2(2)&(S_1(2)-S_2(2))^+\\ \hline
uu&196&144&52\\
ud,\ du&112&108&4\\
dd&64&81&0
\end{array}
$$

The two stocks span both one-step states, so this finite market is complete. The [risk-neutral pricing](../../../../../risk-neutral-pricing.md) uses the independent transition probabilities $q=1/3$ and $1-q=2/3$. Since the synthetic risk-free rate is zero,

$$
V_0=\frac19\,52+2\left(\frac13\frac23\right)4+\frac49\,0
=\boxed{\frac{68}{9}}.
$$

The price is approximately 7.56 in the currency units of the stock prices.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
