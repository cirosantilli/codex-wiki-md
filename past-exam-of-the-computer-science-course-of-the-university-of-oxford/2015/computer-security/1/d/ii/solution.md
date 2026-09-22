<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the positive [integer](../../../../../../integer-split.md) $k$ whose existence is allowed by the question and write

$$
3^k=1+t(p-1)(q-1).
$$

Modulo $p$, if $c=0$ then $c^{3^k}=c$ directly. Otherwise [Fermat's little theorem](../../../../../../fermat-little-theorem.md) applies, since $3^k-1$ is a multiple of $p-1$. Hence $c^{3^k}=c\pmod p$. The same two-case argument works modulo $q$. By the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md),

$$
c^{3^k}\equiv c\pmod n,
$$

so

$$
\boxed{g_k=\gcd(c^{3^k}-c,n)=n.}
$$

This also covers a [ciphertext](../../../../../../ciphertext.md) that is not [coprime](../../../../../../coprime-integers.md) to $n$; applying [Euler's theorem](../../../../../../euler-s-theorem.md) without checking that hypothesis would miss this detail. Equivalently, repeated application of a [permutation](../../../../../../permutation.md) on a finite set eventually returns to the starting point, although the arithmetic argument gives the requested sufficient exponent.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
