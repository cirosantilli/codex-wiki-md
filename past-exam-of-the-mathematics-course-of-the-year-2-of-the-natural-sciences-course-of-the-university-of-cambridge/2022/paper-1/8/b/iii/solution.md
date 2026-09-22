<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the normal-form coefficient $p(x)=-1/(1-x)$, [Abel's identity](../../../../../../abel-s-identity.md) gives the [Wronskian](../../../../../../wronskian.md)

$$
\boxed{W(x)=C\exp\left[-\int^xp(s)ds\right]=\frac{C}{1-x}.}
$$

Use [reduction of order](../../../../../../reduction-of-order.md): if $y_2=y_1v$, then $W=y_1^2v'$. Absorbing a nonzero Wronskian constant into the second integration constant, the general solution is

$$
\boxed{y(x)=C_1y_1(x)+C_2y_1(x)\int^x\frac{ds}{(1-s)y_1(s)^2}.}
$$

This local representation applies on intervals where $y_1\ne0$, in particular sufficiently near $x=1$ because $y_1(1)=a_0\ne0$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
