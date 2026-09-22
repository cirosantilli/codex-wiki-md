<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the struck interval lies within the string, so $0\leq\ell-a/2<\ell+a/2\leq L$. The initially stationary straight string has $A_n=0$. Write its initial velocity as a [Fourier sine series](../../../../../fourier-sine-series.md) $g(x)=\sum_ng_n\sin(k_nx)$. Then

$$
g_n=\frac{2v}{L}\int_{\ell-a/2}^{\ell+a/2}\sin\frac{n\pi x}{L}\,dx=\frac{4v}{n\pi}\sin\frac{n\pi\ell}{L}\sin\frac{n\pi a}{2L}.
$$

Thus $y(x,t)=\sum_n(g_n/\omega_n)\sin(\omega_nt)\sin(k_nx)$. Immediately after the strike all the [energy](../../../../../energy-split.md) is [kinetic energy](../../../../../kinetic-energy.md):

$$
E=\frac\rho2\int_0^L g(x)^2\,dx=\frac{\rho av^2}{2}.
$$

The [orthogonality](../../../../../orthogonal-vectors.md) [integral](../../../../../integral-split.md) $\int_0^L\sin(k_nx)\sin(k_mx)\,dx=(L/2)\delta_{nm}$ assigns [energy](../../../../../energy-split.md) $E_n=\rho Lg_n^2/4$ to mode $n$. Since the ideal modes evolve independently, their total kinetic-plus-elastic energies remain constant. Therefore the [modal energy of a localized velocity impulse on a string](../../../../../modal-energy-of-a-localized-velocity-impulse-on-a-string.md) gives

$$
\boxed{\frac{E_n}{E}=\frac{8L}{a\pi^2n^2}\sin^2\frac{n\pi\ell}{L}\sin^2\frac{n\pi a}{2L}.}
$$

The centre factor selects modes having significant motion at the impact location; the width factor accounts for cancellation across the finite hammer footprint. [Parseval's identity](../../../../../parseval-identity.md) ensures $\sum_{n\geq1}E_n/E=1$. The velocity discontinuities are understood in the mean-square sense and do not alter the [energy](../../../../../energy-split.md) [integrals](../../../../../integral-split.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
