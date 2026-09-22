<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $P(T,T)=1$, part (b) shows that the [density process](../../../../../../density-process.md) of the [T-forward measure](../../../../../../t-forward-measure.md) is

$$
L_t^T=\mathbb E^{\mathbb Q}\!\left[\frac{D_T}{P(0,T)}\,\middle|\,\mathcal F_t\right]
=\frac{D_tP(t,T)}{P(0,T)}
=\mathcal E\!\left(-\int_0^\cdot b_s^T\,dW_s\right)_t.
$$

Its terminal [expectation](../../../../../../expected-value.md) is one and it is strictly positive, so the stated [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) defines an [equivalent probability measure](../../../../../../equivalent-probability-measure.md). By the [Girsanov theorem](../../../../../../girsanov-theorem.md),

$$
W_t^T=W_t+\int_0^t b_s^T\,ds
$$

is a [Brownian motion](../../../../../../brownian-motion-split.md) under $\mathbb Q_T$. Substitution of $dW_t=dW_t^T-b_t^Tdt$ cancels the entire [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) drift:

$$
df(t,T)=\sigma(t,T)\,dW_t^T.
$$

Because the integrand is deterministic and bounded, its [Itô integral](../../../../../../ito-integral.md) is square-integrable on $[0,T]$. With the usual fixed initial [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) curve, **the requested true martingale is**

$$
\boxed{f(t,T)=f(0,T)+\int_0^t\sigma(s,T)\,dW_s^T.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
