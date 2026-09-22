<h1 id="11f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**The statement is false.** Take two independent fair bits $U,V$ on the four equally probable outcomes $00,01,10,11$, and put $A_1=\{U=0\}$, $A_2=\{V=0\}$, and $B=\{U=V\}$. Each of $A_1,A_2,B$ has probability $1/2$, and

$$
P(B\cap A_1)=P(B\cap A_2)=\frac14=P(B)P(A_i).
$$

Thus $B$ is independent of each event separately. But $A_1\cup A_2$ contains $00,01,10$, whereas its intersection with $B$ contains only $00$. Therefore

$$
P(B\cap(A_1\cup A_2))=\frac14
\ne\frac12\cdot\frac34=P(B)P(A_1\cup A_2).
$$

This is a concrete failure of extending separate [independence](../../../../../../independent-random-variables.md) to the generated union. A counterexample at the permitted value $n=2$ disproves the universal claim; for any larger $n$ one can repeat $A_1$ as the additional events.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
