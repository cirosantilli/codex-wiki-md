<h1 id="11i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $k=0$, the convention $0^0=1$ gives $S_0=p\equiv0\pmod p$. Now suppose $1\leq k<p-1$ and choose a [primitive root](../../../../../../primitive-root-modulo-n.md) $g$ modulo $p$. The nonzero residues are $g^j$ for $0\leq j\leq p-2$, while the $x=0$ term vanishes. Hence

$$
S_k\equiv\sum_{j=0}^{p-2}g^{jk}\pmod p.
$$

This is a [finite geometric series](../../../../../../finite-geometric-series.md). Since $g^k\not\equiv1\pmod p$ but $g^{k(p-1)}\equiv1\pmod p$ by [Fermat's little theorem](../../../../../../fermat-little-theorem.md), multiplication by the nonzero residue $g^k-1$ gives

$$
(g^k-1)S_k\equiv g^{k(p-1)}-1\equiv0\pmod p.
$$

The factor $g^k-1$ is invertible modulo the [prime number](../../../../../../prime-number.md) $p$, so

$$
\boxed{S_k\equiv0\pmod p.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11I](../../11i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
