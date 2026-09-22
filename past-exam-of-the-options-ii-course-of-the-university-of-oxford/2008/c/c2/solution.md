<h1 id="c/c2/solution">Solution</h1>

↑ **Parent:** [C2](../c2.md)

The $d$ distinct powers $1,a,\ldots,a^{d-1}$ all solve $X^d=1$. By the allowed root bound they are all its solutions. A [residue](../../../../residue.md) $b$ of order $d$ must therefore equal $a^j$; conversely $\operatorname{ord}(a^j)=d/\gcd(d,j)$, because $d\mid jt$ characterizes the exponents $t$ with $(a^j)^t=1$. This proves the equivalence with $\gcd(d,j)=1$ and gives exactly $\varphi(d)$ elements of order $d$ whenever any such element exists.

To establish existence at the full order too, put $m=p-1$ and let $N_d$ count elements of order $d$. By [Lagrange's theorem for finite groups](../../../../lagrange-s-theorem.md), these orders divide $m$. The first result gives $N_d=0$ or $\varphi(d)$. Therefore

$$
m=\sum_{d\mid m}N_d\leq\sum_{d\mid m}\varphi(d)=m,
$$

using the standard divisor-sum identity for Euler's [function](../../../../function-split.md). Equality forces every deficit to vanish, so $N_m=\boxed{\varphi(p-1)}$.

Finally let $h=g^{(p-1)/8}$, which has order eight. Its fourth power is the unique nonidentity square root of one, namely $-1$. Since $h^7=h^{-1}$,

$$
(h+h^{-1})^2=h^2+2+h^{-2}=2,
$$

because $h^{-2}=h^6=-h^2$. This proves **the stated [residue](../../../../residue.md) squares to two**.

## ↑ Ancestors (12)

1. [C2](../c2.md)
2. [C](../../c.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
