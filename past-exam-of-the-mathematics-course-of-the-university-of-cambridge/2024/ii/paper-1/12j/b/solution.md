<h1 id="12j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an input word $w$ of length at least $n+1$. The final value $f_{M,1}(w)=\chi_L(w)$ has length at most one. Every symbol initially in register $0$ must either be deleted or transferred elsewhere, and either action begins with a remove instruction

$$
-(0,q,q').
$$

No other instruction can lower the length of register $0$. Consequently at least

$$
|w|-1\geq n
$$

such remove instructions occur in this computation. Since words of arbitrary length exist, the assertion follows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12J](../../12j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
