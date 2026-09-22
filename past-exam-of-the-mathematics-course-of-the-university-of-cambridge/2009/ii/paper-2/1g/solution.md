<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

For odd positive coprime integers, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) for the [Jacobi symbol](../../../../../jacobi-symbol.md) is

$$
\boxed{\left(\frac mn\right)\left(\frac nm\right)=(-1)^{(m-1)(n-1)/4}.}
$$

If the integers are not coprime, both symbols vanish; equivalently the usual signed reciprocity identity still holds. To deduce it from [quadratic reciprocity](../../../../../quadratic-reciprocity.md) for the [Legendre symbol](../../../../../legendre-symbol.md), factor $m=\prod_i p_i^{a_i}$ and $n=\prod_jq_j^{b_j}$. Multiplication of the prime reciprocity identities gives the sign exponent

$$
\sum_{i,j}a_ib_j\frac{p_i-1}{2}\frac{q_j-1}{2}
=\left(\sum_i a_i\frac{p_i-1}{2}\right)\left(\sum_j b_j\frac{q_j-1}{2}\right).
$$

Modulo two, each bracket is respectively $(m-1)/2$ and $(n-1)/2$: for odd $u,v$, $(uv-1)/2\equiv(u-1)/2+(v-1)/2\pmod2$. This proves the composite-denominator law, including repeated prime factors.

Now $261=9\cdot29$, and 9 contributes a square factor. Since $317\equiv1\pmod4$, reciprocity and reduction of the numerator give

$$
\left(\frac{261}{317}\right)=\left(\frac{29}{317}\right)=\left(\frac{27}{29}\right)=\left(\frac3{29}\right).
$$

A second reciprocity step gives $(3/29)=(29/3)(-1)^{14}=(2/3)=-1$. Thus **the requested [Jacobi symbol](../../../../../jacobi-symbol.md) is $-1$**.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
