<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $B=\beta$ for the driving [Brownian motion](../../../../../../brownian-motion-split.md) throughout; the two symbols in the displayed formulas refer to the same process. For $t<1$ the deterministic integrand is square-integrable on $[0,t]$, so

$$
I_t=\int_0^t\frac{dB_s}{1-s},\qquad X_t=(1-t)I_t
$$

is well defined. The [Itô product rule](../../../../../../ito-product-rule.md), with zero [quadratic covariation](../../../../../../quadratic-covariation.md) against the deterministic factor, gives

$$
dX_t=-I_t\,dt+(1-t)\frac{dB_t}{1-t}
=dB_t-\frac{X_t}{1-t}\,dt,\qquad X_0=0.
$$

For the other form, apply the same [Itô product rule](../../../../../../ito-product-rule.md) to $B_t/(1-t)$:

$$
\frac{B_t}{1-t}=\int_0^t\frac{dB_s}{1-s}+\int_0^t\frac{B_s}{(1-s)^2}\,ds.
$$

Multiplying by $1-t$ gives the [stochastic integral representation of a Brownian bridge](../../../../../../stochastic-integral-representation-of-a-brownian-bridge.md)

$$
\boxed{X_t=B_t-(1-t)\int_0^t\frac{B_s}{(1-s)^2}\,ds},\qquad t<1.
$$

The drift coefficient is singular only at the terminal endpoint, so this calculation is performed on compact subintervals of $[0,1)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
