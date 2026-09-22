<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The call spread in the hint has payoff

$$
H_\epsilon(s)=\frac{(s-K)^+-(s-K-\epsilon)^+}{\epsilon}.
$$

It is between zero and one and converges to $1_{\{s>K\}}$ as $\epsilon\downarrow0$. In the [Black-Scholes model](../../../../../black-scholes-model.md) with positive volatility and $t<T$, the conditional terminal stock distribution has no atom at $K$. The strict and non-strict indicator therefore have the same discounted expectation. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) in the risk-neutral pricing formula gives

$$
V_{\rm digital}
=\lim_{\epsilon\downarrow0}
\frac{C(t,S_t;K)-C(t,S_t;K+\epsilon)}{\epsilon}
=\boxed{-C_K(t,S_t;K).}
$$

Equivalently this is $e^{-r(T-t)}\Phi(d_2)$. The no-atom condition explains the endpoint subtlety: the displayed spread has value zero at $s=K$, whereas the printed digital pays one there. At maturity the strike derivative can be one-sided or undefined, so the smooth pricing identity is understood before expiry.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
