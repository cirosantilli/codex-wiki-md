<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At fixed [frequency](../../../../../../frequency.md), the transformed equation has characteristic roots $\pm ik$, where

$$
\boxed{k^2=\omega^2-\mu^2.}
$$

For a consistent explicit branch choose

$$
k(\omega)=\begin{cases}
\sqrt{\omega^2-\mu^2},&|\omega|>\mu,\\
i\sqrt{\mu^2-\omega^2},&|\omega|<\mu.
\end{cases}
$$

This branch is even in $\omega$. Away from the two thresholds, the spatial solution is $\widetilde\sigma=A(\omega)e^{ikr}+B(\omega)e^{-ikr}$, so [Fourier inversion](../../../../../../fourier-inversion-theorem.md) gives

$$
\boxed{\sigma(t,r)=\frac1{2\pi}\int_{-\infty}^{\infty}
\left[A(\omega)e^{ik(\omega)r}+B(\omega)e^{-ik(\omega)r}\right]e^{i\omega t}\,d\omega.}
$$

At $|\omega|=\mu$, the spatial equation has a double zero characteristic root and its full solution is $C+D r$. The two exponentials at $k=0$ represent only its constant part. This isolated-frequency issue does not change an [integral](../../../../../../integral-split.md) with ordinary integrable amplitudes; threshold-supported distributional modes require separate treatment.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
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
