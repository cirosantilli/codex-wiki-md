<h1 id="4g/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

This language is **not context-free**. Suppose it were, and define the homomorphism

$$
h(a)=h(c)=a,qquad h(b)=h(d)=b.
$$

Then closure under inverse homomorphism and [intersection of a context-free language with a regular language](../../../../../../../intersection-of-a-context-free-language-with-a-regular-language.md) would make

$$
h^{-1}(L)cap a^+b^+c^+d^+
={a^m b^n c^m d^n:m,ngeq1}
$$

context-free. The equality holds because the midpoint of a square with four nonempty alternating runs must lie between its second and third runs.

Apply the [pumping lemma for context-free languages](../../../../../../../pumping-lemma-for-context-free-languages.md) to $a^pb^pc^pd^p$. A pumpable window of length at most $p$ meets at most two adjacent blocks. Pumping changes at least one block but cannot reach its equal-count partner two blocks away, so either the $a,c$ counts or the $b,d$ counts cease to agree. This contradiction proves the claim.

## ↑ Ancestors (12)

1. [I](../i.md)
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
