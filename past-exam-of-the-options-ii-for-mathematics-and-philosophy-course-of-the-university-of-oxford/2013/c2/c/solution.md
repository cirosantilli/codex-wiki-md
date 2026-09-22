<h1 id="c2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $p=4272943$. Since $p\equiv7\pmod8$, the supplementary laws give $(-1/p)=-1$ and $(2/p)=1$. Therefore $(-286/p)=-(143/p)$.

Both $143$ and $p$ are three modulo four. Reciprocity for the [Jacobi symbol](../../../../jacobi-symbol.md), followed by the supplied remainder, gives

$$
(143/p)=-(p/143)=-(103/143).
$$

Again both denominators are three modulo four, so

$$
(103/143)=-(143/103)=-(40/103).
$$

Now $103\equiv7\pmod8$ and $40=8\cdot5$. Consequently

$$
(40/103)=(2/103)^3(5/103)=(103/5)=(3/5)=-1,
$$

because the nonzero squares modulo five are one and four. Thus $(103/143)=1$, $(143/p)=-1$, and finally

$$
\boxed{(-286/p)=1.}
$$

The congruence **is soluble**, with exactly two distinct solutions modulo this prime: a nonzero root and its negative. The computation uses a prime denominator in its final step; a positive Jacobi symbol with composite denominator would not by itself imply solubility.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [C2](../../c2.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Options II for mathematics and philosophy course of the University of Oxford](../../../../options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
