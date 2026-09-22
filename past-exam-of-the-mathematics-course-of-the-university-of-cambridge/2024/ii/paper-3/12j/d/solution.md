<h1 id="12j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take pumping length $p=1$. If a nonempty word $w\in\{0,1\}^*$, pump its first symbol; every pumped word remains in $\{0,1\}^*$. Otherwise write $w=u2v$ with $v\in L$. If $u\ne\varepsilon$, pump the first symbol of $u$, leaving a word of the same form. If $u=\varepsilon$, pump the initial $2$: deleting it leaves $v\in\{0,1\}^*$, while retaining one or more copies lets the last pumped $2$ serve as the separator. Thus every required pumped word belongs to $\widehat L$.

## ↑ Ancestors (11)

1. [D](../d.md)
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
