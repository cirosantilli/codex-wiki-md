<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Euler's totient function](../../../../euler-totient-function.md) counts the [integers](../../../../integer-split.md) in a complete [complete residue system](../../../../complete-residue-system.md) that are [coprime](../../../../coprime-integers.md) to the modulus:

$$
\boxed{\phi(n)=\#\{1\leq a\leq n:\gcd(a,n)=1\}.}
$$

If the [prime factorization](../../../../fundamental-theorem-of-arithmetic.md) is $n=\prod_{j=1}^r p_j^{e_j}$ with distinct [prime numbers](../../../../prime-number-split.md) $p_j$, [Euler's totient product formula](../../../../euler-s-totient-product-formula.md) is

$$
\boxed{\phi(n)=n\prod_{j=1}^r\left(1-\frac1{p_j}\right)
=\prod_{j=1}^r p_j^{e_j-1}(p_j-1).}
$$

In particular, $\phi(2017)=2016$. Adjoining the [prime factor](../../../../prime-factor.md) $2$ changes neither the odd factor nor its count of [units](../../../../unit-in-a-ring.md), since $\phi(2)=1$. The product formula gives

$$
\boxed{n=4034=2\cdot2017,\qquad\phi(4034)=(2-1)(2017-1)=2016.}
$$

This is a positive [integer](../../../../integer-split.md) distinct from $2017$, as required.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
