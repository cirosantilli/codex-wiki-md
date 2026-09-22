<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the [stationary phase method](../../../../../../../stationary-phase-method.md) to the real part of the exponential integral for the [Bessel function of the first kind](../../../../../../../bessel-function-of-the-first-kind.md). With $n$ fixed, use [oscillatory phase](../../../../../../../oscillatory-integral-phase.md) $\sin\vartheta$ and [oscillatory integral amplitude](../../../../../../../amplitude-of-an-oscillatory-integral.md) $e^{-in\vartheta}$. The unique [stationary point](../../../../../../../stationary-point.md) is $\vartheta_0=\pi/2$, with second [derivative](../../../../../../../derivative.md) $-1$. Its contribution is

$$
\frac1\pi\Re\left[e^{-in\pi/2}e^{ix-i\pi/4}\sqrt{\frac{2\pi}{x}}\right].
$$

The leading endpoint terms of the exponential integral are imaginary and do not contribute to its real part. Hence the [large-argument asymptotic expansion of the Bessel function of the first kind](../../../../../../../large-argument-asymptotic-expansion-of-the-bessel-function-of-the-first-kind.md) is

$$
\boxed{J_n(x)=\sqrt{\frac{2}{\pi x}}\cos\left(x-\frac{n\pi}{2}-\frac\pi4\right)+O(x^{-3/2})}.
$$

This is an additive asymptotic formula: a relative ratio is inappropriate at zeros of the leading cosine. The envelope decreases like $x^{-1/2}$ while the oscillation [frequency](../../../../../../../frequency.md) approaches one.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 74](../../../../paper-74-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
