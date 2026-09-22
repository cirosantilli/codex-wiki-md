<h1 id="9/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $d(\ln\sec x)/dx=\tan x$ and $\ln\sec0=0$. To obtain enough terms of [tangent](../../../../../tangent.md), write $t(x)=x+ax^3+bx^5+O(x^7)$; it is an [odd function](../../../../../odd-function.md). The identity $t'=1+t^2$ gives

$$
1+3ax^2+5bx^4+O(x^6)=1+x^2+2ax^4+O(x^6),
$$

so $a=1/3$, $b=2/15$. Integrate this [Taylor expansion](../../../../../taylor-expansion.md) term by term from zero to $x$:

$$
\boxed{\ln\sec x=\int_0^x\tan t\,dt=\frac{x^2}2+\frac{x^4}{12}+\frac{x^6}{45}+O(x^8).}
$$

There is no constant term, and only even powers occur because $\ln\sec x$ is an [even function](../../../../../even-function.md) near zero. Thus reaching the first three nonzero terms requires expansion through degree six.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
