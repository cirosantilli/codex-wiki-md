<h1 id="7b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiply the [first-order linear differential equation](../../../../../../first-order-linear-differential-equation.md) by the [integrating factor](../../../../../../integrating-factor.md) $e^{t/\alpha}$. Then

$$
\frac d{dt}(e^{t/\alpha}y)=\frac1\alpha e^{t/\alpha}f(t).
$$

If $y\to0$ in the remote past, then $e^{t/\alpha}y\to0$ there. Integration from $-\infty$ gives the necessary formula

$$
\boxed{y(t)=\frac1\alpha\int_{-\infty}^t e^{-(t-s)/\alpha}f(s)\,ds.}
$$

When this integral exists and tends to zero as $t\to-\infty$, differentiating verifies the equation and the past condition. Two such solutions differ by $Ce^{-t/\alpha}$, which diverges at $-\infty$ unless $C=0$, proving uniqueness. This is the [causal response of a first-order relaxation equation](../../../../../../causal-response-of-a-first-order-relaxation-equation.md), a [convolution](../../../../../../convolution.md) with its decaying [impulse response](../../../../../../impulse-response.md).

The phrase “general function” implicitly requires compatibility with the past condition: it does not guarantee existence for arbitrary $f$. A sufficient condition is bounded forcing with $f(t)\to0$ as $t\to-\infty$; after setting $r=t-s$, the integral is bounded by the supremum of $|f|$ before $t$. For example, $f\equiv1$ gives $y=1+Ce^{-t/\alpha}$, so no solution has the stated past limit. Both forcings below vanish in the past and meet the intended causal condition, the impulse being interpreted distributionally.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7B](../../7b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
