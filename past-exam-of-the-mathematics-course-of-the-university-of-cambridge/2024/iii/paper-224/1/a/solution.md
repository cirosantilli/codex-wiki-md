<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $X\to Y\to Z$ is a [Markov chain](../../../../../../markov-chain.md), the two forms of the [data processing inequality for mutual information](../../../../../../data-processing-inequality.md) are

$$
I(X;Z)\leq I(X;Y),
\qquad
I(X;Z)\leq I(Y;Z).
$$

The [chain rule for mutual information](../../../../../../chain-rule-for-mutual-information.md) and the Markov property $I(X;Z\mid Y)=0$ give

$$
I(X;Y,Z)=I(X;Y)+I(X;Z\mid Y)=I(X;Y).
$$

Using the other order,

$$
I(X;Y,Z)=I(X;Z)+I(X;Y\mid Z)\geq I(X;Z),
$$

because [conditional mutual information](../../../../../../conditional-mutual-information.md) is nonnegative. This proves the first inequality. Applying the same result to the reversed Markov chain $Z\to Y\to X$, which has the same conditional-independence statement, proves the second.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
