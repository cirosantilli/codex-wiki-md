<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Use the one-sided [Laplace transform](../../../../../laplace-transform.md) $F(s)=\int_0^\infty e^{-st}f(t)\,dt$. Since $f=0$ on $[0,1)$, substitution gives $\mathcal L[f(t+1)](s)=e^sF(s)$. Thus

$$
F(s)=\frac1{s(e^s-1/2)}=\frac{2e^{-s}}{s(1-e^{-s}/2)}.
$$

Its [poles](../../../../../pole.md) are $s=0$ and $s_n=-\log2+2\pi in$, with [residues](../../../../../residue.md) of $e^{st}F(s)$ respectively two and $2e^{s_nt}/s_n$. For $t>1$ close the [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) to the left, using horizontal heights avoiding those [poles](../../../../../pole.md). The left-side integrand decays like $e^{st}/s$, and on the right-side horizontal ends like $e^{s(t-1)}/s$, so the added integrals vanish with the usual symmetric limiting contour. The [residue theorem](../../../../../residue-theorem.md) gives

$$
\boxed{f(t)=2+2^{1-t}\sum_{n=-\infty}^{\infty}\frac{e^{2\pi int}}{2\pi in-\log2}\quad(t\geq1),}
$$

where the series is summed symmetrically and at jumps has the midpoint value.

For $t<1$ the vanishing can be checked directly in the inversion integral, rather than inferred from the recurrence. On any vertical line $\Re s=c>0$ expand the denominator geometrically, uniformly there:

$$
F(s)=2\sum_{j=0}^\infty2^{-j}\frac{e^{-(j+1)s}}s.
$$

Each inversion term is $2^{1-j}(2\pi i)^{-1}\int_{c-i\infty}^{c+i\infty}e^{s(t-j-1)}ds/s$. If $t<1$, close this contour to the right: the exponential decays, and the [pole](../../../../../pole.md) at zero is outside, so every term is zero. Equivalently the geometric expansion bounds the full closing contour by the same decaying factors. Thus **$f(t)=0$ for $t<1$**.

The same integral gives $f(t)=2\sum_{j\geq0}2^{-j}H(t-j-1)$ elsewhere. For $m<t<m+1$ with [integer](../../../../../integer.md) $m\geq1$, this is $4(1-2^{-m})$, which directly verifies the difference equation. Neither a [Laplace transform](../../../../../laplace-transform.md) nor a Fourier series determines values at isolated jumps; the printed series fixes the standard convention $H(0)=1/2$, including $f(1)=1$.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
