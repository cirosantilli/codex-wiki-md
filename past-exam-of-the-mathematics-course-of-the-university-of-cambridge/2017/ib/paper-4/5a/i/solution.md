<h1 id="5a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The original PDF contains this subpart; the local TeX has omitted it. Write $a_n$ for the [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md) of $P_n$. The [Legendre polynomial recurrence relation](../../../../../../legendre-polynomial-recurrence-relation.md) and the starting [polynomials](../../../../../../polynomial-split.md) give $a_0=a_1=1$, and induction gives

$$
a_{n+1}=\frac{2n+1}{n+1}a_n>0.
$$

Indeed, $xP_n$ has [degree of a polynomial](../../../../../../degree-of-a-polynomial.md) $n+1$, while $P_{n-1}$ has smaller [degree of a polynomial](../../../../../../degree-of-a-polynomial.md) and cannot cancel its leading term. Hence

$$
\boxed{\deg P_n=n}.
$$

At $x=1$, the same [linear recurrence relation](../../../../../../linear-recurrence-relation.md) gives $(n+1)P_{n+1}(1)=(2n+1)P_n(1)-nP_{n-1}(1)$. Starting from $P_0(1)=P_1(1)=1$, induction yields

$$
\boxed{P_n(1)=1\quad(n\geq0)}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5A](../../5a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
