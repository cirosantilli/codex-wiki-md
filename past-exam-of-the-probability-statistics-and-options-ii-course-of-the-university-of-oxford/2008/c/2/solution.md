<h1 id="c/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The $d$ distinct powers $1,a,\ldots,a^{d-1}$ all satisfy $X^d=1$. The supplied root bound says they exhaust those roots. Thus every element of order $d$ has the form $a^n$. If $g=\gcd(n,d)$, the least positive $k$ with $a^{nk}=1$ is $d/g$, so

$$
\boxed{\operatorname{ord}_p(a^n)=\frac d{\gcd(n,d)}.}
$$

This proves both directions of the first assertion.

For existence of a [primitive root](../../../../primitive-root-modulo-n.md) one may apply the finite-[field](../../../../field.md) cyclicity criterion proved in the preceding section. There is also a direct counting proof: for each divisor $d$ of $p-1$, either no elements have order $d$, or the preceding argument shows there are exactly $\phi(d)$. [Lagrange's theorem](../../../../lagrange-s-theorem.md) partitions all $p-1$ nonzero [residue](../../../../residue.md) classes by such orders, while $\sum_{d\mid p-1}\phi(d)=p-1$. Every count is at most its corresponding $\phi(d)$, so equality of the totals forces equality at every divisor. In particular there are $\boxed{\phi(p-1)}$ [primitive roots](../../../../primitive-root-modulo-n.md).

Put $t=g^{(p-1)/8}$. It has order eight, so $t^4=-1$ and $t^8=1$. The specified element is $k=t+t^7=t+t^{-1}$. Since $t^{-2}=-t^2$, squaring gives $\boxed{k^2=t^2+2+t^{-2}=2\pmod p}$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [C](../../c.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
