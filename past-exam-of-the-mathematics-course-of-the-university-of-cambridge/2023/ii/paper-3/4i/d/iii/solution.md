<h1 id="4i/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The first grammar generates

$$
L(G_0)=\{ab^{2r+1}a:r\geq0\},
$$

because $A\to bAb$ adds two $b$'s and $A\to b$ terminates the derivation.

In the second grammar, $Z$ is a [nonproductive nonterminal](../../../../../../../nonproductive-nonterminal.md): every right-hand side of a $Z$-production still contains a $Z$. Consequently the branch $Y\to ZZ$ never yields a terminal word. Every terminal derivation from $Y$ instead uses $Y\to bYb$ repeatedly and ends with $Y\to b$, so

$$
L(G_1)=\{ab^{2r+1}a:r\geq0\}=L(G_0).
$$

The grammars are therefore [equivalent](../../../../../../../equivalent-grammar.md), although they are not [isomorphic](../../../../../../../isomorphic-grammar.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [4I](../../../4i.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
