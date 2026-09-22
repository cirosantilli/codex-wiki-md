# Independent revelation of a binary variable

↑ **Parent:** [Conditioning reduces entropy](conditioning-reduces-entropy.md)

Let $X$ be a [Bernoulli random variable](bernoulli-distribution.md) with $\Pr(X=1)=p$. Independently of $X$, a [Bernoulli random variable](bernoulli-distribution.md) $R$ with $\Pr(R=1)=r$ decides whether to reveal it:

$$
Y=\begin{cases}X,&R=1,\\\bot,&R=0.\end{cases}
$$

The symbol $\bot$ means “hidden” and is distinct from both binary states. This is a [binary erasure channel](binary-erasure-channel.md) with erasure [probability](probability.md) $1-r$. The hidden report leaves the [posterior distribution](bayesian-posterior.md) equal to the [prior distribution](prior-probability.md), because hiding is independent of the state. Either visible report determines $X$. Weighting these three reports gives the exact [conditional entropy](conditional-entropy.md) and [mutual information](mutual-information.md):

$$
H(X)=h_2(p),\qquad H(X\mid Y)=(1-r)h_2(p),\qquad I(X;Y)=rh_2(p).
$$

For $p=1/4$ and $r=1/2$, $H(X)=h_2(1/4)=2-(3/4)\log_2 3\approx0.811278$ [bits](bit.md), while $H(X\mid Y)=I(X;Y)\approx0.405639$ [bits](bit.md). With $r=0$ the report tells us nothing; with $r=1$ it reveals the state completely. If $0<p<1$, every positive reveal [probability](probability.md) makes the conditioning inequality strict. At $p=0$ or $p=1$, the state was already known and every value of $r$ gives equality.

<a id="image-independent-revelation-divides-binary-entropy-into-remaining-uncertainty-and-revealed-information"></a>
![](entropy-independent-binary-revelation.png)

**[Figure 3](#image-independent-revelation-divides-binary-entropy-into-remaining-uncertainty-and-revealed-information). Independent revelation divides binary entropy into remaining uncertainty and revealed information**.

For a [Bayesian inference](bayesian-statistics-split.md) problem, this model distinguishes an uninformative missing report from a decisive observed state. If hiding depended on $X$, even $Y=\bot$ could carry [mutual information](mutual-information.md), and the displayed calculation would change. In [lossless source coding](lossless-source-coding.md), suppose both [encoder](channel-encoder.md) and [decoder](channel-decoder.md) already know the reveal pattern for repeated [independent and identically distributed](independent-and-identically-distributed-random-variables.md) pairs. Only the hidden states require descriptions. Applying [Shannon's source coding theorem](shannon-s-source-coding-theorem.md) to those states gives an asymptotic average rate $(1-r)h_2(p)$ [bits](bit.md) per original state. A single hidden state need not have a [codeword](codeword.md) of that fractional length.

The reveal pattern itself has [information entropy](information-entropy-split.md) $H(R)=h_2(r)$. If that pattern must also be sent, the [chain rule for information entropy](chain-rule-for-information-entropy.md) gives $H(R,X)=h_2(r)+h_2(p)$, since $R$ and $X$ are [independent random variables](independent-random-variables.md). Equivalently, $H(Y)=h_2(r)+rh_2(p)$ and $H(X,Y)=H(Y)+H(X\mid Y)=h_2(r)+h_2(p)$. Thus a saving in the description of $X$ given $Y$ assumes that $Y$ is already available; it is not a free saving in the description of the whole pair.

## ↑ Ancestors (7)

1. [Conditioning reduces entropy](conditioning-reduces-entropy.md)
2. [Conditional entropy](conditional-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
