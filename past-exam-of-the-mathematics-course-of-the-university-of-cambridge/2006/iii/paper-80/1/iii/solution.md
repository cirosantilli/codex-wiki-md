<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In one dimension the [periodic conductivity cell problem](../../../../../../periodic-conductivity-cell-problem.md) reduces to

$$
\frac{d}{dy}\left[a(y)(1+w'(y))\right]=0.
$$

Hence $a(y)(1+w')=C$ is constant. Periodicity requires $\int_0^1w'\,dy=0$, so

$$
1=C\int_0^1\frac{dy}{a(y)}
=C\left(\frac{p_1}{a_1}+\frac{p_2}{a_2}\right).
$$

The effective flux average is $a^*=\int_0^1a(1+w')\,dy=C$, giving

$$
\boxed{a^*=\left(\frac{p_1}{a_1}+\frac{p_2}{a_2}\right)^{-1}
=\frac{a_1a_2}{p_1a_2+p_2a_1}.}
$$

One can exhibit the corrector explicitly: $w'=a^*/a_1-1$ in phase 1 and $w'=a^*/a_2-1$ in phase 2. Its integrated change over a period is zero, so a continuous piecewise affine periodic $w$ exists, and an additive constant fixes its mean.

This is precisely the normal component of the [laminate conductivity](../../../../../../laminate-conductivity.md) in part (i). In one dimension there is no tangential direction: every heat-flow path crosses the phases in sequence, so only the harmonic-mean response remains.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
