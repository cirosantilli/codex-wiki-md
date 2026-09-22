<h1 id="4i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the claim by induction on the length of the [grammar derivation](../../../../../../grammar-derivation.md) from $S$. At length zero the sentential form is $S=\epsilon S$, which has the required form.

Suppose the current sentential form is $wA$. Because $w$ is terminal, the only symbol to which a production can apply is $A$. A production $A\to uB$ produces

$$
wA\Rightarrow wuB,
$$

again a terminal word followed by one variable. A production $A\to u$ produces the terminal word $wu$. Once a completely terminal word is reached, no further production can apply. The induction proves the [sentential form of a right-linear regular grammar](../../../../../../sentential-form-of-a-right-linear-regular-grammar.md): every reachable $\alpha$ is either $wA$ or $w$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4I](../../4i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
