<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work under the money-market [risk-neutral measure](../../../../../risk-neutral-measure.md), with $r_0\geq0$. The [zero-coupon bond](../../../../../zero-coupon-bond.md) price is $P(0,T)=\mathbb E[\exp(-\int_0^T r_sds)]$. For this [CIR model](../../../../../cox-ingersoll-ross-model.md), write $p(\tau,r)=A(\tau)e^{-B(\tau)r}$. The [Feynman-Kac formula](../../../../../feynman-kac-formula.md) gives

$$
\partial_\tau p=(a-br)\partial_rp+\tfrac12\sigma^2r\partial_{rr}p-rp,\qquad p(0,r)=1.
$$

Matching the constant and linear coefficients of $r$ yields

$$
B'=1-bB-\tfrac12\sigma^2B^2,\qquad A'/A=-aB,\qquad B(0)=0,\quad A(0)=1.
$$

For [CIR bond pricing](../../../../../cir-bond-pricing.md), solving this [Riccati equation](../../../../../riccati-equation.md) and integrating the scalar equation for $A$, put $\gamma=\sqrt{b^2+2\sigma^2}$ and $D(\tau)=(\gamma+b)(e^{\gamma\tau}-1)+2\gamma$. Then

$$
B(\tau)=\frac{2(e^{\gamma\tau}-1)}{D(\tau)},\qquad A(\tau)=\left[\frac{2\gamma e^{(b+\gamma)\tau/2}}{D(\tau)}\right]^{2a/\sigma^2}.
$$

Substitution verifies both equations and their initial conditions. The discounted candidate solves the [martingale](../../../../../martingale-split.md) pricing equation; its boundedness on finite horizons, or [Feynman-Kac formula](../../../../../feynman-kac-formula.md), identifies it with the [conditional expectation](../../../../../conditional-expectation.md). **The answer is $\boxed{P(0,T)=A(T)e^{-B(T)r_0}}$.** More generally the same coefficients give $P(t,T)=A(T-t)e^{-B(T-t)r_t}$.

The [CIR model](../../../../../cox-ingersoll-ross-model.md) mean reverts to $a/b$ and has volatility $\sigma\sqrt r$, so it remains nonnegative and its fluctuation size depends on the rate level. For positive initial rate, zero is inaccessible if $2a\geq\sigma^2$; below this threshold zero is reachable but the process remains nonnegative. Its stationary law is a [gamma distribution](../../../../../gamma-distribution.md), of shape $2a/\sigma^2$ and rate $2b/\sigma^2$. Explicit affine bond prices and nonnegative rates are useful features. Limitations include exclusion of negative rates, restricted volatility behavior and a single stochastic factor; the time-homogeneous parameter family cannot fit an arbitrary initial term structure exactly.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
