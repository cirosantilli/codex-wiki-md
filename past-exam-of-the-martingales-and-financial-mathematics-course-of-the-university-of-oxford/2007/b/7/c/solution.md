<h1 id="b/7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
c(u)=\Phi\left(\frac{r+\sigma^2/2}{\sigma}\sqrt u\right)
-e^{-ru}\Phi\left(\frac{r-\sigma^2/2}{\sigma}\sqrt u\right),
\qquad c(0)=0.
$$

The [homogeneous function](../../../../../homogeneous-function.md) of the [Black-Scholes formula](../../../../../black-scholes-formula.md) gives its at-the-money value at the start date as $S_{T_1}c(T-T_1)$. Before that date, [risk-neutral valuation](../../../../../risk-neutral-pricing.md) and the discounted stock [martingale](../../../../../martingale-split.md) give

$$
e^{-r(T_1-t)}\mathbb E[S_{T_1}c(T-T_1)\mid\mathcal F_t]
=S_t c(T-T_1).
$$

After the start date the [strike price](../../../../../strike-price.md) is the realized value $S_{T_1}$, so the complete answer is

$$
\boxed{V_t=
\begin{cases}
S_t c(T-T_1),&0\leq t<T_1,\\
C(t,S_t;T,S_{T_1}),&T_1\leq t\leq T.
\end{cases}}
$$

At maturity the second line is $(S_T-S_{T_1})_+$. After entry the price depends on the historical [strike price](../../../../../strike-price.md) as well as the current stock, so that history cannot be discarded when giving the answer for all times.

## ↑ Ancestors (13)

1. [C](../c.md)
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
