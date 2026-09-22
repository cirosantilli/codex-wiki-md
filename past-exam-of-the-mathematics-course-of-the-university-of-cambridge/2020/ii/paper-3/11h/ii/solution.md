<h1 id="11h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) states that if $p\nmid a$ and $m$ of the least positive residues of

$$
a,2a,\ldots,\frac{p-1}{2}a
$$

exceed $p/2$, then $(a/p)=(-1)^m$.

To prove it, replace each residue exceeding $p/2$ by its negative, obtaining numbers $r_1,\ldots,r_{(p-1)/2}$ in $\{1,\ldots,(p-1)/2\}$. No two of them are equal modulo $p$: such an equality would give $ia\equiv\pm ja\pmod p$, hence $i=j$ in the allowed range. They therefore permute $1,\ldots,(p-1)/2$, and multiplication gives

$$
a^{(p-1)/2}\left(\frac{p-1}{2}\right)!
\equiv(-1)^m\left(\frac{p-1}{2}\right)!\pmod p.
$$

Cancel the nonzero factorial and apply [Euler's criterion](../../../../../../euler-s-criterion.md) to obtain the lemma.

For $a=-1$, all $(p-1)/2$ least positive residues $p-1,p-2,\ldots,(p+1)/2$ exceed $p/2$. Hence the [first supplementary law for quadratic reciprocity](../../../../../../first-supplementary-law-for-quadratic-reciprocity.md) is

$$
\boxed{\left(\frac{-1}{p}\right)=(-1)^{(p-1)/2}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11H](../../11h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
