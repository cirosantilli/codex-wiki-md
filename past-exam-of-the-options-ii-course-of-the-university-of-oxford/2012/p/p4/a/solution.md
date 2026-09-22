<h1 id="p/p4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Subtract the two finite sums. In the shifted sum replace the summation index $k$ by $k-1$. For every interior index the new [coefficient](../../../../../coefficient.md) is

$$
(-1)^k\binom rk-(-1)^{k-1}\binom r{k-1}=(-1)^k\binom{r+1}k
$$

by [Pascal's identity](../../../../../pascal-s-rule.md); the two endpoint [coefficients](../../../../../coefficient.md) agree as well. Therefore

$$
\boxed{Q_{(r)}(x)-Q_{(r)}(x-h)=Q_{(r+1)}(x).}
$$

For a degree-$d$ [polynomial](../../../../../polynomial-split.md) with [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $c\neq0$, the backward difference has leading term

$$
c\bigl(x^d-(x-h)^d\bigr)=cdh\,x^{d-1}+\text{lower-degree terms}.
$$

Since $h>0$, this [coefficient](../../../../../coefficient.md) is nonzero for $d\geq1$. Starting with $Q_{(0)}=P$, iteration gives [degree](../../../../../degree-of-a-polynomial.md) $n-r$ and [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $c h^r n!/(n-r)!$ for $0\leq r\leq n$. The next difference of the resulting constant is zero:

$$
\boxed{\deg Q_{(r)}=n-r\ (0\leq r\leq n),\qquad Q_{(n+1)}\equiv0.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
