<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider an occurrence counted by $G_m$. Before the next counted occurrence, the exploration must first take a downward step of the [simple symmetric random walk](../../../../../../../simple-symmetric-random-walk.md), which has probability $1/2$, and then choose the decrement $-1$ among the three equally likely values of $\xi$, which has probability $1/3$. Thus it terminates the visits to the current record value with probability

$$
p=\frac12\frac13=\frac16.
$$

The [Strong Markov property](../../../../../../../strong-markov-property.md) at successive counted occurrences makes these trials independent. Therefore $G_m$ has the [geometric distribution](../../../../../../../geometric-distribution.md) on $\{1,2,\ldots\}$ with parameter $1/6$, and

$$
\boxed{\mathbb P(G_m\geq j)=\left(1-\frac16\right)^{j-1}}
$$

for every $j\geq1$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 220](../../../../paper-220-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
