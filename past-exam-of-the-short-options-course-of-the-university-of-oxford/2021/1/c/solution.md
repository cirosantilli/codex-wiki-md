<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $P=\prod_i p_i$, $Q=\prod_j q_j$, counting repetitions. Since $P,Q$ are [coprime](../../../../coprime-integers.md), every pair $p_i,q_j$ consists of distinct odd [prime numbers](../../../../prime-number-split.md). [Quadratic reciprocity](../../../../quadratic-reciprocity.md) for the [Legendre symbol](../../../../legendre-symbol.md) gives

$$
\left(\frac{p_i}{q_j}\right)=(-1)^{((p_i-1)/2)((q_j-1)/2)}\left(\frac{q_j}{p_i}\right).
$$

Multiplying over all $i,j$ and using [multiplicativity of the Jacobi symbol](../../../../multiplicativity-of-the-jacobi-symbol.md) yields the sign exponent

$$
\left(\sum_i\frac{p_i-1}{2}\right)\left(\sum_j\frac{q_j-1}{2}\right)\equiv\frac{P-1}{2}\frac{Q-1}{2}\pmod2,
$$

by the odd-product parity identity proved in (b)(i). Thus the [Jacobi reciprocity law](../../../../jacobi-reciprocity-law.md) is

$$
\boxed{\left(\frac P Q\right)=(-1)^{(P-1)(Q-1)/4}\left(\frac Q P\right).}
$$

If either integer is $1$, its factorization is empty and both sides equal $1$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
