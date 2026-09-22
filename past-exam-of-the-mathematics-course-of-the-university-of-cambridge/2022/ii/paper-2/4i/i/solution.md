<h1 id="4i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md) states that if $L$ is regular, then some $p\geq1$ has the following property: every $w\in L$ with $|w|\geq p$ can be written $w=xyz$ with $|xy|\leq p$, $|y|\geq1$, and $xy^iz\in L$ for every $i\geq0$. Indeed, while a deterministic finite automaton with $p$ states reads the first $p$ symbols, two of the first $p+1$ visited states coincide; the intervening nonempty loop may be traversed any number of times.

The language $\{0^{n^2}1:n\geq0\}$ is not regular. If its pumping length were $p$, apply the lemma to $w=0^{p^2}1$. The pumped block is $y=0^r$ for some $1\leq r\leq p$. Pumping once more gives $p^2+r$ zeros, but

$$
p^2<p^2+r<(p+1)^2,
$$

so their number is not a square.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4I](../../4i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
