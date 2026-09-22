<h1 id="11i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For odd coprime positive [integers](../../../../../../integer.md) $a=\prod_i p_i^{e_i}$ and $b=\prod_j q_j^{f_j}$, define the [Jacobi symbol](../../../../../../jacobi-symbol.md) by multiplying [Legendre symbols](../../../../../../legendre-symbol.md) over the prime factorization of the denominator. Multiplicativity in the numerator gives

$$
\left(\frac ab\right)\left(\frac ba\right)=\prod_{i,j}\left[\left(\frac{p_i}{q_j}\right)\left(\frac{q_j}{p_i}\right)\right]^{e_if_j}.
$$

By [quadratic reciprocity](../../../../../../quadratic-reciprocity.md) for the [Legendre symbol](../../../../../../legendre-symbol.md), this is $(-1)^{UV}$, where $U=\sum_i e_i(p_i-1)/2$ and $V=\sum_j f_j(q_j-1)/2$. For odd $x,y$, $(xy-1)/2\equiv(x-1)/2+(y-1)/2\pmod2$, since $(x-1)(y-1)/2$ is even. Thus $U\equiv(a-1)/2$ and $V\equiv(b-1)/2\pmod2$. We obtain

$$
\boxed{\left(\frac ab\right)\left(\frac ba\right)=(-1)^{(a-1)(b-1)/4}.}
$$

If $a,b$ are not coprime, both symbols are zero and the equivalent identity $(a/b)=(-1)^{(a-1)(b-1)/4}(b/a)$ still holds. The convention $(a/1)=1$ handles denominator one.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11I](../../11i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
