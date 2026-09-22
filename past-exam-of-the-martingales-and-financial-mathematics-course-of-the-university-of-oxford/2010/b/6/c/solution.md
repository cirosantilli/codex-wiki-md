<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The conditional mean solves $m'(v)=rm(v)+\delta$ with $m(t)=S_t$. Hence, for $r\ne0$,

$$
\boxed{\mathbb E[\widehat S_T\mid\widehat S_t=S_t]
=S_te^{r\tau}+\frac\delta r(e^{r\tau}-1).}
$$

The forward contract's terminal payoff is $S_T-K$, so discounting this expectation gives its current value

$$
\boxed{F(t,S_t)=S_t+\frac\delta r(1-e^{-r\tau})-Ke^{-r\tau}.}
$$

For $r=0$, the continuous limits are $S_t+\delta\tau$ for the mean and $S_t+\delta\tau-K$ for the contract value. A fair delivery price, as distinct from the current contract value, is the strike making this value zero: $K_*=S_te^{r\tau}+\delta(e^{r\tau}-1)/r$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
