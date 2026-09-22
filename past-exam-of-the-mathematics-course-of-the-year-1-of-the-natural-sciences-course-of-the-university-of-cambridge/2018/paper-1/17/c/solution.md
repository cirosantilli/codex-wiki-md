<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate $x/(1+x^2)^n$ and integrate between zero and infinity. Its boundary values vanish for every integer $n\ge1$, giving

$$
0=\int_0^\infty\left[\frac1{(1+x^2)^n}-\frac{2nx^2}{(1+x^2)^{n+1}}\right]dx.
$$

Since $x^2/(1+x^2)^{n+1}=(1+x^2)^{-n}-(1+x^2)^{-n-1}$, this becomes $0=E_n-2n(E_n-E_{n+1})$. Hence the [recurrence relation](../../../../../recurrence-relation.md) is

$$
\boxed{E_{n+1}=\frac{2n-1}{2n}E_n.}
$$

The starting value is $E_1=[\arctan x]_0^\infty=\pi/2$. Therefore $E_2=\pi/4$, $E_3=3\pi/16$, and

$$
\boxed{\int_0^\infty\frac{dx}{(1+x^2)^4}=E_4=\frac56\frac34\frac12\frac\pi2=\frac{5\pi}{32}.}
$$

These are also [Wallis integrals](../../../../../wallis-integrals.md) after the [integration by substitution](../../../../../integration-by-substitution.md) $x=\tan t$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
