<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Initially suppose $0<\alpha<\pi/2$, the usual oscillatory range. The [oscillatory phase](../../../../../../../oscillatory-integral-phase.md) is $n\Phi(\vartheta)$ with $\Phi=\sec\alpha\sin\vartheta-\vartheta$. Its [stationary point](../../../../../../../stationary-point.md) is $\vartheta=\alpha$, since $\sec\alpha\cos\vartheta=1$. At that point

$$
\Phi(\alpha)=\tan\alpha-\alpha,\qquad \Phi''(\alpha)=-\tan\alpha.
$$

The [stationary phase method](../../../../../../../stationary-phase-method.md) therefore gives the [Debye Bessel asymptotic](../../../../../../../debye-asymptotic-for-oscillatory-bessel-functions.md)

$$
\boxed{J_n(n\sec\alpha)=\sqrt{\frac{2}{\pi n\tan\alpha}}
\cos\left[n(\tan\alpha-\alpha)-\frac\pi4\right]+O(n^{-3/2})}.
$$

The error is additive for fixed positive $\alpha$ bounded away from $\pi/2$; this formula is not uniform as $\alpha\to0$, when the [stationary point](../../../../../../../stationary-point.md) joins the endpoint and its curvature vanishes.

The printed condition $\alpha>0$ alone includes other trigonometric branches. All defined fixed real cases can be covered as follows. If $0<|\cos\alpha|<1$, put $\beta=\arccos|\cos\alpha|\in(0,\pi/2)$. Use the displayed formula with $\beta$ instead of $\alpha$, and multiply it by $1$ if $\sec\alpha>0$, or by $(-1)^n$ if $\sec\alpha<0$. This follows from the integer-order parity $J_n(-x)=(-1)^nJ_n(x)$, which is also obtained from the defining integral by $\vartheta\mapsto\pi-\vartheta$. If $|\cos\alpha|=1$, the argument is $\pm n$ and the turning-point answer below applies, with the same parity factor. If $\cos\alpha=0$, the stated argument is undefined.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
