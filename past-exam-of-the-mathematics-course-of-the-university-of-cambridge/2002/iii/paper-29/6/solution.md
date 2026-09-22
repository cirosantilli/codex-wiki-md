<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use $T$ for the fixed maturity and $s\leq T$ for the observation time. The original PDF's discounting uses the [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) over $[s,T]$ and the [short rate](../../../../../short-rate.md) over $[0,s]$. Let $X(s,u)=F_{s,u}-\mu_{s,u}$ be the centered [Gaussian forward-rate field](../../../../../gaussian-forward-rate-field.md), and define

$$
A(s,T)=\int_0^s\mu_{u,u}\,du+\int_s^T\mu_{s,u}\,du,\qquad
Y(s,T)=\int_0^T X(s\wedge u,u)\,du.
$$

Assume the [covariance](../../../../../covariance.md) and mean have the regularity needed for these [mean-square integrals](../../../../../mean-square-integral.md) and the maturity differentiation below. Splitting $Y$ at $u=s$ shows that the discounted [zero-coupon bond](../../../../../zero-coupon-bond.md) price is

$$
Z_{s,T}=\exp[-A(s,T)-Y(s,T)].
$$

This [integrated Gaussian forward-rate process](../../../../../integrated-gaussian-forward-rate-process.md) has deterministic [variance](../../../../../variance-split.md)

$$
v(s,T)=\int_0^T\int_0^T c(s\wedge u\wedge w,u,w)\,du\,dw.
$$

Its [independent increments](../../../../../independent-increments.md) hold relative to the entire specified [filtration](../../../../../filtration-probability-theory.md). Indeed, if $r\leq s$ and $z\leq r$, the [covariance](../../../../../covariance.md) between $Y(s,T)-Y(r,T)$ and any earlier $X(z,w)$ is the integral of

$$
c((s\wedge u)\wedge z,u,w)-c((r\wedge u)\wedge z,u,w)=0.
$$

Since [uncorrelated jointly Gaussian variables are independent](../../../../../uncorrelated-jointly-normal-variables-are-independent.md), the increment is independent of every finite family of earlier observations and hence of their generated [sigma-algebra](../../../../../sigma-algebra.md). The increment has [normal distribution](../../../../../normal-distribution.md) with mean zero and variance $v(s,T)-v(r,T)$. Also $Y(0,T)=0$ because $c(0,u,w)=0$.

The [Gaussian moment-generating function](../../../../../moment-generating-function-of-a-normal-distribution.md) now gives

$$
\mathbb E[Z_{s,T}\mid\mathcal F_r]
=\exp[-A(s,T)-Y(r,T)+\tfrac12(v(s,T)-v(r,T))].
$$

Therefore the [Gaussian forward-rate covariance drift restriction](../../../../../gaussian-forward-rate-covariance-drift-restriction.md) is exactly the deterministic condition

$$
\boxed{A(s,T)-A(0,T)=\frac12v(s,T).}
$$

It turns $Z_{s,T}/Z_{0,T}$ into a [Gaussian exponential martingale with deterministic variance](../../../../../gaussian-exponential-martingale-with-deterministic-variance.md). The subparts establish the requested equivalent descriptions from this common calculation.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
