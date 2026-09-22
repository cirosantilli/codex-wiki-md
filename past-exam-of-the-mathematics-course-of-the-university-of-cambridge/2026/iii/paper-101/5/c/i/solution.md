<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $P=p_1\cdots p_n$ and $A=\mathbb Z/P\mathbb Z=R_0$. By the [Chinese remainder theorem](../../../../../../../chinese-remainder-theorem.md), $A\cong\prod_i\mathbb F_{p_i}$, so $\operatorname{length}_A(A)=n$.

If a positive-degree monomial contains both $t_i$ and $t_j$ with $i\ne j$, then it vanishes: [Bezout identity](../../../../../../../bezout-identity.md) gives $u p_i+v p_j=1$, while both $p_i$ and $p_j$ annihilate that monomial. Thus the degree-$d$ component for $d\ge1$ is

$$
R_d\cong\bigoplus_{i=1}^n A/(p_i),
$$

and every summand has length one. Hence every $R_d$ has length $n$, including $d=0$, and

$$
\boxed{P_R(z)=\sum_{d\ge0}nz^d=\frac{n}{1-z}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 101](../../../../paper-101-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
