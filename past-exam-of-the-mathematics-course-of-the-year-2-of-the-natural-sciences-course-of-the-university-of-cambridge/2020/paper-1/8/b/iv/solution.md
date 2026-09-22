<h1 id="8/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Split the inverse transform into the intervals $|\omega|<\mu$ and $|\omega|>\mu$, and in each case pair the positive-frequency [integral](../../../../../../integral-split.md) with its [complex conjugate](../../../../../../complex-conjugate.md) at negative [frequency](../../../../../../frequency.md). The low-frequency pair becomes

$$
\frac1\pi\operatorname{Re}\int_0^\mu A(\omega)e^{ik(\omega)r}e^{i\omega t}\,d\omega,
$$

since $B=0$ and the decaying spatial factor is real. In the high-frequency positive half, replace $A(\omega)$ by $B(-\omega)^*$. The negative half is again its conjugate. Combining the two pieces gives

$$
\boxed{\sigma(t,r)=\frac1\pi\operatorname{Re}\left[
\int_0^\mu A(\omega)e^{ikr}e^{i\omega t}\,d\omega+
\int_\mu^\infty\left\{B(\omega)e^{-ikr}e^{i\omega t}
+B(-\omega)^*e^{ikr}e^{i\omega t}\right\}d\omega\right],\quad\lambda=\frac1\pi.}
$$

Every integrand satisfies the massive [wave equation](../../../../../../wave-equation-split.md) because $\omega^2=k^2+\mu^2$. Linearity, and taking the real part, preserve the equation whenever differentiation under the [integrals](../../../../../../integral-split.md) is justified, or distributionally under the corresponding spectral assumptions. The construction is exactly the [real bounded Fourier modes of the Klein-Gordon equation](../../../../../../real-bounded-fourier-modes-of-the-klein-gordon-equation.md) decomposition.

The displayed expression uses ordinary spectral amplitudes. If distributions supported at $\omega=\pm\mu$ are admitted, a further bounded threshold contribution $c_1\cos\mu t+c_2\sin\mu t$, independent of $r$, is possible. It is not a missing propagating or evanescent branch of the open [frequency](../../../../../../frequency.md) intervals.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
