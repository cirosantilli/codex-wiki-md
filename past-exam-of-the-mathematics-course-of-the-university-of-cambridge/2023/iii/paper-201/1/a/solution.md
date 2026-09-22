<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $M_n=\mathbb E[Z\mid\mathcal F_n]$. Each $M_n$ is $\mathcal F_n$-measurable and integrable, with $|M_n|\leq\mathbb E[|Z|\mid\mathcal F_n]\leq1$. Since a [filtration](../../../../../../filtration-probability-theory.md) is increasing, the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives

$$
\mathbb E[M_{n+1}\mid\mathcal F_n]
=\mathbb E[\mathbb E[Z\mid\mathcal F_{n+1}]\mid\mathcal F_n]
=\mathbb E[Z\mid\mathcal F_n]=M_n.
$$

**Thus $(M_n)$ is the [conditional-expectation martingale](../../../../../../conditional-expectation-martingale.md) associated with $Z$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
