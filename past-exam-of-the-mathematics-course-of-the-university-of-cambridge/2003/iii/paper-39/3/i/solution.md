<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the [classical risk model](../../../../../../classical-risk-model.md), the surplus with initial capital $u\geq0$ is

$$
U(t)=u+ct-\sum_{j=1}^{N(t)}X_j,\qquad c=(1+\rho)\lambda\mu,
$$

where $N(t)$ is a [Poisson process](../../../../../../poisson-process.md) of rate $\lambda$, and the nonnegative independent [claim sizes](../../../../../../claim-size.md), of mean $\mu>0$, are independent of that process. Positive [relative safety loading](../../../../../../relative-safety-loading.md) $\rho$ makes expected premium income exceed expected claim outflow. With ruin time $T=\inf\{t\geq0:U(t)<0\}$, the [ultimate ruin probability](../../../../../../ultimate-ruin-probability.md) is

$$
\boxed{\psi(u)=\mathbb P(T<\infty\mid U(0)=u).}
$$

The [adjustment coefficient](../../../../../../adjustment-coefficient.md) is the positive root $R$ in the finite domain of the claim [moment-generating function](../../../../../../moment-generating-function.md) satisfying

$$
\boxed{\lambda(M_X(R)-1)=cR,\quad\text{or }M_X(R)=1+(1+\rho)\mu R.}
$$

The zero root is excluded by definition.

Under the stated transform-divergence assumption this positive root exists and is unique. Indeed $F(r)=M_X(r)-1-(1+\rho)\mu r$ has $F(0)=0$, derivative $F'(0)=-\rho\mu<0$, and strictly positive second derivative on its positive domain. At a finite endpoint the diverging transform makes $F$ positive eventually. At an infinite endpoint, choose $a>0$ with $\mathbb P(X\geq a)>0$; the bound $M_X(r)\geq\mathbb P(X\geq a)e^{ar}$ makes it dominate the linear term. Strict convexity then gives exactly one positive crossing. This is the [secant-slope existence criterion for an adjustment coefficient](../../../../../../secant-slope-existence-criterion-for-an-adjustment-coefficient.md).

The [Lundberg inequality](../../../../../../lundberg-inequality.md) is

$$
\boxed{\psi(u)\leq e^{-Ru}\qquad(u\geq0).}
$$

For a short justification, the compound-Poisson transform and the defining equation make $e^{-RU(t)}$ a nonnegative [martingale](../../../../../../martingale-split.md) starting at $e^{-Ru}$. Stop it at $T\wedge t$, a bounded [stopping time](../../../../../../stopping-time.md). On $\{T\leq t\}$ its value is greater than one. The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) therefore gives $\mathbb P(T\leq t)\leq e^{-Ru}$; let $t$ increase to infinity. No expectation identity at an unbounded ruin time is required.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
