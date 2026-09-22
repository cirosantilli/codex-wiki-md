<h1 id="4g/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This language is **not context-free**. Let $p$ be a proposed [pumping length](../../../../../../../pumping-length.md) and choose $n$ with $3^n\geq p$. In any pumping decomposition of the unary word $a^{3^n}$, pumping once more increases its length by an integer $d$ with $1\leq d\leq p$. But

$$
3^n<3^n+d\leq2\cdot3^n<3^{n+1},
$$

so the pumped length is not a power of three, contrary to the [pumping lemma for context-free languages](../../../../../../../pumping-lemma-for-context-free-languages.md). This is also an instance of the fact that a [unary context-free language is regular](../../../../../../../unary-context-free-language-is-regular.md), whereas the powers of three are not ultimately periodic.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4G](../../../4g.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
