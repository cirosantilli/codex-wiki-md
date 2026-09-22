<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [isolated singularity](../../../isolated-singularity-split.md) at $a$ means that the function is [holomorphic](../../../holomorphic-function-split.md) throughout some punctured disc $0<|z-a|<r$. Its [residue](../../../residue.md) is the [Laurent coefficient](../../../laurent-coefficient.md) $c_{-1}$, equivalently $(2\pi i)^{-1}\int_{|z-a|=\rho}f(z)\,dz$. The singularity is removable if all negative [Laurent coefficients](../../../laurent-coefficient.md) vanish, a [pole](../../../pole.md) of order $k$ if only finitely many are nonzero and the lowest power is $-k$, and essential if infinitely many negative [coefficients](../../../coefficient.md) are nonzero.

For the final [contour integral](../../../contour-integral.md), expand $e^{tz}e^{t/z}$. On the [circle](../../../circle.md) these exponential series converge absolutely and uniformly for $t$ in every bounded set, so their product can be integrated term by term. In

$$
\sum_{j,k\ge0}\frac{t^{j+k}}{j!k!}z^{j-k-2},
$$

only $j-k-2=-1$ contributes. Set $k=m$, $j=m+1$. Thus

$$
\boxed{b_m=\frac{2\pi i}{m!(m+1)!},\qquad m\ge0.}
$$

The resulting power series converges for every complex $t$ by the ratio test. The [coefficients](../../../coefficient.md) are independent of the positive radius $R$.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2008](../../2008-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
