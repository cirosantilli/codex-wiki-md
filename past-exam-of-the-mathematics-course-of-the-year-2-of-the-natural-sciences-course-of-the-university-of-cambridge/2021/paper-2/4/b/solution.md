<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $s=1/n$, so $0<s<1$. For the [complex exponentiation](../../../../../complex-exponentiation.md) $z^s$, choose $-\pi/2<\arg z<3\pi/2$: the [branch cut](../../../../../branch-cut.md) is the negative imaginary axis. Integrate $z^s/(a^2+z^2)$ around the upper half-plane semicircle, with a small semicircular indentation excluding the origin. The only enclosed [simple pole](../../../../../simple-pole.md) is $z=ia$, with [residue](../../../../../residue.md)

$$
\operatorname{Res}_{z=ia}\frac{z^s}{a^2+z^2}=\frac{(ia)^s}{2ia}.
$$

The large arc is $O(R^{s-1})$ and the small arc is $O(\epsilon^{s+1})$, so both vanish. On the negative real segment, $z^s=e^{i\pi s}|z|^s$; accounting for the direction of traversal, the two real segments therefore sum to $(1+e^{i\pi s})I$, where $I$ is the desired positive-axis integral. The [residue theorem](../../../../../residue-theorem.md) gives

$$
(1+e^{i\pi s})I=\pi a^{s-1}e^{i\pi s/2}.
$$

Since $1+e^{i\pi s}=2e^{i\pi s/2}\cos(\pi s/2)$,

$$
\boxed{I=\frac{\pi a^{1/n-1}}{2\cos[\pi/(2n)]}.}
$$

The endpoint estimates also prove convergence. More generally the same calculation is the [fractional-power integral from an upper-half-plane contour](../../../../../fractional-power-integral-from-an-upper-half-plane-contour.md), valid for $-1<s<1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
