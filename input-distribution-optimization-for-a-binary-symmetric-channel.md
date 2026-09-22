# Input distribution optimization for a binary symmetric channel

↑ **Parent:** [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)

Let $q=\Pr(X=1)$ for the input [bit](bit.md) of a [binary symmetric channel](binary-symmetric-channel.md) with crossover [probability](probability.md) $p$. The [law of total probability](law-of-total-probability.md) gives

$$
\Pr(Y=1)=(1-q)p+q(1-p)=p+(1-2p)q.
$$

Consequently its [mutual information](mutual-information.md) is

$$
I(X;Y)=h_2\!\left(p+(1-2p)q\right)-h_2(p).
$$

Here $p$ specifies the noise and $q$ specifies the input bias; they are different choices. At $p=0.1$ and $q=0.2$, the output has $\Pr(Y=1)=0.26$, giving $H(Y)\approx0.82674637$ and $I(X;Y)\approx0.35775078$ [bits](bit.md). With the same noise and the fair input $q=1/2$, the output becomes fair and $I(X;Y)\approx0.53100441$ [bits](bit.md), attaining [binary symmetric channel capacity](binary-symmetric-channel-capacity.md).

<a id="image-a-fair-input-maximizes-retained-information-through-a-binary-symmetric-channel"></a>
![](binary-channel-input-optimization.png)

**[Figure 19](#image-a-fair-input-maximizes-retained-information-through-a-binary-symmetric-channel). A fair input maximizes retained information through a binary symmetric channel**. The left panel holds the crossover [probability](probability.md) fixed and varies $q=\Pr(X=1)$. The right panel shows the output [probability distributions](probability-distribution.md) for $p=0.1$ with input biases $q=0.2$ and $q=0.5$. More output [Shannon entropy](information-entropy.md) helps here because the conditional noise [information entropy](information-entropy.md) stays fixed.

For $p\ne1/2$, [binary entropy](binary-entropy.md) reaches one only at output mass $1/2$, and the equation $p+(1-2p)q=1/2$ forces $q=1/2$. Thus the maximizing input is unique in those cases. For $p=1/2$, every input produces the same fair output and zero [mutual information](mutual-information.md), so every input bias is optimal and none transmits information. A fixed input $q=0$ or $q=1$ also carries zero [mutual information](mutual-information.md) for every $p$: noise can make its output unpredictable without creating an unknown message to recover.

## ↑ Ancestors (8)

1. [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
2. [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
3. [Channel capacity](channel-capacity.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Binary symmetric channel](binary-symmetric-channel.md)
