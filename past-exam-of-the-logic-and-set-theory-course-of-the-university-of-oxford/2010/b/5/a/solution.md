<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The recursive definitions of [ordinal addition](../../../../../ordinal-addition.md) and [ordinal multiplication](../../../../../ordinal-multiplication.md) are

$$
\alpha+0=\alpha,\quad\alpha+(\beta+1)=(\alpha+\beta)+1,\quad
\alpha+\lambda=\sup_{\beta<\lambda}(\alpha+\beta),
$$



$$
\alpha\cdot0=0,\quad\alpha\cdot(\beta+1)=\alpha\cdot\beta+\alpha,\quad
\alpha\cdot\lambda=\sup_{\beta<\lambda}(\alpha\cdot\beta),
$$

where the limit clauses apply to nonzero limit [ordinals](../../../../../ordinal-split.md). [Ordinal exponentiation](../../../../../ordinal-exponentiation.md) has $\alpha^0=1$, $\alpha^{\beta+1}=\alpha^\beta\cdot\alpha$, and for $\alpha>0$, $\alpha^\lambda=\sup_{\beta<\lambda}\alpha^\beta$. Complete the zero-base convention by $0^\beta=0$ for $\beta>0$, with $0^0=1$. Stating the zero-base exception avoids including the value $0^0$ in a naive supremum at a positive limit.

For finite $n$, induction gives $1+n=n+1$. Now prove commutativity for finite $m,n$ by induction on $m$. The case $m=0$ is immediate. Associativity, the finite identity just obtained, and the induction hypothesis give

$$
(m+1)+n=m+(1+n)=m+(n+1)=(m+n)+1=(n+m)+1=n+(m+1).
$$

Thus $\boxed{m+n=n+m\text{ for finite ordinals}}$.

It fails for general [ordinals](../../../../../ordinal-split.md): $\boxed{1+\omega=\omega<\omega+1}$. The equality follows from the limit clause, since the finite sums $1+n$ are cofinal in $\omega$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
