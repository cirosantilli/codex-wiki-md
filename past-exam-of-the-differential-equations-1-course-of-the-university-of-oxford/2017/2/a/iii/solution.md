<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under $Mh\leq k$, the same [Picard iteration](../../../../../picard-iteration.md) operator maps all of $C_h$ into itself. It need not be a [contraction mapping](../../../../../contraction-mapping.md) in one step, since $Lh$ can exceed one. Instead repeated integration gives the [factorial estimate for Picard iteration](../../../../../factorial-estimate-for-picard-iteration.md)

$$
|(T^ny)(x)-(T^nz)(x)|\leq\frac{L^n|x-a|^n}{n!}\|y-z\|_\infty,
$$

proved inductively by integrating the preceding bound between $a$ and $x$. Thus

$$
\|T^ny-T^nz\|_\infty\leq\frac{(Lh)^n}{n!}\|y-z\|_\infty.
$$

For some $n$ the coefficient is less than one, so $T^n$ is a contraction. Its unique fixed point $y_*$ is also fixed by $T$: $T^n(Ty_*)=T(T^ny_*)=Ty_*$ and uniqueness forces $Ty_*=y_*$. Conversely any fixed point of $T$ is one of $T^n$. This [iterated contraction](../../../../../iterated-contraction.md) argument gives **a unique solution on the full interval $[a-h,a+h]$**, without the unjustified extra assumption $Lh<1$.

The uniqueness statement is for solutions in the specified rectangle, where $f$ is given and controlled. The bound $Mh\leq k$ keeps the constructed solution inside that rectangle throughout the interval.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
