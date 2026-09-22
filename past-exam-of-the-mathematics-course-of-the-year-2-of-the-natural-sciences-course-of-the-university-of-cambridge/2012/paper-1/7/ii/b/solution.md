<h1 id="7/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Iterate the [Gamma function recurrence](../../../../../../gamma-function-recurrence.md) to obtain, near $z=-m$ for $m\geq0$,

$$
\Gamma(z)=\frac{\Gamma(z+m+1)}{z(z+1)\cdots(z+m)}.
$$

The numerator is holomorphic and equals $\Gamma(1)=1$ at $z=-m$. Exactly one denominator factor, $z+m$, vanishes; the product of the remaining factors there is $(-m)(-m+1)\cdots(-1)=(-1)^m m!$. Thus there is a [simple pole](../../../../../../simple-pole.md), with [Gamma function residue at a nonpositive integer](../../../../../../gamma-function-residue-at-a-nonpositive-integer.md)

$$
\boxed{\operatorname*{Res}_{z=-m}\Gamma(z)=\lim_{z\to-m}(z+m)\Gamma(z)=\frac{(-1)^m}{m!}.}
$$

For $m=0$ the empty product is one. The same recurrence with a sufficiently large shift defines the continuation at every point away from these integers, so no further poles occur. At the poles, the recurrence is an identity of [meromorphic functions](../../../../../../meromorphic-function.md), rather than an equality of finite values.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [7](../../../7.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
