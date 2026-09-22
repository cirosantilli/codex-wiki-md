<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For functions with the required [derivatives](../../../../../derivative.md), the [Leibniz rule](../../../../../leibniz-rule.md) is

$$
(fg)^{(n)}=\sum_{k=0}^n\binom nk f^{(k)}g^{(n-k)}.
$$

At $n=0$ it is immediate. If it holds at $n$, differentiating each summand gives two sums. The coefficient of $f^{(k)}g^{(n+1-k)}$ after regrouping is $\binom nk+\binom n{k-1}=\binom{n+1}k$ by [Pascal's identity](../../../../../pascal-s-rule.md), including the two endpoint terms. This proves the formula by [mathematical induction](../../../../../mathematical-induction.md).

Apply it to $(fg)h$ and then expand the derivatives of $fg$. For $p+q+r=n$, the resulting coefficient is $\binom n{p+q}\binom{p+q}p=n!/(p!q!r!)$. Consequently

$$
\boxed{(fgh)^{(n)}=\sum_{p+q+r=n}\frac{n!}{p!q!r!}f^{(p)}g^{(q)}h^{(r)},}
$$

where $p,q,r$ range over nonnegative integers. This is the three-factor [generalized Leibniz rule](../../../../../generalized-leibniz-rule.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
