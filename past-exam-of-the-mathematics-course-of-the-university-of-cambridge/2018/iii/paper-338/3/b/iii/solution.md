<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Increasing exposure reduces fractional [photon shot noise](../../../../../../../photon-shot-noise.md) as $T^{-1/2}$, but a fixed background mismatch grows in proportion to the signal. The fractional systematic error is $|1-f|R_B/R_Q$, independent of exposure. The [systematic-error signal-to-noise ceiling](../../../../../../../systematic-error-signal-to-noise-ceiling.md) can therefore be poor for a faint source in a bright sky even when random fluctuations are tiny.

Better [background subtraction](../../../../../../../background-subtraction.md) requires matching sky location and time, correcting detector response, dithering or modelling spatial background variations. If $f$ were known exactly, one could instead use $X-Y/f$, which is unbiased and has variance $Q+B+B/f$. The ceiling arises from an uncorrected or unknown mismatch in the prescribed subtraction, not an unavoidable property of measuring two patches.

To reach an accuracy ratio $Z_*$ at all, a necessary condition in the fixed-mismatch model is

$$
\boxed{|1-f|<\frac{R_Q}{Z_*R_B}.}
$$

Equality allows only an asymptotic approach; finite exposure adds positive random error. **More exposure improves precision, but only better calibration removes the fixed background bias.**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
