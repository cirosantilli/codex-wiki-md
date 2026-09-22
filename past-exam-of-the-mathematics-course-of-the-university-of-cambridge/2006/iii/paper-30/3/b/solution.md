<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md) says that a memoryless channel permits transmission at any fixed [code rate](../../../../../../code-rate.md) $R<C$ with error probability tending to zero as block length tends to infinity. Conversely, a sequence of codes with error probability tending to zero cannot have a limiting rate above $C$. The [channel capacity](../../../../../../channel-capacity.md), in bits per use, is

$$
\boxed{C=\sup_{P_X}I(X;Y).}
$$

For a finite [discrete memoryless channel](../../../../../../discrete-memoryless-channel.md) with transition probabilities $W(y\mid x)$, the supremum is a maximum and its [mutual information](../../../../../../mutual-information.md) is

$$
I(X;Y)=\sum_{x,y}P_X(x)W(y\mid x)
\log_2\frac{W(y\mid x)}{\sum_{x'}P_X(x')W(y\mid x')}.
$$

For a general memoryless channel, [mutual information](../../../../../../mutual-information.md) is the [relative entropy](../../../../../../kullback-leibler-divergence.md) of the joint input-output law with respect to the product of its marginal laws; the same supremum is taken over the admissible input laws.

For the [binary symmetric channel](../../../../../../binary-symmetric-channel.md), write $Y=X\oplus Z$ with independent noise $Z$ having [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $p$. Given either input bit, the output [conditional entropy](../../../../../../conditional-entropy.md) is $h_2(p)$. Thus

$$
I(X;Y)=H(Y)-H(Y\mid X)=H(Y)-h_2(p)\leq1-h_2(p).
$$

An input with [uniform distribution](../../../../../../continuous-uniform-distribution.md) makes the output have [uniform distribution](../../../../../../continuous-uniform-distribution.md), attaining $H(Y)=1$. The [binary symmetric channel capacity](../../../../../../binary-symmetric-channel-capacity.md) is therefore

$$
\boxed{C_{\mathrm{BSC}}(p)=1-h_2(p)\ \text{bits per channel use}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
