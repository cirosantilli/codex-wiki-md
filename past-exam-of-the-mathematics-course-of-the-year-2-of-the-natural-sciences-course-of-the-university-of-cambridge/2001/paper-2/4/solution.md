<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Poles and residues.** An isolated singularity $z_0$ is a [pole](../../../../pole.md) of order $m$ if its [Laurent series](../../../../laurent-series.md) has finitely many negative powers, the lowest being a nonzero multiple of $(z-z_0)^{-m}$. The [residue](../../../../residue.md) is the coefficient of $(z-z_0)^{-1}$.

If $h(z_0)=0$ and $h'(z_0)\ne0$, factor $h(z)=(z-z_0)H(z)$, where $H$ is [holomorphic](../../../../holomorphic-function-split.md) near $z_0$ and $H(z_0)=h'(z_0)$. For $g(z_0)\ne0$,

$$
\frac{g(z)}{h(z)}=\frac1{z-z_0}\frac{g(z)}{H(z)}.
$$

The last quotient is [holomorphic](../../../../holomorphic-function-split.md) and nonzero at $z_0$, proving a [simple pole](../../../../simple-pole.md) with

$$
\boxed{\operatorname{Res}_{z_0}\frac gh=\frac{g(z_0)}{h'(z_0)}.}
$$

**The given function.** For noninteger $a$, specify a [branch of a multivalued function](../../../../branch-of-a-multivalued-function.md) before using $z^a$. Choose $z^a=\exp(a\log z)$ with $-\pi/2<\arg z<3\pi/2$, a cut along the negative imaginary axis. This leaves all three roots of $1+z^3$ off the cut. They are $z_+=e^{i\pi/3}$, $z_- =e^{-i\pi/3}$ and $z_0=-1$, all simple. The numerator is nonzero at these points. Since the denominator has [derivative](../../../../derivative.md) $3z^2$, the [residues](../../../../residue.md) are

$$
\boxed{\begin{array}{c|c}
\text{pole}&\text{residue}\\\hline
e^{i\pi/3}&\tfrac13e^{i\pi(a-2)/3}\\
e^{-i\pi/3}&\tfrac13e^{-i\pi(a-2)/3}\\
-1&\tfrac13e^{i\pi(a-2)}
\end{array}.}
$$

For noninteger $a$, zero is a [branch point](../../../../branch-point.md), rather than an isolated [pole](../../../../pole.md). This remains true when $-1<a<0$ and the numerator diverges there. For nonnegative integer $a$ it is a regular point. Other logarithm branches change the phases of the [residues](../../../../residue.md) consistently.

**Integral and convergence.** Near zero the integrand behaves as $x^a$, requiring $a>-1$. At infinity it behaves as $x^{a-3}$, requiring $a<2$. Therefore the exact convergence range is

$$
\boxed{-1<a<2.}
$$

Use a counterclockwise sector contour with rays at angles $0$ and $2\pi/3$, inner radius $\varepsilon$ and outer radius $R$. The same [complex logarithm](../../../../complex-logarithm.md) branch is valid throughout this sector. Only $z_+=e^{i\pi/3}$ lies inside. The small circular arc contributes $O(\varepsilon^{a+1})$ and the large one contributes $O(R^{a-2})$, so both vanish precisely in the stated range.

The outward positive-real ray contributes $I$. On the returning ray set $z=xe^{2\pi i/3}$: the denominator is still $1+x^3$, while $z^a dz=e^{2\pi i(a+1)/3}x^a dx$, with reversed limits. The [residue theorem](../../../../residue-theorem.md) gives

$$
(1-e^{2\pi i(a+1)/3})I=\frac{2\pi i}{3}e^{i\pi(a-2)/3}.
$$

Put $\alpha=\pi(a+1)/3$. The right-hand phase is $-e^{i\alpha}$ and $1-e^{2i\alpha}=-2ie^{i\alpha}\sin\alpha$. Hence

$$
\boxed{\int_0^\infty\frac{x^a}{1+x^3}\,dx=\frac{\pi}{3\sin(\pi(a+1)/3)},\qquad-1<a<2.}
$$

The sine is positive in this range, consistent with a positive real [integral](../../../../integral-split.md). This is a special case of the [Mellin integral of a reciprocal binomial](../../../../mellin-integral-of-a-reciprocal-binomial.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
