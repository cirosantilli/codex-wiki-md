<h1 id="11g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First, every nonzero nonunit in a [principal ideal domain](../../../../../../principal-ideal-domain.md) factors into [irreducible elements](../../../../../../irreducible-element.md). Otherwise repeatedly choose a proper nonunit factor $a_{j+1}$ of $a_j$; then the principal ideals

$$
(a_1)\subsetneq(a_2)\subsetneq\cdots
$$

form a strictly increasing chain, contradicting the [ascending chain condition](../../../../../../ascending-chain-condition.md), since every principal ideal domain is a [Noetherian ring](../../../../../../noetherian-ring.md).

Next every irreducible $p$ is a [prime element](../../../../../../prime-element.md). If $p\mid ab$ but $p\nmid a$, then $\gcd(p,a)=1$. The [Bezout identity](../../../../../../bezout-identity.md) gives $up+va=1$, so multiplying by $b$ shows $p\mid b$. Thus irreducibles are prime.

Existence of an irreducible factorization and primality give uniqueness: an irreducible on one side divides the product on the other, hence is associate to one factor; cancel and continue. **Therefore every principal ideal domain is a [unique factorization domain](../../../../../../unique-factorization-domain.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11G](../../11g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
