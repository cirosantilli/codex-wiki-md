<h1 id="c/2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) and [multiplicativity](../../../../../../multiplicativity-of-an-arithmetic-function.md) to check the identity one [prime](../../../../../../prime-number-split.md) at a time. Fix $p$ and put $a=v_p(m)$, $b=v_p(n)$, $r=\min(a,b)$. The local factors to compare are

$$
\phi(p^{a+b})\phi(p^r)\quad\text{and}\quad
\phi(p^a)\phi(p^b)p^r.
$$

If either exponent is zero, $r=0$ and the equality follows from $\phi(1)=1$. If both are positive, the prime-power formula makes both sides

$$
p^{a+b+r-2}(p-1)^2.
$$

Multiplying the local identities over all [primes](../../../../../../prime-number-split.md) and using $\gcd(m,n)=\prod_p p^{\min(v_p(m),v_p(n))}$ gives

$$
\boxed{\phi(mn)\phi(\gcd(m,n))=\phi(m)\phi(n)\gcd(m,n).}
$$

This accounts for repeated [prime factors](../../../../../../prime-factor.md) shared by the two inputs, which ordinary [coprime](../../../../../../coprime-integers.md) [multiplicativity](../../../../../../multiplicativity-of-an-arithmetic-function.md) alone would not remove.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [C](../../../../c.md)
5. [2005](../../../../../2005-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
