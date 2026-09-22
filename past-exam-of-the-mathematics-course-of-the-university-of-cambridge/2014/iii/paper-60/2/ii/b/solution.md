<h1 id="2/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the definitions of [conditional entropy](../../../../../../../conditional-entropy.md) and insert $H(X,Y)$:

$$
\begin{aligned}
H(Z,X\mid Y)&=H(Z,X,Y)-H(Y)\\
&=[H(X,Y)-H(Y)]+[H(Z,X,Y)-H(X,Y)]\\
&=H(X\mid Y)+H(Z\mid X,Y).
\end{aligned}
$$

Inserting $H(Z,Y)$ instead gives the alternative [chain rule for conditional entropy](../../../../../../../chain-rule-for-conditional-entropy.md)

$$
\boxed{H(Z,X\mid Y)=H(Z\mid Y)+H(X\mid Z,Y).}
$$

Both are expansions of the same joint conditional uncertainty, with the variables exposed in opposite orders.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [2](../../../2.md)
4. [Paper 60](../../../../paper-60-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
