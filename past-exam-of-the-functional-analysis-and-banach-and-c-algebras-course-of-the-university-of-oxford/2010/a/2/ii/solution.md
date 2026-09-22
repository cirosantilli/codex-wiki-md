<h1 id="a/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under [duality of sequence spaces](../../../../../duality-of-sequence-spaces.md), $a=(a_n)\in\ell_1$ represents $f_a(x)=\sum a_nx_n$ on $c_0$, with [operator norm](../../../../../operator-norm.md) $\|f_a\|=\sum|a_n|$. Here $c_0$ is the [space of sequences converging to zero](../../../../../space-of-sequences-converging-to-zero.md), equipped with its supremum [norm](../../../../../norm.md).

If $\|x\|_\infty\leq1$ and $f_a(x)=\sum|a_n|$, then

$$
0=\sum_{n\geq1}(|a_n|-a_nx_n).
$$

Every summand is nonnegative, so $x_n=\operatorname{sgn}(a_n)$ whenever $a_n\ne0$. Infinitely many such coordinates would give infinitely many $|x_n|=1$, contradicting $x_n\to0$. Therefore $a$ has finite support.

Conversely, if $a$ has finite support, choose $x_n=\operatorname{sgn}(a_n)$ on that support and $x_n=0$ elsewhere. Then $x\in c_0$, $\|x\|_\infty\leq1$, and $f_a(x)=\|f_a\|$. The zero functional is included by taking $x=0$. Thus

$$
\boxed{f_a\text{ attains its norm on }B_{c_0}\iff a\in c_{00}.}
$$

This is [norm attainment on the vanishing sequence space](../../../../../norm-attainment-on-the-vanishing-sequence-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
