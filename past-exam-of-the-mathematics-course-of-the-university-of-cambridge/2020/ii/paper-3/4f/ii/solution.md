<h1 id="4f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The language $L=\{a^{m^2}b^{m^2}:m\geq0\}$ is not [context-free](../../../../../../context-free-language.md). Suppose it had [pumping length](../../../../../../pumping-length.md) $p$ in the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md), and apply the lemma to $w=a^{p^2}b^{p^2}$. Write $w=uvxyz$ with $|vxy|\leq p$, $|vy|>0$, and $uv^ixy^iz\in L$ for every $i\geq0$.

Let $\alpha$ and $\beta$ be the respective numbers of $a$s and $b$s in $vy$. If $\alpha\ne\beta$, pumping with $i=0$ or $i=2$ destroys equality of the two block lengths. Hence a valid decomposition would require $\alpha=\beta=d>0$. Pumping with $i=2$ would then produce $a^{p^2+d}b^{p^2+d}$, where $1\leq d\leq p$. But

$$
p^2<p^2+d<(p+1)^2,
$$

so $p^2+d$ is not a [square number](../../../../../../square-number.md). This contradiction proves the [square-count language is not context-free](../../../../../../square-count-language-is-not-context-free.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4F](../../4f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
