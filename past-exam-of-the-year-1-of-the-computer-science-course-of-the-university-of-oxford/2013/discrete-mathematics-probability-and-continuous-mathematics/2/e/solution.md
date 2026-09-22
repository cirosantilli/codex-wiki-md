<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In [modular arithmetic](../../../../../modular-arithmetic-split.md), calculations may be performed after replacing each input by its remainder. For a positive modulus $m$, write $[a]_m$ for the remainder in $\{0,\ldots,m-1\}$. Then

$$
\boxed{\begin{aligned}
[a+b]_m&=[[a]_m+[b]_m]_m,\\
[ab]_m&=[[a]_m[b]_m]_m,\\
[a^k]_m&=[[a]_m^k]_m\qquad(k\geq0).
\end{aligned}}
$$

Equivalently, if $a\equiv a'\pmod m$ and $b\equiv b'\pmod m$, addition and multiplication give $a+b\equiv a'+b'$ and $ab\equiv a'b'$, and a fixed nonnegative integer exponent gives $a^k\equiv(a')^k$. One cannot in general reduce the exponent modulo $m$ by this rule.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
