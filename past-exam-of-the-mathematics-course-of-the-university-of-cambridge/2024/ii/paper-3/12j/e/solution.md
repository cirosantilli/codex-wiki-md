<h1 id="12j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose a language $L\subseteq\{0,1\}^*$ that is not recursively enumerable; such a language exists because there are uncountably many languages but only countably many algorithms. Form $\widehat L$ as in part (d), which satisfies the pumping lemma.

If a grammar generated $\widehat L$, enumerate its terminal derivations and retain precisely words of the form $2v$ with $v\in\{0,1\}^*$. Since such a word contains only one separator,

$$
2v\in\widehat L\quad\Longleftrightarrow\quad v\in L.
$$

This would enumerate $L$, a contradiction. Hence $\widehat L$ is the required language.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [12J](../../12j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
