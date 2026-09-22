<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [instrumental variable](../../../../../../instrumental-variable.md) graph is

$$
Z\longrightarrow A\longrightarrow Y,
\qquad
U\longrightarrow A,
\qquad
U\longrightarrow Y,
$$

with no arrow $Z\to Y$ and no common cause of $Z$ with $A$ or $Y$.

In [potential outcome](../../../../../../potential-outcome.md) notation, a valid instrument requires:

- [Instrumental-variable independence](../../../../../../instrumental-variable-independence.md): $Z\perp\{A(0),A(1),Y(0),Y(1)\}$, strengthened to all relevant joint potential outcomes as needed. Coin flipping makes the incentive assignment independent of quitting behavior and blood pressure under either assignment.
- [Exclusion restriction](../../../../../../exclusion-restriction.md): $Y(z,a)=Y(a)$. The incentive can affect blood pressure only by changing whether the subject quits, not through stress, income, or another direct route.
- [Instrument relevance](../../../../../../instrument-relevance.md): $\mathbb P\{A(1)\ne A(0)\}>0$, or at least $\mathbb E[A(1)-A(0)]\ne0$. The monetary incentive must change quitting probability.
- [Consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md) and no interference: observed quitting and blood pressure equal the potential values under the assigned encouragement and received exposure, and one subject's assignment does not affect another's outcome.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
