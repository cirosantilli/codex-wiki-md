<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $M=|f(z_0)|$. The local maximum property gives a [disk](../../../../../disk-mathematics.md) around $z_0$ on which $|f|\leq M$, contained in the [unit disk](../../../../../unit-disk.md). If $M=0$, then $f=0$ on that neighbourhood, and the [identity theorem](../../../../../identity-theorem.md) makes $f$ zero on the connected [unit disk](../../../../../unit-disk.md).

Otherwise multiply $f$ by the unit [complex number](../../../../../complex-number.md) $\overline{f(z_0)}/M$, obtaining a [holomorphic function](../../../../../holomorphic-function-split.md) $g$ with $g(z_0)=M$ and $|g|\leq M$ nearby. Applying the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) on any sufficiently small circle of radius $r$ gives the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md)

$$
M=\frac1{2\pi}\int_0^{2\pi}g(z_0+re^{it})\,dt.
$$

Take real parts. The continuous function $M-\operatorname{Re}g$ is nonnegative on the circle and has [integral](../../../../../integral-split.md) zero, so it vanishes everywhere there. Since $|g|\leq M$, having real part $M$ forces imaginary part zero. Thus $g=M$ throughout the circle. The zeros of $g-M$ have an accumulation point inside its domain, so the [identity theorem](../../../../../identity-theorem.md) gives **$f$ constant on the entire [unit disk](../../../../../unit-disk.md)**. This proves the local [maximum modulus principle](../../../../../maximum-modulus-principle.md) directly from the [Cauchy integral formula](../../../../../cauchy-integral-formula.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
