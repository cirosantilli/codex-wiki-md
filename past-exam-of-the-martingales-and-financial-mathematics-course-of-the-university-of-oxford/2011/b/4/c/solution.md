<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The terminal stock prices and [European put option](../../../../../european-put-option.md) payoffs are

$$
\begin{array}{c|ccc}
\text{state}&uu&ud,du&dd\\\hline
S_2&144&108&81\\
(117-S_2)^+&0&9&36.
\end{array}
$$

Let $q$ be the risk-neutral up probability. [Risk-neutral pricing](../../../../../risk-neutral-pricing.md) and the supplied discounted-price condition give

$$
8=e^{2r}V_0=18q(1-q)+36(1-q)^2,
$$

so $9q^2-27q+14=0$. Its roots are $2/3$ and $7/3$; only the first is a probability. Therefore

$$
\boxed{q=\frac23,\qquad e^r=0.9+0.3q=1.1,\qquad r=\log1.1.}
$$

The current put price is $V_0=8/1.1^2=800/121$ pounds. This interest rate is specific to part (c), and differs from the zero rate in part (b).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
