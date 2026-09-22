<h1 id="11i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X\in\{0,1\}$ denote whether $00$ or $11$ was sent, and write

$$
Y_j=X\mathbin\oplus E_j,
$$

where $E_1,E_2$ are independent Bernoulli variables of parameter $p$. Because $X$ is uniform, $Y_1$ is uniform, while $H(Y_1\mid X)=h_2(p)$. Thus the [mutual information](../../../../../../mutual-information.md) in the first received digit is

$$
\boxed{I(X;Y_1)=1-h_2(p)}.
$$

By the [chain rule for mutual information](../../../../../../chain-rule-for-mutual-information.md), the extra information in the second digit is $I(X;Y_2\mid Y_1)$. Conditional on $X$, the second channel error is independent of the first output, so

$$
H(Y_2\mid X,Y_1)=H(E_2)=h_2(p).
$$

Moreover,

$$
\mathbb P(Y_2\ne Y_1)
=\mathbb P(E_2\ne E_1)=2p(1-p).
$$

Given either value of $Y_1$, the second output therefore differs from it with probability $2p(1-p)$, and

$$
H(Y_2\mid Y_1)=h_2(2p(1-p)).
$$

Consequently the [incremental information in a twofold binary repetition code](../../../../../../incremental-information-in-a-twofold-binary-repetition-code.md) is

$$
\boxed{
I(X;Y_2\mid Y_1)
=h_2(2p(1-p))-h_2(p)
}
$$

bits.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11I](../../11i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
