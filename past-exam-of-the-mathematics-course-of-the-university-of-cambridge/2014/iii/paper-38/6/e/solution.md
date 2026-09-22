<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

[Concavity](../../../../../../concave-function.md) gives the supporting-tangent inequality

$$
U(\hat c_t)-U(c_t)\leq U'(c_t)(\hat c_t-c_t).
$$

Multiply by the [discount factor](../../../../../../discount-factor.md) $e^{-bt}$ and use the first-order condition $e^{-bt}U'(c_t)=Y_t$. This gives the pointwise [marginal-utility verification of optimal consumption](../../../../../../marginal-utility-verification-of-optimal-consumption.md) inequality

$$
e^{-bt}[U(\hat c_t)-U(c_t)]\leq Y_t(\hat c_t-c_t).
$$

Apply the budget inequality from part (d) to the competing admissible strategy, and use equality for the proposed one:

$$
\mathbb E\int_0^\infty Y_t\hat c_tdt\leq Y_0X_0
=\mathbb E\int_0^\infty Y_tc_tdt.
$$

The two weighted [consumption](../../../../../../consumption.md) integrals are finite, so their difference is [integrable](../../../../../../integrability.md). Under the usual positive discount-rate assumption $b>0$, the utility integrals are also [integrable](../../../../../../integrability.md): $U(0)\leq U(x)\leq L$ for a finite upper bound $L$, and $\int_0^\infty e^{-bt}dt=1/b$. Integrating the tangent inequality and taking [expectations](../../../../../../expected-value.md) therefore gives

$$
\boxed{\mathbb E\int_0^\infty e^{-bt}U(c_t)dt
\geq\mathbb E\int_0^\infty e^{-bt}U(\hat c_t)dt.}
$$

Economically, both consumers face the same state-price budget, and the candidate spends it exactly where its discounted marginal utility equals the state price. This is [utility duality with martingale deflators](../../../../../../utility-duality-with-martingale-deflators.md) in its [consumption](../../../../../../consumption.md) form.

A positive $b$, or another hypothesis making the infinite-horizon objectives well defined and permitting this integration, is needed. The printed question does not specify the sign of $b$. Bounded utility alone does not ensure that an undiscounted infinite time integral exists: a bounded integrand can have both infinite positive and negative parts. Thus the conclusion is established under the standard discount convention $b>0$, and also whenever the displayed objectives satisfy the stated [integrability](../../../../../../integrability.md) conditions; without either convention the literal infinite-horizon comparison need not be a defined mathematical expression.

This can occur within an admissible financial model, not just for an abstract bounded integrand. Take $U(x)=1-2e^{-x}$ and $b=0$. Choose a deterministic smooth nonnegative $c$ with successive unit-length plateaus alternating between zero and the integer $n$, and connect them over intervals whose lengths have finite sum. Then $\int_0^\infty2c_te^{-c_t}dt<\infty$: the high-plateau contributions sum to $\sum_{n\geq1}2ne^{-n}$ and the transition integrand is bounded by $2/e$. Set

$$
Y_t=2e^{-c_t},\qquad B_t=Y_0/Y_t,\qquad
X_t=\frac1{Y_t}\int_t^\infty Y_sc_sds.
$$

The bank account is a positive deterministic [Itô process](../../../../../../ito-process.md) and $Y_tB_t=Y_0$, so $Y$ is a [state-price density](../../../../../../state-price-density.md). Holding $X_t/B_t$ bank units finances consumption with nonnegative wealth and exact budget equality. Also $U'(c_t)=Y_t$. Nevertheless every zero plateau contributes $-1$ to the utility integral, while each sufficiently high plateau contributes a fixed positive amount. Both its negative and positive parts are infinite, so the undiscounted objective is undefined. This establishes why the missing discount or objective-integrability hypothesis is substantive.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
