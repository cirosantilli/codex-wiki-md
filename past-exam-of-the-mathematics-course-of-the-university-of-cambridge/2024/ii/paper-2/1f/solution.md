<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

A [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) $[a,b,c]$ satisfies

$$
|b|\leq a\leq c,
$$

with $b\geq0$ when either $|b|=a$ or $a=c$. For $d\equiv0$ or $3\pmod4$, the [class number of a negative discriminant](../../../../../class-number-of-a-negative-discriminant.md) $h(-d)$ is the number of proper equivalence classes of primitive positive definite [integral](../../../../../integral.md) forms of discriminant $-d$, equivalently the number of their reduced representatives.

Write

$$
d=\prod_{j=1}^k p_j^{e_j}.
$$

Partitioning the $k$ complete prime-power factors between $r$ and $s$ gives $2^k$ ordered factorizations $d=rs$ with $\gcd(r,s)=1$. After identifying $(r,s)$ with $(s,r)$, there are $2^{k-1}$ choices with $r\leq s$. Each gives the primitive reduced form

$$
[r,0,s],
$$

whose discriminant is $-4rs=-4d$. The uniqueness of reduced representatives makes these classes distinct, proving the [coprime-factorization lower bound for a quadratic-form class number](../../../../../coprime-factorization-lower-bound-for-a-quadratic-form-class-number.md)

$$
h(-4d)\geq2^{k-1}.
$$

The inequality can be strict. For $d=5$, there is one distinct prime factor, while the reduced primitive forms of discriminant $-20$ are

$$
[1,0,5]\quad\hbox{and}\quad[2,2,3].
$$

**Thus $h(-20)=2>1=2^{1-1}$.**

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
