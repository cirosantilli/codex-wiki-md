<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce a selector $B$ with [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $\alpha$, and construct $W$ by taking its conditional law given $B=1$ to be $p_U$, and its conditional law given $B=0$ to be $p_V$. No prescribed joint law of $U,V$ is needed. Summing over the selector gives the desired mixture [probability mass function](../../../../../../probability-mass-function.md). The [conditional entropy](../../../../../../conditional-entropy.md) is

$$
H(W\mid B)=\alpha H(U)+(1-\alpha)H(V).
$$

Since conditioning cannot increase [information entropy](../../../../../../information-entropy.md),

$$
\boxed{H(W)\geq\alpha H(U)+(1-\alpha)H(V).}
$$

This proves the [concavity of information entropy](../../../../../../concavity-of-information-entropy.md). The argument also covers infinite [information entropies](../../../../../../information-entropy.md) with the convention that a zero mixing weight contributes zero. At $\alpha=0$ or $1$, the mixture is the corresponding original law and equality is immediate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
