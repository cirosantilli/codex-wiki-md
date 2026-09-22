<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md) in its [channel capacity](../../../../../../channel-capacity.md) form $C=\max_{P_X}I(X;Y)$. The [finite-alphabet erasure channel](../../../../../../finite-alphabet-erasure-channel.md) erases independently of the input. On an unerased output Bob knows $X$ exactly; on the erasure output his posterior distribution is still $P_X$. Its classical [conditional entropy](../../../../../../conditional-entropy.md) is therefore

$$
H(X|Y)=fH(X),\qquad I(X;Y)=H(X)-H(X|Y)=(1-f)H(X).
$$

Equivalently, $H(Y)=h(f)+(1-f)H(X)$ and $H(Y|X)=h(f)$, so the [binary entropy](../../../../../../binary-entropy.md) terms cancel in the [mutual information](../../../../../../mutual-information.md).

For an alphabet of size $k$, [Shannon entropy](../../../../../../information-entropy.md) is at most $\log_2k$, with equality for the uniform distribution. Maximizing the displayed [mutual information](../../../../../../mutual-information.md) proves the [capacity of a finite-alphabet erasure channel](../../../../../../capacity-of-a-finite-alphabet-erasure-channel.md):

$$
\boxed{C=(1-f)\log_2k\quad\text{bits per channel use}.}
$$

This includes $f=0$, which transmits the whole symbol, and $f=1$, which transmits no information.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
