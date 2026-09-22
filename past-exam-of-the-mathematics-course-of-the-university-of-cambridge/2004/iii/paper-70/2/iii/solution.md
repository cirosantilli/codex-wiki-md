<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Scale the equal intervals to unit length. A nonzero compactly supported cubic [B-spline](../../../../../../b-spline.md) with maximum continuity is $C^2$, so its fourth [derivative](../../../../../../derivative.md) is a sum of impulses at the knots. Equivalently it is a combination of truncated cubes,

$$
N(x)=\sum_{j=0}^{m}a_j(x-j)_+^3.
$$

To vanish to the right of its support, the polynomial tail must be identically zero. Expanding that tail requires $\sum_ja_jj^r=0$ for $r=0,1,2,3$. Four or fewer distinct knots give a full-rank [Vandermonde matrix](../../../../../../vandermonde-matrix.md) and only the zero solution. Hence a nonzero function requires at least five knots, or four intervals. At knots $0,1,2,3,4$, the one-dimensional nullspace has coefficients proportional to $(1,-4,6,-4,1)$. The unscaled combination integrates to six on $[0,4]$, so unit-integral cardinal normalization gives:

$$
N(x)=\frac16\left[x_+^3-4(x-1)_+^3+6(x-2)_+^3-4(x-3)_+^3+(x-4)_+^3\right].
$$

This is the [Cardinal cubic B-spline](../../../../../../cardinal-cubic-b-spline.md), nonnegative with support $[0,4]$. To obtain its [cubic B-spline Bézier extraction](../../../../../../cubic-b-spline-bezier-extraction.md), use local parameter $t=x-j\in[0,1]$ on interval $[j,j+1]$. The four power-form numerators, with a common divisor six, are

$$
t^3,\qquad1+3t+3t^2-3t^3,\qquad4-6t^2+3t^3,\qquad(1-t)^3.
$$

For $a+bt+ct^2+dt^3$, the cubic [Bernstein basis](../../../../../../bernstein-basis.md) coefficients are $a$, $a+b/3$, $a+2b/3+c/3$, $a+b+c+d$. Applying this conversion gives

$$
\boxed{\begin{array}{c|cccc}
\text{interval}&b_0&b_1&b_2&b_3\\\hline
[0,1]&0&0&0&1/6\\
[1,2]&1/6&1/3&2/3&2/3\\
[2,3]&2/3&2/3&1/3&1/6\\
[3,4]&1/6&0&0&0
\end{array}}
$$

Each scalar row describes a cubic [Bézier curve](../../../../../../bezier-curve.md) graph piece with abscissa controls $j,j+1/3,j+2/3,j+1$. The truncated-cube construction proves value, first- and second-derivative agreement at all joins, including the zero exterior. Minimum support and maximum continuity determine the basis up to a scalar; the displayed normalization fixes that remaining freedom.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
