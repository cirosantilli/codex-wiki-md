<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) of the [binary string](../../../../../binary-string.md), the set positions have weights $2^{15},2^{13},2^{12},2^{11},2^{10},2^8,2^6,2^5,2^4$. Thus

$$
\boxed{u=2^{15}+2^{13}+2^{12}+2^{11}+2^{10}+2^8+2^6+2^5+2^4=48496.}
$$

In 16-[bit](../../../../../bit.md) [two's complement](../../../../../two-s-complement.md), the [most significant bit](../../../../../most-significant-bit.md) is set, so subtract $2^{16}$ from that [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md):

$$
\boxed{z=48496-65536=-17040.}
$$

For a [half-precision floating-point number](../../../../../half-precision-floating-point-format.md), split the fields at their actual boundaries rather than the printed groups of four:

$$
1\;01111\;0101110000.
$$

The sign is negative, the true [exponent](../../../../../exponent.md) is $15-15=0$, and the fraction is $2^{-2}+2^{-4}+2^{-5}+2^{-6}=23/64$. It is a normal finite value, so

$$
\boxed{x=-\left(1+2^{-2}+2^{-4}+2^{-5}+2^{-6}\right)2^0=-\frac{87}{64}=-1.359375.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
