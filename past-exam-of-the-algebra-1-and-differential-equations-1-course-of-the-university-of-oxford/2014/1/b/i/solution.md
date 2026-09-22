<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Evaluate [Bézout's identity for polynomials](../../../../../bezout-s-identity-for-polynomials.md) at $T$:

$$
a(T)p(T)+b(T)q(T)=I,\qquad p(T)q(T)=0.
$$

All these [linear operators](../../../../../linear-operator.md) commute because they are [polynomials](../../../../../polynomial-split.md) in the same operator. Thus every $v\in V$ can be written

$$
v=b(T)q(T)v+a(T)p(T)v.
$$

The first summand belongs to $\ker p(T)$ and the second to $\ker q(T)$, since applying the corresponding operator introduces the product $p(T)q(T)=0$.

If $v$ lies in both [kernels](../../../../../kernel-of-a-linear-map-split.md), the same identity gives $v=0+0=0$. Therefore the sum is direct:

$$
\boxed{V=\ker p(T)\oplus\ker q(T).}
$$

This is the [kernel decomposition for coprime polynomials](../../../../../kernel-decomposition-for-coprime-polynomials.md). It uses both annihilation by $pq$ and the coprimality expressed by the Bézout identity.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
