# Data processing inequality

↑ **Parent:** [Mutual information](mutual-information.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_processing_inequality)

For finite [discrete random variables](discrete-random-variable.md), suppose $X\to Y\to Z$ is a [Markov chain](markov-chain.md): the final [channel](communication-channel.md) uses only $Y$, so $X$ and $Z$ have [conditional independence](conditional-independence.md) given $Y$. In terms of the joint [probability mass function](probability-mass-function.md),

$$
p(x,y,z)=p_X(x)p(y\mid x)p(z\mid y),
$$

and hence $I(X;Z\mid Y)=0$. Then the two data processing inequalities are

$$
I(X;Z)\leq I(X;Y),
\qquad
I(X;Z)\leq I(Y;Z).
$$

All [mutual informations](mutual-information.md) here use base-two [logarithms](logarithm.md). Thus deterministic or randomized processing cannot increase the information shared with an unprocessed variable.[Stanford CS229T/STATS231, Theorem 2.1 and its chain-rule proof](https://web.stanford.edu/class/cs229t/scribe_notes/12_05_final.pdf)

For a concrete cascade, take a fair [bit](bit.md) $X$ and [Bernoulli random variables](bernoulli-distribution.md) $N_q,N_r$ with [probabilities](probability.md) $q=0.1$, $r=0.2$ of being one. Assume $X,N_q,N_r$ are jointly [independent random variables](independent-random-variables.md), and pass through two [binary symmetric channels](binary-symmetric-channel.md):

$$
Y=X\oplus N_q,\qquad Z=Y\oplus N_r.
$$

The second noise is independent of both $X$ and $Y$, so this is a [Markov chain](markov-chain.md). Both $Y$ and $Z$ are fair [bits](bit.md). The net [exclusive or](exclusive-or.md) error is one exactly when one noise flips the [bit](bit.md) and the other does not:

$$
s=\mathbb P(N_q\oplus N_r=1)
=q(1-r)+(1-q)r=q+r-2qr=0.26.
$$

Using the [binary entropy](binary-entropy.md) $h_2(t)=-t\log_2t-(1-t)\log_2(1-t)$, the three [mutual informations](mutual-information.md) are fully determined:

$$
\begin{aligned}
I(X;Y)&=1-h_2(0.1)\approx1-0.4689955936\approx0.5310044064,\\
I(Y;Z)&=1-h_2(0.2)\approx1-0.7219280949\approx0.2780719051,\\
I(X;Z)&=1-h_2(0.26)\approx1-0.8267463725\approx0.1732536275.
\end{aligned}
$$

All numbers are in [bits](bit.md). The two losses are $I(X;Y\mid Z)\approx0.3577507789$ and $I(Y;Z\mid X)\approx0.1048182776$. Thus the cascade retains less information about the original source than either individual [channel](communication-channel.md) shares between its own input and output.

<a id="image-two-noisy-binary-channels-compose-to-a-noisier-channel-and-obey-both-data-processing-bounds"></a>
![](data-processing-binary-cascade.png)

**[Figure 8](#image-two-noisy-binary-channels-compose-to-a-noisier-channel-and-obey-both-data-processing-bounds). Two noisy binary channels compose to a noisier channel and obey both data processing bounds**.

With $q=0.1$ fixed and $0\leq r\leq1/2$, the effective error is $s=0.1+0.8r$. At $r=0$, $Z=Y$ and $I(X;Z)=I(X;Y)$; at $r=1/2$, $Z$ is independent of the previous variables and $I(X;Z)=I(Y;Z)=0$. The diagram plots these endpoints and the computed $r=0.2$ example.

The [data processing inequality](data-processing-inequality.md) is useful for testing what a proposed decoder or data summary could possibly reveal: if its only input is $Y$, even randomized processing cannot provide more [mutual information](mutual-information.md) about $X$ than $Y$ already contains. The [Markov chain](markov-chain.md) hypothesis matters. In the [exclusive or](exclusive-or.md) example from [conditional mutual information](conditional-mutual-information.md), allowing a processor to use both $Y$ and $Z$ reveals $X$ exactly; that processor has additional input, so the conclusion for processing $Y$ alone does not apply.

The [chain rule for mutual information](chain-rule-for-mutual-information.md) proves both inequalities and identifies their exact gaps. First expand the information about $X$ in the two observation orders:

$$
\begin{aligned}
I(X;Y,Z)&=I(X;Y)+\underbrace{I(X;Z\mid Y)}_{0}\\
&=I(X;Z)+I(X;Y\mid Z).
\end{aligned}
$$

Therefore $I(X;Y)-I(X;Z)=I(X;Y\mid Z)\geq0$. Next use $Z$ as the variable being learned:

$$
\begin{aligned}
I(Z;X,Y)&=I(Z;Y)+\underbrace{I(Z;X\mid Y)}_{0}\\
&=I(Z;X)+I(Z;Y\mid X).
\end{aligned}
$$

Symmetry of [mutual information](mutual-information.md) gives $I(Y;Z)-I(X;Z)=I(Y;Z\mid X)\geq0$. Both signs follow from the nonnegativity of [conditional mutual information](conditional-mutual-information.md); the first gap also gives [equality in data processing inequality](equality-in-data-processing-inequality.md).

**Table of contents**

- [Equality in data processing inequality](equality-in-data-processing-inequality.md)
- [Conditional data-processing inequality](conditional-data-processing-inequality.md)

## ↑ Ancestors (6)

1. [Mutual information](mutual-information.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Chain rule for mutual information](chain-rule-for-mutual-information.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Data processing inequality](data-processing-inequality.md)
- [Equality in data processing inequality](equality-in-data-processing-inequality.md)
- [Shannon's rate-distortion theorem](shannon-s-rate-distortion-theorem.md)
