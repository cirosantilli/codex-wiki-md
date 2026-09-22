<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $X\to Y\to Z$ is a [Markov chain](../../../../../../markov-chain.md), so $I(X;Z\mid Y)=0$. The [chain rule for mutual information](../../../../../../chain-rule-for-mutual-information.md) gives

$$
I(X;Y,Z)=I(X;Y)+I(X;Z\mid Y)=I(X;Y)
$$

and also

$$
I(X;Y,Z)=I(X;Z)+I(X;Y\mid Z)\geq I(X;Z),
$$

because [conditional mutual information](../../../../../../conditional-mutual-information.md) is nonnegative. Therefore $I(X;Z)\leq I(X;Y)$. Similarly,

$$
I(X,Y;Z)=I(Y;Z)+I(X;Z\mid Y)=I(Y;Z)
$$

while $I(X,Y;Z)=I(X;Z)+I(Y;Z\mid X)\geq I(X;Z)$, so $I(X;Z)\leq I(Y;Z)$. These are the two [data processing inequalities](../../../../../../data-processing-inequality.md). In particular, applying any deterministic function or [Markov kernel](../../../../../../markov-kernel.md) to either argument cannot increase [mutual information](../../../../../../mutual-information.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
