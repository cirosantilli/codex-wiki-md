<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

For $0<s<1$, differentiation gives

$$
V'(t)=\frac{Q}{1-s}\left(e^{-t/\tau}-s e^{-st/\tau}\right).
$$

Its unique zero solves $e^{-(1-s)t/\tau}=s$. Therefore the [mobile-volume peak of an exponentially forced porous current](../../../../../../mobile-volume-peak-of-an-exponentially-forced-porous-current.md) occurs at

$$
\boxed{t_{\max}=\frac{\tau\log(1/s)}{1-s}.}
$$

The derivative is initially positive and is negative after this time. More explicitly, at the stationary point $V''=-Qs e^{-st/\tau}/\tau<0$. Thus it is the global positive maximum, with

$$
\boxed{V_{\max}=Q\tau s^{s/(1-s)}.}
$$

The claim of a finite maximum requires nonzero [capillary residual trapping](../../../../../../capillary-residual-trapping.md). At $s=0$ the mobile volume rises monotonically towards $Q\tau$ and the peak time tends to infinity. As $s\to1$, the limiting peak time is $\tau$ and the limiting maximum is $Q\tau/e$.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
