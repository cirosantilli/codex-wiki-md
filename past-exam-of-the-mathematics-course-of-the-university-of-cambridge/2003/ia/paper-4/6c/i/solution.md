<h1 id="6c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [prime number](../../../../../../prime-number.md) $p$, every nonzero [residue class](../../../../../../residue-class.md) has a unique multiplicative inverse modulo $p$: [Bezout identity](../../../../../../bezout-identity.md) supplies one because its representative is [coprime](../../../../../../coprime-integers.md) to $p$, and cancellation modulo a prime gives uniqueness. Pair each residue with its inverse. The only unpaired residues satisfy $a^2\equiv1$, so $p\mid(a-1)(a+1)$; the [Euclid lemma](../../../../../../euclid-lemma.md) gives $a\equiv1$ or $-1$. For odd $p$, these are distinct. Every other pair contributes one to the product of all nonzero residues, leaving

$$
(p-1)!\equiv1\cdot(-1)\equiv-1\pmod p.
$$

For $p=2$, $1!\equiv-1\pmod2$ as well. This proves [Wilson theorem](../../../../../../wilson-s-theorem.md) in all cases.

For an odd prime, set $q=(p-1)/2$. Pair the upper half of the factorial with the negatives of the lower half:

$$
(p-1)!=q!\prod_{r=1}^q(p-r)\equiv(-1)^q(q!)^2\pmod p.
$$

If $p\equiv1\pmod4$, then $q$ is even. Therefore

$$
\boxed{\left[\left(\frac{p-1}{2}\right)!\right]^2\equiv-1\pmod p}.
$$

This constructs a [square root of minus one modulo a prime](../../../../../../square-root-of-minus-one-modulo-a-prime.md) explicitly.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6C](../../6c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
