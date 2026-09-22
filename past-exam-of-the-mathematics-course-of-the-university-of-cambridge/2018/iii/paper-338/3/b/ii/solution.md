<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $Q=R_QT$ and $B=R_BT$ in the root-mean-square accuracy measure:

$$
Z(T)=\frac{R_Q\sqrt T}{\sqrt{R_Q+(1+f)R_B+(1-f)^2R_B^2T}}.
$$

For a fixed uncorrected $f\neq1$ and $R_B>0$, the squared bias eventually dominates the shot-noise terms. Therefore

$$
\boxed{\lim_{T\to\infty}Z(T)=\frac{R_Q}{|1-f|R_B}.}
$$

The PDF omits the absolute value. Its expression is the positive accuracy ratio only if $f<1$; for $f>1$ the residual background changes sign, but an error magnitude and a [signal-to-noise ratio in photon counting](../../../../../../../signal-to-noise-ratio-in-photon-counting.md) remain nonnegative. The printed signed formula can instead be read as source divided by signed bias.

For exact background matching $f=1$, there is no [systematic-error signal-to-noise ceiling](../../../../../../../systematic-error-signal-to-noise-ceiling.md): $Z=R_Q\sqrt{T/(R_Q+2R_B)}$ grows without bound in this idealized model. With $R_B=0$ the same conclusion holds. Limits in which $f$ itself approaches one with exposure time are different from the fixed-mismatch limit used here.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
