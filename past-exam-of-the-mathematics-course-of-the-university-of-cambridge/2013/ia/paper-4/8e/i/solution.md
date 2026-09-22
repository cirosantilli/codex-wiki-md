<h1 id="8e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [Fermat's little theorem](../../../../../../fermat-little-theorem.md), first suppose $p\nmid x$. Multiplication by $x$ permutes the nonzero residue classes modulo $p$: if $xa\equiv xb\pmod p$, the prime cannot divide $x$, so cancellation gives $a\equiv b\pmod p$. Multiplying the representatives in this permutation,

$$
x^{p-1}(p-1)!\equiv(p-1)!\pmod p.
$$

Every factor of the factorial is nonzero modulo the prime, so the factorial has a [modular inverse](../../../../../../modular-multiplicative-inverse.md) and can be cancelled. Thus $x^{p-1}\equiv1\pmod p$ and $x^p\equiv x\pmod p$. If $p\mid x$, both sides are zero modulo $p$. Hence for every integer $x$,

$$
\boxed{x^p\equiv x\pmod p.}
$$

For completeness, the cancellation used above follows from [Bézout's identity](../../../../../../bezout-identity.md): a number relatively prime to $p$ has an inverse modulo $p$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
