<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write

$$
a_1(E_k)=\frac{2}{\zeta(1-k)}=\frac rs,
\qquad \gcd(r,s)=1,
$$

and suppose $p\mid s$. In the basis from part b, comparison of the constant term and the first $N$ nonconstant coefficients gives

$$
sE_k=sf_0+r\sum_{i=1}^N\sigma_{k-1}(i)f_i.
$$

Indeed, $f_0$ has constant term one and no terms $q,ldots,q^N$, while $f_i$ has the sole term $q^i$ in that range.

Set

$$
f=\sum_{i=1}^N\sigma_{k-1}(i)f_i.
$$

Every $f_i$ with $i\geq1$ vanishes at infinity and is therefore a [cusp form](../../../../../../cusp-form.md); moreover $f$ has integral coefficients. Comparing the coefficient of $q^n$ in the displayed identity gives

$$
r\sigma_{k-1}(n)=s,a_n(f_0)+r,a_n(f).
$$

Reduction modulo $p$ kills the first term on the right. Since $p\nmid r$, cancellation of $r$ yields

$$
a_n(f)\equiv\sigma_{k-1}(n)\pmod p
$$

for every $n\geq1$, proving the [Eisenstein congruence from a denominator prime](../../../../../../eisenstein-congruence-from-a-denominator-prime.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
