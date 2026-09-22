<h1 id="11/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Assume any of conditions (i)–(iii). The established [reflexivity](../../../../../../reflexive-relation.md), [symmetry](../../../../../../symmetry-physics.md) and [transitivity](../../../../../../transitive-relation.md) make $T$ an [equivalence relation](../../../../../../equivalence-relation.md), and it contains both $R,S$. If $E$ is any [equivalence relation](../../../../../../equivalence-relation.md) containing $R,S$ and $xRaSz$, then $xEaEz$, so [transitivity](../../../../../../transitive-relation.md) of $E$ gives $xEz$. Thus $T\subseteq E$. This proves that **$T$ is the unique smallest equivalence relation containing $R$ and $S$**. Conversely, condition (iv) explicitly makes $T$ an [equivalence relation](../../../../../../equivalence-relation.md), so it has properties (i) and (ii). Together these implications prove all four conditions equivalent.

For the final integer example, let $g=\gcd(m,n)$. If $x\equiv y\pmod m$ and $y\equiv z\pmod n$, then $z-x$ is a sum of a multiple of $m$ and a multiple of $n$, so $x\equiv z\pmod g$. Conversely, if $g$ divides $z-x$, [Bezout identity](../../../../../../bezout-identity.md) provides integers $a,b$ with $z-x=am+bn$. Set $y=x+am$. Then $y-x$ is divisible by $m$ and $z-y$ by $n$, so $xRySz$. Therefore

$$
\boxed{R_m\circ R_n=R_{\gcd(m,n)}=R_n\circ R_m.}
$$

Interchanging $m,n$ gives the other equality. The composite is thus exactly congruence modulo the [greatest common divisor](../../../../../../greatest-common-divisor.md), an [equivalence relation](../../../../../../equivalence-relation.md), and all four equivalent conditions hold.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [11](../../11.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
