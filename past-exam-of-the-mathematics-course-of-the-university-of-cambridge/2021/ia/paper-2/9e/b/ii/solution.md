<h1 id="9e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Call the coins $1,2,3$ in the order given. Coin 1 beats the constant score of coin 2 exactly when it shows a head, so coin 1 wins with probability $3/5$. Coin 2 beats coin 3 exactly when coin 3 shows a head and scores three, again with probability $3/5$.

Coin 3 beats coin 1 whenever coin 3 shows a tail, or when coin 3 shows a head and coin 1 shows a tail. Its winning probability is therefore

$$
\frac25+\frac35\frac25
=\frac{16}{25}>\frac12.
$$

Thus the preferences form a nontransitive cycle:

$$
1\text{ beats }2,\qquad
2\text{ beats }3,\qquad
3\text{ beats }1.
$$

The second chooser can always select a coin that has winning probability greater than one half against the first choice. Therefore

$$
\boxed{\text{it is preferable to choose second}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9E](../../../9e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
