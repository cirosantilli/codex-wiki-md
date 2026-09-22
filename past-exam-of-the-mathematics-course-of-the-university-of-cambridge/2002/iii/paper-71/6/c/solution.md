<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $k\gg aH$, the dominant term is

$$
w_k\simeq\frac{e^{ik/(aH)}}{L^{3/2}a\sqrt{2k}}=\frac{e^{-ik\eta}}{\sqrt{2L^3a^3\omega_{\rm phys}}},\qquad\eta=-\frac1{aH},\quad\omega_{\rm phys}=\frac ka.
$$

This is the positive-frequency harmonic-oscillator normalization with the physical box volume $a^3L^3$. Over a period much shorter than $H^{-1}$, the [scale factor](../../../../../../scale-factor-cosmology.md) and physical frequency are effectively constant. Equivalently, the rescaled field $aL^{3/2}w_k$ approaches $e^{-ik\eta}/\sqrt{2k}$ exactly in the short-wavelength limit.

For $k\ll aH$, $w_k\to iL^{-3/2}H/\sqrt{2k^3}$ and $\dot w_k=O(x^2)$, so the growing field mode freezes. A single [Fourier coefficient](../../../../../../fourier-coefficient.md) has [variance](../../../../../../variance-split.md) proportional to $k^{-3}$, which by itself is not scale-independent. The number of modes in a logarithmic shell is proportional to $L^3k^3$. Their product gives

$$
\boxed{\frac{d\langle\delta\phi^2\rangle}{d\log k}=\frac{L^3k^3}{2\pi^2}|w_k|^2\longrightarrow\frac{H^2}{4\pi^2}=\left(\frac H{2\pi}\right)^2}.
$$

Thus equal logarithmic intervals have equal [variance](../../../../../../variance-split.md) in exact de Sitter. Slow evolution of $H$ or nonnegligible effective [mass](../../../../../../mass.md) produces a tilt. Integrating an exactly flat spectrum over arbitrarily many logarithmic intervals still requires infrared and ultraviolet cutoffs; the statement concerns power per interval, not a finite all-scale total [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
