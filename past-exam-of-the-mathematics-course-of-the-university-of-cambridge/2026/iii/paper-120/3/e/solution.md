<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take

$$
OR=\lambda a:Bool_\sigma.\lambda b:Bool_\sigma.
\lambda x:\sigma.\lambda y:\sigma.a\,x\,(b\,x\,y).
$$

It has type $Bool_\sigma\to Bool_\sigma\to Bool_\sigma$. If $a\equiv_\beta\top$, the body selects $x$. If $a\equiv_\beta\bot$, it reduces to $bxy$, which selects $x$ exactly when $b\equiv_\beta\top$. Thus it has the stated truth table.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
