<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The autoregressive polynomial factors as $(1-0.4z)(1+0.7z)$, with zeros

$$
\boxed{z=2.5,\qquad z=-10/7.}
$$

Both have modulus greater than one. The [causality root criterion for an autoregressive model](../../../../../../causality-root-criterion-for-an-autoregressive-model.md) therefore gives a causal stationary solution. The moving-average polynomial has its only zero at $-2$, also outside the unit circle, so the [invertibility of a moving-average model](../../../../../../invertibility-of-a-moving-average-model.md) holds. There is no common root to cancel.

To use unit-[variance](../../../../../../variance-split.md) [white noise](../../../../../../white-noise.md), put $W_t=Z_t/2$. One suitable pair is

$$
\boxed{\widetilde\phi(z)=1+0.30z-0.28z^2,\qquad\widetilde\theta(z)=2+z.}
$$

Then $\widetilde\phi(B)X_t=\widetilde\theta(B)W_t$ with $W\sim\operatorname{WN}(0,1)$. The factor two changes the innovation scale, not the zero of the moving-average polynomial.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
