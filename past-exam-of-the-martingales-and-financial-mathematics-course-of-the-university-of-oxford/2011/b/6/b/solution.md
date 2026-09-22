<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the accumulated bank account from past dividends be

$$
A_t=\int_0^t0.01S_u e^{0.05(t-u)}\,du.
$$

Holding one stock share and banking its dividends is a [self-financing portfolio](../../../../../self-financing-portfolio.md) with wealth $X_t=S_t+A_t$ and $dA_t=0.05A_tdt+0.01S_tdt$. Doubling that strategy replicates the specified terminal payoff. Its price is therefore

$$
\boxed{\text{price at }t=2X_t=2S_t+2\int_0^t0.01S_u e^{0.05(t-u)}\,du.}
$$

In particular its initial price is one hundred pounds. This illustrates [banking stock dividends versus reinvesting them](../../../../../banking-stock-dividends-versus-reinvesting-them.md). The accrued-dividend term is known at time $t$ and belongs to the payoff defined from time zero; it cannot be discarded when $t>0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
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
