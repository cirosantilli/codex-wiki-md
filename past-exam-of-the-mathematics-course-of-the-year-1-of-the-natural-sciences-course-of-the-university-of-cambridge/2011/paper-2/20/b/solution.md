<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating $v=x^ne^{-x}$ gives $xv'=(n-x)v$. Applying the [Leibniz rule](../../../../../leibniz-rule.md) $n+1$ times to this identity gives

$$
xv^{(n+2)}+(n+1)v^{(n+1)}=(n-x)v^{(n+1)}-(n+1)v^{(n)}.
$$

Only two terms survive on each side because the multiplying factors are linear. Rearranging yields $xv^{(n+2)}+(x+1)v^{(n+1)}+(n+1)v^{(n)}=0$. Since $v^{(n)}=n!e^{-x}L_n$, the next two [derivatives](../../../../../derivative.md) are $n!e^{-x}(L_n'-L_n)$ and $n!e^{-x}(L_n''-2L_n'+L_n)$. Substituting and cancelling $n!e^{-x}$ gives

$$
\boxed{xL_n''+(1-x)L_n'+nL_n=0}.
$$

This is [deriving the Laguerre equation from Rodrigues' formula](../../../../../deriving-the-laguerre-equation-from-rodrigues-formula.md), exhibiting $L_n$ as an [eigenfunction](../../../../../eigenfunction.md) of the [Laguerre differential operator on polynomials](../../../../../laguerre-differential-operator-on-polynomials.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
