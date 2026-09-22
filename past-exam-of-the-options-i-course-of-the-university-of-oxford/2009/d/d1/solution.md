<h1 id="d/d1/solution">Solution</h1>

↑ **Parent:** [D1](../d1.md)

The [Lebesgue outer measure](../../../../lebesgue-outer-measure.md) can be defined by

$$
m^*(E)=\inf\left\{\sum_{j=1}^{\infty}|I_j|:E\subseteq\bigcup_{j=1}^{\infty}I_j,\ I_j\text{ open intervals}\right\}.
$$

A [null set](../../../../null-set.md) has $m^*(E)=0$, equivalently it admits such a cover of total length below every positive $\varepsilon$.

The usual [Cantor set](../../../../cantor-set.md) is the [intersection](../../../../set-intersection.md) of the sets obtained from $[0,1]$ by repeatedly removing every open middle third. At stage $n$ there are $2^n$ closed intervals of length $3^{-n}$. Enlarge them slightly to open intervals whose total added length is below $\varepsilon$. Thus $m^*(C)\leq(2/3)^n+\varepsilon$ for every $n$ and $\varepsilon>0$, proving $m^*(C)=0$.

For the different deletion rule in this problem, let $L_n$ be the total length of the stage-$n$ intervals. Removing the stated fraction from each component gives

$$
L_{n+1}=L_n\frac{2^n+1}{2^n+2},\qquad L_0=1.
$$

For $n\geq1$ the [telescoping product](../../../../telescoping-product.md) simplifies to

$$
L_n=\prod_{j=0}^{n-1}\frac{2^j+1}{2^j+2}
=\frac23\prod_{j=1}^{n-1}\frac{2^j+1}{2(2^{j-1}+1)}
=\frac{2^{n-1}+1}{3\,2^{n-1}}.
$$

Because $K\subseteq K_n$, the same finite [interval](../../../../interval-mathematics.md)-enlargement argument gives $m^*(K)\leq L_n$. Taking the limit proves

$$
\boxed{m^*(K)\leq\frac13}.
$$

Only [interval](../../../../interval-mathematics.md) covers and their lengths were used; no [continuity](../../../../continuous-function.md) theorem for integrals is needed.

## ↑ Ancestors (12)

1. [D1](../d1.md)
2. [D](../../d.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
