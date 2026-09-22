<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $\gcd(m,|H|)=1$, choose $r$ with $mr\equiv1\pmod{|H|}$ by the [Bezout identity](../../../../../../../bezout-identity.md). The [Lagrange theorem](../../../../../../../lagrange-s-theorem.md) gives $x^{|H|}=1$ for every $x\in H$, so $(x^m)^r=x$ and $(x^r)^m=x$. Thus $x\mapsto x^m$ is bijective, even though it need not be a homomorphism.

Conversely, if a prime $p$ divides both $m$ and $|H|$, the [Cauchy theorem for groups](../../../../../../../cauchy-theorem-for-groups.md) gives $x\ne1$ with $x^p=1$. Then $x^m=1$, so the power map sends both $x$ and the identity to the identity and is not injective. This proves the [power-map criterion for a finite group](../../../../../../../power-map-criterion-for-a-finite-group.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 151](../../../../paper-151-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
