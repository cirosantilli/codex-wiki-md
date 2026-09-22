<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If the discounted [zero-coupon bond](../../../../../../zero-coupon-bond.md) price is a [martingale](../../../../../../martingale-split.md), its [expectation](../../../../../../expected-value.md) is $Z_{0,T}=e^{-A(0,T)}$. The [Gaussian moment-generating function](../../../../../../moment-generating-function-of-a-normal-distribution.md) applied to the representation above gives $\mathbb E Z_{s,T}=e^{-A(s,T)+v(s,T)/2}$, so

$$
A(s,T)-A(0,T)=\frac12v(s,T).
$$

Differentiate in maturity $T\geq s$. The two mean derivatives are $\mu_{s,T}$ and $\mu_{0,T}$. Symmetry of the [covariance](../../../../../../covariance.md) in its last two arguments makes the two boundary terms in the derivative of the double integral equal. Hence

$$
\frac12\partial_Tv(s,T)=\int_0^T c(s\wedge u,u,T)\,du.
$$

We obtain the [Gaussian forward-rate covariance drift restriction](../../../../../../gaussian-forward-rate-covariance-drift-restriction.md)

$$
\boxed{\mu_{s,T}=\mu_{0,T}+\int_0^T c(s\wedge u,u,T)\,du,}
$$

which proves that the [martingale](../../../../../../martingale-split.md) condition implies the mean restriction. Only maturity differentiation is used; a time derivative of the [covariance](../../../../../../covariance.md) is unnecessary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
