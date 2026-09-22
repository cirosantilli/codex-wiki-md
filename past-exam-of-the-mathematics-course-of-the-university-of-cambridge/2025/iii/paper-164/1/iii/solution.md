<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Because $X,Y,Z$ are [independent random variables](../../../../../../independent-random-variables.md), adding $Y$ is an independent noise channel, so

$$
X\longrightarrow X+Z\longrightarrow X+Y+Z
$$

is a [Markov chain](../../../../../../markov-chain.md). The [data processing inequality for mutual information](../../../../../../data-processing-inequality.md) gives

$$
I(X;X+Y+Z)\leq I(X;X+Z).
$$

Translation in the [finite additive group](../../../../../../finite-additive-group.md) preserves [conditional entropy](../../../../../../conditional-entropy.md), and independence therefore gives

$$
I(X;X+Y+Z)=H(X+Y+Z)-H(Y+Z)
$$

and

$$
I(X;X+Z)=H(X+Z)-H(Z).
$$

Substitution proves the required [entropy submodularity for three independent sums](../../../../../../entropy-submodularity-for-three-independent-sums.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
