<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The graph factorizes as

$$
p(x)=p(x_2)p(x_1\mid x_2)p(x_4\mid x_2)
p(x_3\mid x_1,x_4)p(x_5\mid x_2)
p(x_6\mid x_4,x_5).
$$

Conditioning on all variables except $X_1$, terms not involving $x_1$ cancel, leaving

$$
p(x_1\mid x_2,x_3,x_4,x_5,x_6)
\propto p(x_1\mid x_2)p(x_3\mid x_1,x_4).
$$

This depends only on $(x_2,x_3,x_4)$, so

$$
X_1\perp(X_5,X_6)\mid(X_2,X_3,X_4).
$$

**Thus $(X_2,X_3,X_4)$ is a [Markov blanket](../../../../../../markov-blanket.md) of $X_1$.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
