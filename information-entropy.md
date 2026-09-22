# Information entropy

↑ **Parent:** [Information theory](information-theory.md)

For a finite [discrete random variable](random-variable.md#discrete-random-variable) with [probability mass function](probability-distribution.md#probability-mass-function) $p$, its information entropy is the [expected value](expected-value.md) of its [information content](#information-content):

$$
H(X)=-\sum_{x:p(x)>0}p(x)\log_2p(x)
=\mathbb E[-\log_2p(X)].
$$

Base-two [logarithms](calculus.md#logarithm) give [bits](information-theory.md#bit); choosing a different base rescales the units. The convention $0\log_2 0=0$ is justified by a [limit](calculus.md#limit-of-a-function), so outcomes of zero [probability](probability-theory.md#probability) contribute nothing. The definition also applies to countable distributions, but the sum may be infinite.

A fair [bit](information-theory.md#bit) has $H=1$. A certain outcome has $H=0$. A [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) that is one with [probability](probability-theory.md#probability) $0.1$ has $H=h_2(0.1)\approx0.469$ [bits](information-theory.md#bit), because most of its outcomes are predictable. A rare outcome still has large [information content](#information-content): the outcome of [probability](probability-theory.md#probability) $0.1$ contributes $-\log_2(0.1)\approx3.322$ [bits](information-theory.md#bit) of surprise when it occurs. **Entropy is the average surprise, rather than the surprise of each outcome.**

For $m$ possible outcomes, $0\leq H(X)\leq\log_2m$, with the upper bound attained exactly by the [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution). The [Gibbs inequality](f-divergence.md#gibbs-inequality) proves this by comparing $p$ with the uniform distribution: $D(p\Vert u)=\log_2m-H(X)\geq0$. Thus increasing predictability reduces the required average description length. The four-symbol [prefix code](coding-theory.md#prefix-code) in [information theory](information-theory.md) attains $H=7/4$ [bits](information-theory.md#bit) exactly; for general probabilities, integer codeword lengths prevent such a perfect match for every individual symbol. [Shannon's source coding theorem](coding-theory.md#shannon-s-source-coding-theorem) explains how coding sufficiently long independent blocks approaches the entropy per symbol.

The [logarithm](calculus.md#logarithm) is especially natural because [independent](random-variable.md#independent-random-variables) outcomes have additive surprise: $-\log_2(pq)=-\log_2p-\log_2q$. Taking [expected values](expected-value.md) gives additive [information entropy](information-entropy.md) for [independent random variables](random-variable.md#independent-random-variables); for dependent ones, the [chain rule for information entropy](#chain-rule-for-information-entropy) replaces the second term by [conditional entropy](information-theory.md#conditional-entropy). This is why the same quantity can govern both a single observation and a long message.

**Table of contents**

- [Joint entropy](#joint-entropy)
- [Cross-entropy](#cross-entropy)
  - [Cross-entropy equals entropy plus relative entropy](#cross-entropy-equals-entropy-plus-relative-entropy)
  - [Mismatch penalty in lossless coding](#mismatch-penalty-in-lossless-coding)
  - [Binary cross-entropy](#binary-cross-entropy)
  - [Empirical cross-entropy](#empirical-cross-entropy)
    - [Cross-entropy and maximum likelihood](#cross-entropy-and-maximum-likelihood)
- [Entropy monotonicity under independent addition](#entropy-monotonicity-under-independent-addition)
- [Entropy function for a q-ary alphabet](#entropy-function-for-a-q-ary-alphabet)
- [Information content](#information-content)
- [Graph entropy](#graph-entropy)
- [Entropy bound with one prescribed probability](#entropy-bound-with-one-prescribed-probability)
- [Epsilon-sufficient set](#epsilon-sufficient-set)
  - [Minimum size of a sufficient set for an IID source](#minimum-size-of-a-sufficient-set-for-an-iid-source)
- [Differential entropy](#differential-entropy)
  - [Differential entropy of a uniform law](#differential-entropy-of-a-uniform-law)
  - [Differential entropy of a Gaussian law](#differential-entropy-of-a-gaussian-law)
  - [Differential entropy under an increasing transformation](#differential-entropy-under-an-increasing-transformation)
    - [Differential entropy of a squared uniform variable](#differential-entropy-of-a-squared-uniform-variable)
  - [Differential entropy under affine rescaling](#differential-entropy-under-affine-rescaling)
  - [Equal-width bin entropy](#equal-width-bin-entropy)
  - [Relative entropy and coordinate dependence](#relative-entropy-and-coordinate-dependence)
  - [Shannon's continuous-entropy coordinate convention](#shannon-s-continuous-entropy-coordinate-convention)
  - [Entropy power](#entropy-power)
    - [Entropy power inequality](#entropy-power-inequality)
      - [Multiplicative entropy power inequality](#multiplicative-entropy-power-inequality)
- [Min-entropy](#min-entropy)
  - [Information entropy dominates min-entropy](#information-entropy-dominates-min-entropy)
- [Varentropy](#varentropy)
- [Binary entropy](#binary-entropy)
- [Chain rule for information entropy](#chain-rule-for-information-entropy)
  - [Correlated binary variables](#correlated-binary-variables)
- [Subadditivity of information entropy](#subadditivity-of-information-entropy)
- [Concavity of information entropy](#concavity-of-information-entropy)
- [Maximum entropy distribution on a finite set](#maximum-entropy-distribution-on-a-finite-set)
  - [Maximum entropy distribution with a prescribed finite mean](#maximum-entropy-distribution-with-a-prescribed-finite-mean)
  - [Maximum entropy on a finite alphabet](#maximum-entropy-on-a-finite-alphabet)
- [Maximum entropy distribution on the nonnegative integers](#maximum-entropy-distribution-on-the-nonnegative-integers)

## Joint entropy

↑ **Parent:** [Information entropy](information-entropy.md)

[Joint entropy](#joint-entropy) is the [information entropy](information-entropy.md) of an entire [random vector](random-variable.md#random-vector), treating its coordinates together as one outcome. For [random variables](random-variable.md) with finite [alphabets](information-theory.md#alphabet) and joint [probability mass function](probability-distribution.md#probability-mass-function) $p$,

$$
H(X_1,\ldots,X_n)=-\sum_{x_1,\ldots,x_n:p(x_1,\ldots,x_n)>0}p(x_1,\ldots,x_n)\log_2 p(x_1,\ldots,x_n).
$$

It is measured in [bits](information-theory.md#bit). The distinction from separate [information entropies](information-entropy.md) is whether shared uncertainty is counted once or repeatedly. Two copies of the same fair [bit](information-theory.md#bit) have [joint entropy](#joint-entropy) one [bit](information-theory.md#bit), since only $00$ and $11$ can occur. Two [independent](random-variable.md#independent-random-variables) fair [bits](information-theory.md#bit) have [joint entropy](#joint-entropy) two [bits](information-theory.md#bit), since all four pairs are possible and equiprobable.

For a less symmetric example, assign [probabilities](probability-theory.md#probability) $1/2,1/4,1/4$ to $(X,Y)=(0,0),(1,0),(1,1)$ respectively. Then

$$
\boxed{H(X,Y)=\tfrac12\cdot1+\tfrac14\cdot2+\tfrac14\cdot2=\tfrac32\text{ bits}.}
$$

Here $X$ is fair, while $\mathbb P(Y=1)=1/4$. Thus $H(X)=1$ and $H(Y)=h_2(1/4)\approx0.811278$ [bits](information-theory.md#bit), where $h_2$ is [binary entropy](#binary-entropy). Adding the separate [information entropies](information-entropy.md) would give approximately $1.811278$ [bits](information-theory.md#bit), overcounting by the [mutual information](information-theory.md#mutual-information) $I(X;Y)\approx0.311278$ [bits](information-theory.md#bit).

The [chain rule for information entropy](#chain-rule-for-information-entropy) makes the shared information explicit:

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

In this example $Y$ is certain given $X=0$ and fair given $X=1$, so its average [conditional entropy](information-theory.md#conditional-entropy) is $H(Y\mid X)=\tfrac12\cdot0+\tfrac12\cdot1=1/2$ [bit](information-theory.md#bit). Sending the first coordinate changes how much uncertainty remains in the second. A [prefix code](coding-theory.md#prefix-code) with codewords `0`, `10`, `11` for the three possible pairs has average length $3/2$ [bits](information-theory.md#bit), exactly the [joint entropy](#joint-entropy) in this stipulated law.

For finite [alphabets](information-theory.md#alphabet),

$$
\max_iH(X_i)\leq H(X_1,\ldots,X_n)\leq\sum_iH(X_i).
$$

The lower bound follows because knowing the full [random vector](random-variable.md#random-vector) determines every coordinate; the upper bound follows from [conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy) in the [chain rule for information entropy](#chain-rule-for-information-entropy). Equality in the upper bound means joint [independence](random-variable.md#independent-random-variables). The difference from that upper bound is [total correlation](information-theory.md#total-correlation), whose [noisy parity total correlation](information-theory.md#noisy-parity-total-correlation) example shows why separate pairwise comparisons need not find all the dependence.

## Cross-entropy

↑ **Parent:** [Information entropy](information-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-entropy)

[Cross-entropy](#cross-entropy) measures the average [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss) incurred when outcomes follow one [probability distribution](probability-distribution.md) $P$, but a model assigns [probabilities](probability-theory.md#probability) using another [probability distribution](probability-distribution.md) $Q$. For a finite [alphabet](information-theory.md#alphabet), write their [probability mass functions](probability-distribution.md#probability-mass-function) as $p_i$ and $q_i$. With base-two [logarithms](calculus.md#logarithm),

$$
H(P,Q)=-\sum_{i:p_i>0}p_i\log_2 q_i=\mathbb E_P[-\log_2 q(X)].
$$

The expectation is under the true or stipulated source law $P$, rather than the model $Q$. Terms with $p_i=0$ contribute nothing. If $p_i>0$ but $q_i=0$ for any outcome, the [cross-entropy](#cross-entropy) is $+\infty$: the model rules out an event that can occur. The result is measured in [bits](information-theory.md#bit); [natural logarithms](calculus.md#natural-logarithm) give [nats](information-theory.md#nat-unit).

The useful identity is [cross-entropy equals entropy plus relative entropy](#cross-entropy-equals-entropy-plus-relative-entropy):

$$
\boxed{H(P,Q)=H(P)+D_{\mathrm{KL}}(P\Vert Q).}
$$

The source's [information entropy](information-entropy.md) $H(P)$ is the baseline uncertainty. The [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) is the extra average cost of a mismatched model, with the true law first and model second. Thus optimizing $Q$ for a fixed $P$ reduces the mismatch, rather than changing the source's own uncertainty. For finite [alphabets](information-theory.md#alphabet), the minimum is $H(P)$, attained exactly at $Q=P$.

Take a three-symbol source with $P=(1/2,1/4,1/4)$. A matched binary [prefix code](coding-theory.md#prefix-code) assigns $A\mapsto0$, $B\mapsto10$, $C\mapsto11$, with lengths $(1,2,2)$. A mismatched [prefix code](coding-theory.md#prefix-code) instead assigns $A\mapsto10$, $B\mapsto11$, $C\mapsto0$, with lengths $(2,2,1)$, corresponding to $Q=(1/4,1/4,1/2)$. Both [prefix codes](coding-theory.md#prefix-code) decode exactly, but the most common symbol is shorter in the matched code. Under the same source $P$,

$$
\begin{aligned}
H(P)&=\tfrac12\cdot1+\tfrac14\cdot2+\tfrac14\cdot2=\tfrac32,\\
H(P,Q)&=\tfrac12\cdot2+\tfrac14\cdot2+\tfrac14\cdot1=\tfrac74,\\
D_{\mathrm{KL}}(P\Vert Q)&=\tfrac12\log_2 2+\tfrac14\log_2 1+\tfrac14\log_2(1/2)=\tfrac14.
\end{aligned}
$$

**The mismatched code costs an extra (1/4) bit per source symbol on average.** No information is lost; the penalty is inefficient representation of this source. The [mismatch penalty in lossless coding](#mismatch-penalty-in-lossless-coding) explains when this coding interpretation is exact.

<a id="image-two-lossless-prefix-codes-have-different-average-lengths-for-the-same-source"></a>
![](cross-entropy-mismatched-prefix-codes.png)

**[Figure 1](#image-two-lossless-prefix-codes-have-different-average-lengths-for-the-same-source). Two lossless prefix codes have different average lengths for the same source**. Both sets of [codewords](coding-theory.md#codeword) are [prefix codes](coding-theory.md#prefix-code). The source [probabilities](probability-theory.md#probability) are fixed at $(1/2,1/4,1/4)$. Each colored contribution is source [probability](probability-theory.md#probability) times [codeword length](coding-theory.md#codeword-length); changing which symbol receives the shortest word increases the total from $3/2$ to $7/4$ [bits](information-theory.md#bit) per source symbol.

[Cross-entropy](#cross-entropy) is also useful when evaluating a [predictive distribution](probability-distribution.md#predictive-distribution). A report that places tiny [probability](probability-theory.md#probability) on the realized outcome receives a large [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss), even when it usually predicts the most common outcome correctly. The loss convention is the negative of the reward convention in the [logarithmic scoring rule](statistical-inference.md#logarithmic-scoring-rule). Its expected loss is uniquely minimized by the correct [probability distribution](probability-distribution.md), making it a [strictly proper scoring rule](statistical-inference.md#strictly-proper-scoring-rule). [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others) treats this connection in §3.1, Example 3; its discussion uses rewards, so the signs are reversed for the losses here.[Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others)

[I. J. Good](mathematics-author.md#i-j-good)'s [Rational Decisions by I. J. Good](mathematics-bibliography.md#rational-decisions-by-i-j-good) appeared in 1952. Its published summary describes a method for encouraging accurate [probability](probability-theory.md#probability) estimates and a connection with [information theory](information-theory.md). [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others) traces the [logarithmic scoring rule](statistical-inference.md#logarithmic-scoring-rule) at least as far back as this 1952 paper.[Rational Decisions by I. J. Good](mathematics-bibliography.md#rational-decisions-by-i-j-good)

### Cross-entropy equals entropy plus relative entropy

↑ **Parent:** [Cross-entropy](#cross-entropy)

For finite [probability mass functions](probability-distribution.md#probability-mass-function), with $q_i>0$ whenever $p_i>0$, subtract the two [expectations](expected-value.md) of [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss):

$$
\begin{aligned}
H(P,Q)-H(P)
&=\sum_{i:p_i>0}p_i(\log_2 p_i-\log_2 q_i)\\
&=\sum_{i:p_i>0}p_i\log_2\frac{p_i}{q_i}
=D_{\mathrm{KL}}(P\Vert Q).
\end{aligned}
$$

The [Gibbs inequality](f-divergence.md#gibbs-inequality) makes the difference nonnegative and zero exactly when $P=Q$. If $Q$ assigns zero [probability](probability-theory.md#probability) to an outcome with positive [probability](probability-theory.md#probability) under $P$, both the [cross-entropy](#cross-entropy) and the [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) are infinite. The finite [information entropy](information-entropy.md) still leaves the displayed identity valid in the extended sense. In more general settings, undefined differences such as $\infty-\infty$ cannot be used as a derivation.

### Mismatch penalty in lossless coding

↑ **Parent:** [Cross-entropy](#cross-entropy)

Suppose a binary [prefix code](coding-theory.md#prefix-code) has integer [codeword lengths](coding-theory.md#codeword-length) $\ell_i=-\log_2 q_i$. Under a source with [probability mass function](probability-distribution.md#probability-mass-function) $p_i$, its average [codeword length](coding-theory.md#codeword-length) is exactly [cross-entropy](#cross-entropy), $\sum_i p_i\ell_i=H(P,Q)$. The [Kraft inequality](coding-theory.md#kraft-mcmillan-inequality) is satisfied because $\sum_i2^{-\ell_i}=\sum_iq_i=1$. This exact interpretation requires suitable [dyadic rational](arithmetic.md#dyadic-rational) [probabilities](probability-theory.md#probability); a general $-\log_2q_i$ is not an integer [codeword length](coding-theory.md#codeword-length). For positive $q_i$, a [prefix code](coding-theory.md#prefix-code) with lengths $\lceil-\log_2q_i\rceil$ exists by the [Kraft inequality](coding-theory.md#kraft-mcmillan-inequality) and has average length between $H(P,Q)$ and $H(P,Q)+1$. The [ceiling function](calculus.md#ceiling-function) causes the one-symbol rounding overhead. The cross-entropy term describes mismatch overhead; those are distinct costs.

### Binary cross-entropy

↑ **Parent:** [Cross-entropy](#cross-entropy)

Let $Y$ follow a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) with true event [probability](probability-theory.md#probability) $r$, and let the model report event [probability](probability-theory.md#probability) $q$. The [binary cross-entropy](#binary-cross-entropy) is its expected [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss):

$$
H(r,q)=-r\log_2q-(1-r)\log_2(1-q).
$$

For $0<r<1$, it is minimized at $q=r$, where the value is [binary entropy](#binary-entropy) $h_2(r)$. An individual outcome has loss $-\log_2q$ when $Y=1$ and $-\log_2(1-q)$ when $Y=0$; the [binary cross-entropy](#binary-cross-entropy) averages those two cases using the true [probabilities](probability-theory.md#probability).

For $r=1/4$, truthful reporting gives $h_2(1/4)\approx0.811278$ [bits](information-theory.md#bit). Reporting $q=1/2$ gives one [bit](information-theory.md#bit). Reporting $q=0.01$ gives

$$
H(1/4,0.01)=\tfrac14\log_2 100-\tfrac34\log_2 0.99\approx1.671839\text{ bits}.
$$

Both $q=1/4$ and $q=0.01$ select zero if one predicts only the more likely binary outcome. Their predicted [probabilities](probability-theory.md#probability) are very different, however, and [cross-entropy](#cross-entropy) reveals the cost of underestimating the event that occurs a quarter of the time. Endpoint losses are computed using the realized outcome rather than multiplying zero by an undefined [logarithm](calculus.md#logarithm).

<a id="image-the-expected-logarithmic-loss-is-minimized-by-reporting-the-true-event-probability"></a>
![](binary-cross-entropy-forecast-loss.png)

**[Figure 2](#image-the-expected-logarithmic-loss-is-minimized-by-reporting-the-true-event-probability). The expected logarithmic loss is minimized by reporting the true event probability**. The true [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) has parameter $r=1/4$. The blue curve averages the orange event loss and gray nonevent loss with weights $1/4$ and $3/4$. Its minimum is at $q=r$, while both endpoint limits diverge because both outcomes have positive [probability](probability-theory.md#probability). These are calculated expectations, rather than measurements.

### Empirical cross-entropy

↑ **Parent:** [Cross-entropy](#cross-entropy)

For observations $X_1,\ldots,X_n$ of a [categorical variable](statistical-modelling.md#categorical-variable), [empirical cross-entropy](#empirical-cross-entropy) is the average [logarithmic loss](foundations-of-mathematics.md#logarithmic-loss) under the reported [probability mass function](probability-distribution.md#probability-mass-function) $q$. Writing the [empirical distribution](information-theory.md#type-information-theory) as $\hat p_i=n^{-1}\#\{t:X_t=i\}$ gives

$$
\widehat H_n(Q)=-\frac1n\sum_{t=1}^n\log_2q(X_t)
=-\sum_{i:\hat p_i>0}\hat p_i\log_2q_i=H(\widehat P_n,Q).
$$

Under [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) observations from $P$ and a fixed model with positive [probability](probability-theory.md#probability) for each possible outcome, the [law of large numbers](convergence-of-random-variables.md#law-of-large-numbers) gives convergence to $H(P,Q)$. A finite [empirical distribution](information-theory.md#type-information-theory) is an estimate of $P$, rather than the true source law; unobserved outcomes need not be impossible. If the same data are used to choose $Q$, evaluating the resulting [empirical cross-entropy](#empirical-cross-entropy) on that data need not estimate its prediction performance on fresh observations without [bias](statistical-modelling.md#bias-of-an-estimator).

#### Cross-entropy and maximum likelihood

↑ **Parent:** [Empirical cross-entropy](#empirical-cross-entropy)

For a [parametric statistical model](statistical-model.md#parametric-statistical-model) with [probability mass function](probability-distribution.md#probability-mass-function) $q_\theta$ and an [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) model, minimizing [empirical cross-entropy](#empirical-cross-entropy) is [maximum likelihood estimation](maximum-likelihood-estimation.md). The [logarithm](calculus.md#logarithm) is strictly increasing, so maximizing $\prod_tq_\theta(X_t)$ is equivalent to maximizing $\sum_t\log_2q_\theta(X_t)$. Negating and dividing by $n$ gives the displayed minimization. Restricting the model family can prevent the optimum from matching the [empirical distribution](information-theory.md#type-information-theory), and a finite optimizing parameter need not exist. This algebra does not by itself establish accuracy on new data.[§1, printed p. 360: optimum-score estimation and maximum likelihood](mathematics-bibliography.md#strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others)

## Entropy monotonicity under independent addition

↑ **Parent:** [Information entropy](information-entropy.md)

If $U,V$ are [independent random variables](random-variable.md#independent-random-variables) taking values in a countable additive group, conditioning on $V$ makes $U+V$ a translate of $U$. Consequently $H(U+V\mid V)=H(U)$, and [conditional entropy](information-theory.md#conditional-entropy) gives $H(U+V)\geq H(U)$. If the two [information entropies](information-entropy.md) are finite, equality holds exactly when $U+V$ and $V$ are independent.

// Target: probability-and-statistics.bigb

## Entropy function for a q-ary alphabet

↑ **Parent:** [Information entropy](information-entropy.md)

This is the entropy in base $q$ of the distribution with one symbol of probability $1-x$ and each of the other $q-1$ symbols of probability $x/(q-1)$. It increases on $[0,1-1/q]$ from zero to one, and governs the exponential volume of a [Hamming ball](coding-theory.md#hamming-ball). For $q=2$ it is the [binary entropy](#binary-entropy) function.

// Target: algebra.bigb

## Information content

↑ **Parent:** [Information entropy](information-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Information_content)

The self-information of a positive-probability outcome is the negative logarithm of its probability. Independent outcomes have additive self-information. Its expectation is [Shannon entropy](information-entropy.md).

// Target: probability-and-statistics.bigb

## Graph entropy

↑ **Parent:** [Information entropy](information-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_entropy)

For a vertex law $P$ on a graph, choose $X\sim P$ and an [independent set](graph-theory.md#independent-set-graph-theory) valued random variable $Y$ containing $X$ almost surely. Minimize their [mutual information](information-theory.md#mutual-information) over all such joint laws. This defines graph entropy. It differs from the entropy of a proper coloring, because the random independent set need not be a deterministic color class.

## Entropy bound with one prescribed probability

↑ **Parent:** [Information entropy](information-entropy.md)

If one probability in a $k$-point distribution equals $t$, normalize the remaining $k-1$ probabilities to $q$. Then $H=h(t)+(1-t)H(q)\leq h(t)+(1-t)\log_2(k-1)$. Equality for $t<1$ means that the remaining probabilities are equal. This combines the [binary entropy](#binary-entropy) of the distinguished event with the largest residual [Shannon entropy](information-entropy.md).

## Epsilon-sufficient set

↑ **Parent:** [Information entropy](information-entropy.md)

For a finite-valued [random variable](random-variable.md), an epsilon-sufficient set $S$ retains probability at least $1-\epsilon$. This notion is about covering probability mass and is unrelated to a [sufficient statistic](probability-and-statistics.md#sufficient-statistic). For an [IID random variable](random-variable.md#independent-and-identically-distributed-random-variables) source, any such set of words with fixed $\epsilon<1$ requires exponentially many words at a rate approaching the [Shannon entropy](information-entropy.md).

### Minimum size of a sufficient set for an IID source

↑ **Parent:** [Epsilon-sufficient set](#epsilon-sufficient-set)

For finite-alphabet [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), fixed $0\leq\epsilon<1$ and $\delta>0$, every [epsilon-sufficient set](#epsilon-sufficient-set) $S_n$ of length-$n$ words satisfies $|S_n|\geq(1-\epsilon)2^{n(H-\delta)}/2$ for sufficiently large $n$. Intersect $S_n$ with a [typical set](information-theory.md#typical-set) whose excluded mass is at most $(1-\epsilon)/2$. The intersection retains that much probability and each word has probability at most $2^{-n(H-\delta)}$.

## Differential entropy

↑ **Parent:** [Information entropy](information-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_entropy)

[Differential entropy](#differential-entropy) describes the spread of a continuous [probability distribution](probability-distribution.md) relative to the volume scale of its coordinates. For a real [random variable](random-variable.md) $X$ with [probability density function](continuous-probability-distribution.md#probability-density-function) $f$, use [natural logarithms](calculus.md#natural-logarithm) and write

$$
\boxed{h_e(X)=-\int_{\mathbb R} f(x)\ln f(x)\,dx=-\mathbb E[\ln f(X)].}
$$

The convention is $0\ln0=0$. For a finite value, require $\int f|\ln f|<\infty$; if both positive and negative contributions are infinite, the expression is undefined. Unlike a [probability](probability-theory.md#probability), a [probability density](wave-function.md#probability-density) can exceed one. Consequently [differential entropy](#differential-entropy) can be negative. Base-two [logarithms](calculus.md#logarithm) give $h_2=h_e/\ln2$, in [bits](information-theory.md#bit) instead of [nats](information-theory.md#nat-unit).[§1.3, Definition 1.5, equation (1.19) and warning, printed p. 18](mathematics-bibliography.md#6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-1-information-measures-entropy-and-divergence)

This quantity does not give the exact number of [bits](information-theory.md#bit) needed to store a real number. A recording device supplies a resolution; [equal-width bin entropy](#equal-width-bin-entropy) connects that resolution to discrete [information entropy](information-entropy.md). The useful continuous quantity is what remains after removing the increasing cost of specifying finer bins. Its dependence on coordinates is visible already in [differential entropy of a uniform law](#differential-entropy-of-a-uniform-law).

### Differential entropy of a uniform law

↑ **Parent:** [Differential entropy](#differential-entropy)

For a [continuous uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on an interval of length $L>0$, the [probability density](wave-function.md#probability-density) is $1/L$. Direct integration gives

$$
h_e(X)=-\int_a^{a+L}\frac1L\ln\frac1L\,dx=\ln L.
$$

Thus **a uniform law on an interval of length $1/2$ has differential entropy $-\ln2$**, while length two gives $\ln2$. Both laws have total [probability](probability-theory.md#probability) one. The shorter interval has larger [probability density](wave-function.md#probability-density), making $-\ln f(X)$ negative; this is neither a negative [probability](probability-theory.md#probability) nor a negative discrete [information entropy](information-entropy.md).

<a id="image-uniform-densities-can-have-negative-or-positive-differential-entropy"></a>
![](differential-entropy-uniform-density-and-scale.png)

**[Figure 3](#image-uniform-densities-can-have-negative-or-positive-differential-entropy). Uniform densities can have negative or positive differential entropy**. The two stipulated [continuous uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution) have density two on an interval of length $1/2$ and density $1/2$ on an interval of length two. Each rectangle has area one. The reported [differential entropy](#differential-entropy) is in [nats](information-theory.md#nat-unit), using the displayed numerical coordinates.

### Differential entropy of a Gaussian law

↑ **Parent:** [Differential entropy](#differential-entropy)

For a [normal distribution](probability-distribution.md#normal-distribution) with [mean](expected-value.md) $m$ and positive [variance](variance.md) $\sigma^2$, expand the [logarithm](calculus.md#logarithm) of its [probability density function](continuous-probability-distribution.md#probability-density-function):

$$
-\ln f(X)=\frac12\ln(2\pi\sigma^2)+\frac{(X-m)^2}{2\sigma^2}.
$$

The second term has [expected value](expected-value.md) $1/2$, hence $h_e(X)=\tfrac12\ln(2\pi e\sigma^2)$. Translation of the [mean](expected-value.md) has no effect, while shrinking the [standard deviation](variance.md#standard-deviation) lowers [differential entropy](#differential-entropy). A [standard normal distribution](probability-distribution.md#standard-normal-distribution) has approximately $1.41894$ [nats](information-theory.md#nat-unit). This connects the continuous spread calculation with [entropy power](#entropy-power), whose normalization matches a [Gaussian distribution](probability-distribution.md#normal-distribution)'s [variance](variance.md).

### Differential entropy under an increasing transformation

↑ **Parent:** [Differential entropy](#differential-entropy)

Let $X$ have a [probability density function](continuous-probability-distribution.md#probability-density-function) on an open interval, and let $g$ be continuously [differentiable](analysis.md#differentiable-function), strictly increasing there, with $g'(x)>0$. The [change of variables formula](multivariable-calculus.md#change-of-variables-formula) gives

$$
f_{g(X)}(g(x))=\frac{f_X(x)}{g'(x)}.
$$

If the [differential entropy](#differential-entropy) and the expected absolute [logarithm](calculus.md#logarithm) of $g'(X)$ are finite, taking the [expectation](expected-value.md) of the negative [logarithm](calculus.md#logarithm) proves the displayed formula, for a fixed base $b>1$. Local stretching reduces [probability density](wave-function.md#probability-density); its contribution to [differential entropy](#differential-entropy) is the expected logarithmic stretch. The map is invertible, so this change does not mean that the transformation destroyed information about $X$.

#### Differential entropy of a squared uniform variable

↑ **Parent:** [Differential entropy under an increasing transformation](#differential-entropy-under-an-increasing-transformation)

Take $X$ with [continuous uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$ and set $Y=X^2$. This is an increasing invertible transformation on that interval. Its [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) is $F_Y(y)=\sqrt y$, giving

$$
f_Y(y)=\frac1{2\sqrt y},\qquad 0<y<1.
$$

Although the [probability density](wave-function.md#probability-density) diverges near zero, it is [integrable](measure-theory.md#integrability). The logarithmic stretch is integrable too:

$$
h_e(Y)=h_e(X)+\int_0^1\ln(2x)\,dx
=\boxed{\ln2-1\approx-0.306853\text{ nats}.}
$$

The [inverse function](function.md#inverse-function) $X=\sqrt Y$ recovers every input in the interval. The changed [differential entropy](#differential-entropy) records a changed coordinate volume, rather than a failure of recovery.

// Target: probability-and-statistics.bigb

### Differential entropy under affine rescaling

↑ **Parent:** [Differential entropy](#differential-entropy)

For real $a\ne0$ and $b$, the [change of variables formula](multivariable-calculus.md#change-of-variables-formula) gives $f_{aX+b}(ax+b)=f_X(x)/|a|$. Therefore

$$
\boxed{h_e(aX+b)=h_e(X)+\ln|a|.}
$$

The absolute value also covers a decreasing transformation. If a numerical length changes from metres to centimetres, $a=100$ and the [differential entropy](#differential-entropy) changes by $\ln100\approx4.60517$ [nats](information-theory.md#nat-unit), although the physical uncertainty is the same. The reference coordinate scale must therefore accompany an absolute [differential entropy](#differential-entropy) value.

### Equal-width bin entropy

↑ **Parent:** [Differential entropy](#differential-entropy)

Partition $(0,1)$ into $n$ bins of width $\delta=1/n$, and let the [discrete random variable](random-variable.md#discrete-random-variable) $Q_n$ record the bin containing $X$. This is a [quantization](computer-science.md#quantization-signal-processing) of $X$. Its [probability mass function](probability-distribution.md#probability-mass-function) is

$$
p_j=\int_{j/n}^{(j+1)/n}f(x)\,dx,\qquad 0\leq j<n,
$$

and its discrete [information entropy](information-entropy.md) is $H_e(Q_n)=-\sum_jp_j\ln p_j$. Let $\bar f_j=p_j/\delta$ be the average [probability density](wave-function.md#probability-density) within bin $j$. Rearrangement gives the exact finite-bin identity

$$
H_e(Q_n)+\ln\delta=-\sum_j\delta\bar f_j\ln\bar f_j.
$$

For a [continuous](calculus.md#continuous-function) [probability density](wave-function.md#probability-density) on $[0,1]$, [uniform continuity](topological-analysis.md#uniform-continuity) makes the bin averages converge uniformly to the density. Since $t\ln t$ is [continuous](calculus.md#continuous-function) at zero with the stated convention, the right-hand side converges to $h_e(X)$. Thus the increasing resolution cost is $\ln n$; [differential entropy](#differential-entropy) is the remaining offset, rather than the entire discrete encoding cost.

For a [continuous uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution), every bin has [probability](probability-theory.md#probability) $1/n$, and $H_e(Q_n)=\ln n$ exactly. For the [continuous uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution)'s squared transformation above, the exact bin probabilities are

$$
p_j=\sqrt{\frac{j+1}{n}}-\sqrt{\frac jn}.
$$

The diagram computes these masses directly, including the bin next to the integrable singularity. It compares their corrected [information entropy](information-entropy.md) with the analytic [differential entropy](#differential-entropy) $\ln2-1$.

<a id="image-removing-the-bin-resolution-cost-reveals-differential-entropy"></a>
![](differential-entropy-fine-bin-resolution.png)

**[Figure 4](#image-removing-the-bin-resolution-cost-reveals-differential-entropy). Removing the bin-resolution cost reveals differential entropy**. The left plot shows discrete [information entropy](information-entropy.md) increasing with the number of equal-width bins. The right subtracts $\ln n$ and compares with the exact [differential entropy](#differential-entropy) of a uniform input and its squared transformation. Every plotted point comes from the stated exact [probability mass functions](probability-distribution.md#probability-mass-function); no observations are fitted.

### Relative entropy and coordinate dependence

↑ **Parent:** [Differential entropy](#differential-entropy)

Apply the same invertible differentiable transformation to two [probability distributions](probability-distribution.md) with densities $f$ and $r$. Both transformed densities acquire the same [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) factor. Write their transformed densities as $f_g$ and $r_g$. Their ratio is unchanged, and the integration measure transforms with the numerator density. Consequently their [relative entropy](f-divergence.md#kullback-leibler-divergence) is unchanged:

$$
D(f_g\Vert r_g)=D(f\Vert r).
$$

The densities describe two alternative laws in the same coordinate, with a nonzero [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) on their common domain, and the expression is assumed well defined. This explains why comparing two laws can survive a change of measurement units even though either law's [differential entropy](#differential-entropy) changes. [Mutual information](information-theory.md#mutual-information), formulated as [relative entropy](f-divergence.md#kullback-leibler-divergence) from a product of marginals, has the same invariance under invertible changes to either observed coordinate.

[Differential entropy](#differential-entropy) is also the entropy term in the [evidence lower bound](bayesian-statistics.md#evidence-lower-bound) for continuous [variational inference](bayesian-statistics.md#variational-inference). Its coordinate dependence must be combined consistently with that of the model density; changing units does not justify changing only one term of the objective.

<h3 id="shannon-s-continuous-entropy-coordinate-convention">Shannon's continuous-entropy coordinate convention</h3>

↑ **Parent:** [Differential entropy](#differential-entropy)

In [A Mathematical Theory of Communication by Claude Shannon](mathematics-bibliography.md#a-mathematical-theory-of-communication-by-claude-shannon) (1948), section 20 extends the discrete entropy formula to continuous densities. Properties 8–9 explicitly discuss coordinate dependence, possible negative values and linear rescaling. [Claude Shannon](mathematics-author.md#claude-shannon) relates this coordinate convention to the engineering use of entropy differences, rather than treating an isolated continuous entropy as an invariant count of messages.[section 20, definition and properties 8–9, reprint pp. 35 and 37–38](mathematics-bibliography.md#a-mathematical-theory-of-communication-by-claude-shannon)

### Entropy power

↑ **Parent:** [Differential entropy](#differential-entropy)

The [entropy power](#entropy-power) of an $n$-dimensional [random vector](random-variable.md#random-vector) with finite [differential entropy](#differential-entropy) in bits is the [variance](variance.md) per coordinate of an isotropic [Gaussian distribution](probability-distribution.md#normal-distribution) with the same [differential entropy](#differential-entropy). The normalization makes $N(X)=\sigma^2$ when $X$ has [covariance matrix](variance.md#covariance-matrix) $\sigma^2I_n$.

// Target: probability-and-statistics.bigb

#### Entropy power inequality

↑ **Parent:** [Entropy power](#entropy-power)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_power_inequality)

For independent $n$-dimensional [random vectors](random-variable.md#random-vector) with densities and finite [differential entropies](#differential-entropy), the [entropy power inequality](#entropy-power-inequality) states

$$
2^{2h(X+Y)/n}\geq2^{2h(X)/n}+2^{2h(Y)/n}.
$$

The sum's [differential entropy](#differential-entropy) is required to be defined; a value $+\infty$ makes the inequality immediate. Equality for finite nondegenerate densities occurs for [Gaussian distributions](probability-distribution.md#normal-distribution) with proportional [covariance matrices](variance.md#covariance-matrix).

// Target: probability-and-statistics.bigb

##### Multiplicative entropy power inequality

↑ **Parent:** [Entropy power inequality](#entropy-power-inequality)

For independent positive [random variables](random-variable.md) $Y_1,Y_2$ with densities, finite [differential entropies](#differential-entropy) and finite $\mu_i=\mathbb E\log_2Y_i$, applying the [entropy power inequality](#entropy-power-inequality) to $Z_i=\ln Y_i$ gives

$$
2^{2h(Y_1Y_2)}\geq2^{2\mu_2}2^{2h(Y_1)}+2^{2\mu_1}2^{2h(Y_2)}.
$$

Indeed $h(Z_i)=h(Y_i)-\mu_i$, while $h(Y_1Y_2)=h(Z_1+Z_2)+\mu_1+\mu_2$, provided the sum's [differential entropy](#differential-entropy) is defined. Positivity alone does not ensure these expressions exist: $Y=e^T$ with $T$ having [Cauchy distribution](probability-distribution.md#cauchy-distribution) has undefined $\mathbb E\log_2Y$.

// Target: algebra.bigb

## Min-entropy

↑ **Parent:** [Information entropy](information-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Min-entropy)

For a [discrete random variable](random-variable.md#discrete-random-variable) $X$ with a finite or countable [alphabet](information-theory.md#alphabet) and [probability mass function](probability-distribution.md#probability-mass-function) $p_x=\mathbb P(X=x)$, define $p_{\max}=\max_xp_x$. Its [min-entropy](#min-entropy), using base-two [logarithms](calculus.md#logarithm), is

$$
H_\infty(X)=-\log_2p_{\max}
=\min_{x:p_x>0}(-\log_2p_x).
$$

The unit is the [bit](information-theory.md#bit). This is the smallest [information content](#information-content) of any possible outcome: it records the easiest outcome to predict, whereas [Shannon entropy](information-entropy.md) averages [information content](#information-content) over all outcomes. A normalized countable [probability mass function](probability-distribution.md#probability-mass-function) has an attained positive maximum, so $H_\infty(X)$ is finite even when [Shannon entropy](information-entropy.md) is infinite. Outcomes of zero [probability](probability-theory.md#probability) cannot minimize the surprise and are omitted from the minimum; including extra impossible symbols changes neither quantity.[Pass and shelat, A Course in Cryptography, Section 8.3.2, Definition 148.1](https://www.cs.cornell.edu/courses/cs6830/2009fa/lecnotes.pdf)

Suppose someone knows the [probability mass function](probability-distribution.md#probability-mass-function) but receives no observation correlated with $X$, and must name exactly one outcome. Naming $x$ succeeds with [probability](probability-theory.md#probability) $p_x$, so naming a most likely outcome is optimal:

$$
p_{\mathrm{guess}}(X)=\max_x\mathbb P(X=x)=2^{-H_\infty(X)}.
$$

Tied maxima give equally good guesses. Randomizing independently among guesses cannot improve success: if the guess has [probability mass function](probability-distribution.md#probability-mass-function) $q_x$, its success [probability](probability-theory.md#probability) is $\sum_xq_xp_x\leq p_{\max}\sum_xq_x=p_{\max}$. This is the simplest instance of [maximum a posteriori decoding](coding-theory.md#maximum-a-posteriori-decoding). The identity gives [min-entropy](#min-entropy) an operational meaning: $H_\infty(X)\geq k$ [bits](information-theory.md#bit) means every single guess succeeds with [probability](probability-theory.md#probability) at most $2^{-k}$, under these information assumptions.[König, Renner and Schaffner, The operational meaning of min- and max-entropy, Section I.3.1, equation (18) and the no-side-information case](https://arxiv.org/html/0807.1338)

For an exact analytical example on symbols $A,B,C,D,E$, compare the two [probability mass functions](probability-distribution.md#probability-mass-function)

$$
u=(1/4,1/4,1/4,1/4,0),\qquad b=(1/2,1/8,1/8,1/8,1/8).
$$

Under $u$, each possible outcome has [information content](#information-content) $2$ [bits](information-theory.md#bit); under $b$, $A$ has [information content](#information-content) $1$ [bit](information-theory.md#bit) and each other outcome has $3$ [bits](information-theory.md#bit). Consequently their [Shannon entropies](information-entropy.md) agree exactly,

$$
H(u)=4\frac14\cdot2=2,\qquad H(b)=\frac12\cdot1+4\frac18\cdot3=2,
$$

but $H_\infty(u)=2$ and $H_\infty(b)=1$ [bits](information-theory.md#bit). A best single guess therefore succeeds with [probability](probability-theory.md#probability) $1/4$ under $u$ and $1/2$ under $b$. The same average surprise can hide a factor of two in immediate predictability. The zero entry in $u$ contributes zero to [Shannon entropy](information-entropy.md), using $0\log_2 0=0$.

<a id="image-two-exact-probability-models-have-the-same-average-surprise-but-different-best-single-guesses"></a>
![](min-entropy-guessing-equal-average.png)

**[Figure 5](#image-two-exact-probability-models-have-the-same-average-surprise-but-different-best-single-guesses). Two exact probability models have the same average surprise but different best single guesses**.

For the [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution) on $m$ possible outcomes, $H_\infty=\log_2m$ [bits](information-theory.md#bit) and the best single guess succeeds with [probability](probability-theory.md#probability) $1/m$. A certain outcome has $H_\infty=0$ and success [probability](probability-theory.md#probability) one. Thus [min-entropy](#min-entropy) is useful when a common outcome could defeat an attempt to make outputs unpredictable, even if rare alternatives raise [Shannon entropy](information-entropy.md).

For [cryptography](computer-science.md#cryptography), this unconditional calculation alone does not certify security: an observer might know $X$ already. If a report $Y=X$ reveals a uniform four-outcome source, its unconditional [min-entropy](#min-entropy) remains $2$ [bits](information-theory.md#bit) but guessing after the report succeeds with [probability](probability-theory.md#probability) one. For finite classical reports, the appropriate success calculation uses [conditional probabilities](probability-theory.md#conditional-probability) and [maximum a posteriori decoding](coding-theory.md#maximum-a-posteriori-decoding):

$$
p_{\mathrm{guess}}(X\mid Y)=\sum_{y:p_Y(y)>0}p_Y(y)\max_x\mathbb P(X=x\mid Y=y).
$$

The [conditional entropy](information-theory.md#conditional-entropy) $H(X\mid Y)$ instead averages remaining surprise. A security argument must specify the observer's information and the protocol's required guarantee; neither unconditional [min-entropy](#min-entropy) nor [Shannon entropy](information-entropy.md) supplies those assumptions.

### Information entropy dominates min-entropy

↑ **Parent:** [Min-entropy](#min-entropy)

For a [discrete random variable](random-variable.md#discrete-random-variable) $X$ with [probability mass function](probability-distribution.md#probability-mass-function) $p_x$, using base-two [logarithms](calculus.md#logarithm) for both [Shannon entropy](information-entropy.md) and [min-entropy](#min-entropy),

$$
H(X)\geq H_\infty(X)\geq0.
$$

The first inequality says that average [information content](#information-content) cannot be below the least [information content](#information-content) of a possible outcome. For a finite [alphabet](information-theory.md#alphabet), equality $H(X)=H_\infty(X)$ holds exactly when the [probability mass function](probability-distribution.md#probability-mass-function) is uniform on its positive-probability outcomes. Impossible outcomes do not need to share that positive [probability](probability-theory.md#probability). In particular, $(1/2,1/2,0)$ has both quantities equal to $1$ [bit](information-theory.md#bit), while $(1,0,0)$ has both zero. The same equality characterization holds for a countable [alphabet](information-theory.md#alphabet): equality forces only finitely many positive-probability outcomes, because all must have the same positive mass. The uniform maximum of [Shannon entropy](information-entropy.md) is discussed in Shannon's original treatment.[Shannon, A Mathematical Theory of Communication, Section 6, definition of H and properties 1–2](mathematics-bibliography.md#a-mathematical-theory-of-communication-by-claude-shannon)

For the proof, $0<p_x\leq p_{\max}$ gives $-\log_2p_x\geq-\log_2p_{\max}$; taking the [expected value](expected-value.md) proves [information entropy dominates min-entropy](#information-entropy-dominates-min-entropy). More precisely, the nonnegative gap is

$$
H(X)-H_\infty(X)
=\sum_{x:p_x>0}p_x\log_2\frac{p_{\max}}{p_x}\geq0.
$$

It vanishes precisely when every positive term vanishes, namely $p_x=p_{\max}$ for every possible outcome. With $m$ such outcomes, normalization forces $p_{\max}=1/m$. If [Shannon entropy](information-entropy.md) is infinite, the inequality still holds and is strict, because [min-entropy](#min-entropy) of a countable [probability mass function](probability-distribution.md#probability-mass-function) is finite. No subtraction of two infinite quantities is needed.

An analytical family makes the gap visible. Give $A$ [probability](probability-theory.md#probability) $q$ and each of $B,C,D,E$ [probability](probability-theory.md#probability) $(1-q)/4$, with $1/5\leq q\leq1$. Then $A$ is a most likely outcome, so its [probability](probability-theory.md#probability) is also the best single-guess success [probability](probability-theory.md#probability), and

$$
H_\infty(q)=-\log_2q,\qquad H(q)=h_2(q)+2(1-q),
$$

where $h_2$ is [binary entropy](#binary-entropy). The [entropy bound with one prescribed probability](#entropy-bound-with-one-prescribed-probability) explains the second expression: it separates whether $A$ occurred from which of four equally likely alternatives occurred. At $q=1/5$, all five outcomes are uniform and both quantities are $\log_2 5\approx2.3219$ [bits](information-theory.md#bit). At $q=1/2$, [Shannon entropy](information-entropy.md) is $2$ [bits](information-theory.md#bit) while [min-entropy](#min-entropy) is $1$ [bit](information-theory.md#bit), reproducing the biased example in [min-entropy](#min-entropy). At $q=1$, both are zero; the four impossible alternatives contribute nothing. For every $1/5<q<1$, the [probability mass function](probability-distribution.md#probability-mass-function) is nonuniform on its possible outcomes and the gap is strictly positive.

<a id="image-an-analytical-five-outcome-model-separates-average-surprise-from-the-surprise-of-the-most-likely-outcome"></a>
![](min-entropy-guessing-inequality-family.png)

**[Figure 6](#image-an-analytical-five-outcome-model-separates-average-surprise-from-the-surprise-of-the-most-likely-outcome). An analytical five-outcome model separates average surprise from the surprise of the most likely outcome**.

For finite [Shannon entropy](information-entropy.md), exponentiating the inequality gives the useful but potentially loose bound $p_{\mathrm{guess}}(X)\geq2^{-H(X)}$. Equality holds exactly for a [discrete uniform distribution](discrete-probability-distribution.md#discrete-uniform-distribution) on the possible outcomes. Thus [Shannon entropy](information-entropy.md) alone supplies a lower bound on optimal success, not the upper bound needed to promise that every guess is unlikely. [Shannon's source coding theorem](coding-theory.md#shannon-s-source-coding-theorem) concerns average compression under its hypotheses, while [min-entropy](#min-entropy) answers the single-guess question directly. The two quantities serve different tasks even when both are expressed in [bits](information-theory.md#bit).

## Varentropy

↑ **Parent:** [Information entropy](information-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Varentropy)

The varentropy of a discrete random variable with mass function $P$ is the variance of its information content:

$$
V_H(X)=\operatorname{Var}[-\log P(X)].
$$

## Binary entropy

↑ **Parent:** [Information entropy](information-entropy.md)

The binary entropy function is the [information entropy](information-entropy.md) of a [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution):

$$
h_2(p)=-p\log_2p-(1-p)\log_2(1-p),\qquad 0\leq p\leq1,
$$

with endpoint values zero. It is symmetric under $p\mapsto1-p$, reaches one [bit](information-theory.md#bit) at $p=1/2$, and has

$$
h_2'(p)=\log_2\frac{1-p}{p},\qquad h_2''(p)=-\frac1{(\ln2)p(1-p)}<0
$$

in the interior. Its strict [concavity](real-analysis.md#concave-function) expresses why an even mixture of two outcomes has more uncertainty than a strong bias toward either one. The curve in [mutual information](information-theory.md#mutual-information) also shows how this same uncertainty becomes the loss term in [binary symmetric channel capacity](information-theory.md#binary-symmetric-channel-capacity).

## Chain rule for information entropy

↑ **Parent:** [Information entropy](information-entropy.md)

For finite [discrete random variables](random-variable.md#discrete-random-variable), the chain rule counts uncertainty in two stages:

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

The [joint entropy](#joint-entropy) equals the first variable's [information entropy](information-entropy.md) plus the average [conditional entropy](information-theory.md#conditional-entropy) left in the second. All [logarithms](calculus.md#logarithm) here have base two, so the unit is the [bit](information-theory.md#bit); zero-probability terms contribute zero. The identity holds without assuming [independence](random-variable.md#independent-random-variables).[section 6, property 5, reprint p. 12: joint entropy as first entropy plus average conditional entropy](mathematics-bibliography.md#a-mathematical-theory-of-communication-by-claude-shannon)

Iterating gives $H(X_1,\ldots,X_n)=\sum_iH(X_i\mid X_1,\ldots,X_{i-1})$. The first summand means $H(X_1)$, with no earlier observations. Each later summand counts only the new uncertainty after the preceding [random variables](random-variable.md) are known. For [independent random variables](random-variable.md#independent-random-variables), every term is its ordinary [information entropy](information-entropy.md); for dependent ones, adding those ordinary [information entropies](information-entropy.md) can count shared uncertainty repeatedly. This is the reason the [chain rule for information entropy](#chain-rule-for-information-entropy) is useful in [lossless source coding](information-theory.md#lossless-source-coding) and in calculating an [entropy rate](information-theory.md#entropy-rate).

A short proof starts from the factorization of the [joint probability mass function](random-variable.md#joint-probability-mass-function) into a [marginal distribution](probability-distribution.md#marginal-distribution) and a [conditional probability](probability-theory.md#conditional-probability):

$$
p_{X,Y}(x,y)=p_X(x)p_{Y\mid X}(y\mid x),\qquad
-\log_2 p_{X,Y}(x,y)=-\log_2 p_X(x)-\log_2p_{Y\mid X}(y\mid x).
$$

Use this only where $p_{X,Y}(x,y)>0$, then average with those joint [probabilities](probability-theory.md#probability). Summing over $y$ in the first term gives $H(X)$; the second is precisely $H(Y\mid X)$. Repeating the same step with a longer [random vector](random-variable.md#random-vector) proves the iterated identity. Reversing the order also gives $H(X,Y)=H(Y)+H(X\mid Y)$: the two contributions can change with the order, but their total cannot.

### Correlated binary variables

↑ **Parent:** [Chain rule for information entropy](#chain-rule-for-information-entropy)

Let $A$ be a fair [bit](information-theory.md#bit), let $N$ be an [independent](random-variable.md#independent-random-variables) [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) with $\mathbb P(N=1)=p$, and set $B=A\oplus N$, where $\oplus$ is [exclusive or](theoretical-computer-science.md#exclusive-or). Thus $N=1$ flips the first [bit](information-theory.md#bit). This constructs a [binary symmetric channel](coding-theory.md#binary-symmetric-channel) with a fair input, for $0\leq p\leq1$. The [joint probability mass function](random-variable.md#joint-probability-mass-function) is

$$
\begin{array}{c|cc|c}
& B=0&B=1&\mathbb P(A=a)\\\hline
A=0&(1-p)/2&p/2&1/2\\
A=1&p/2&(1-p)/2&1/2\\\hline
\mathbb P(B=b)&1/2&1/2&1
\end{array}
$$

The column sums show that $B$ is also a fair [bit](information-theory.md#bit), whatever $p$ is. Both [marginal distributions](probability-distribution.md#marginal-distribution) therefore have [information entropy](information-entropy.md) one [bit](information-theory.md#bit). Given $A$, only the flip decision remains unknown, giving [conditional entropy](information-theory.md#conditional-entropy) $H(B\mid A)=h_2(p)$, where

$$
h_2(p)=-p\log_2p-(1-p)\log_2(1-p)
$$

is the [binary entropy](#binary-entropy), with $h_2(0)=h_2(1)=0$. The [chain rule for information entropy](#chain-rule-for-information-entropy) and the definition of [mutual information](information-theory.md#mutual-information) now give

$$
\boxed{H(A,B)=1+h_2(p),\qquad I(A;B)=1-h_2(p).}
$$

Take $p=1/10$. The four joint [probabilities](probability-theory.md#probability), in row order, are $(0.45,0.05,0.05,0.45)$. Directly from the definition of [joint entropy](#joint-entropy),

$$
H(A,B)=-2(0.45)\log_2(0.45)-2(0.05)\log_2(0.05)
\approx1.468995594\ \text{bits}.
$$

Conditioning on either value of $A$ gives [probabilities](probability-theory.md#probability) $0.9$ and $0.1$ for the two values of $B$, hence

$$
H(B\mid A)=h_2(0.1)\approx0.468995594\ \text{bits},\qquad
I(A;B)\approx0.531004406\ \text{bits}.
$$

Adding $H(A)+H(B)=2$ would overcount by exactly $I(A;B)$. These are average uncertainties under the stipulated [probability distribution](probability-distribution.md); the four possible pairs are still represented by four distinct outcomes.

<a id="image-a-correlated-binary-pair-contains-one-bit-plus-the-remaining-flip-uncertainty"></a>
![](entropy-chain-rule-joint-table.png)

**[Figure 7](#image-a-correlated-binary-pair-contains-one-bit-plus-the-remaining-flip-uncertainty). A correlated binary pair contains one bit plus the remaining flip uncertainty**. Original exact-model [joint probability mass function](random-variable.md#joint-probability-mass-function) for $p=0.1$. The bars compare the sum of marginal [information entropies](information-entropy.md) with the [joint entropy](#joint-entropy) from the [chain rule for information entropy](#chain-rule-for-information-entropy). The hatched portion is the [mutual information](information-theory.md#mutual-information) counted twice by the marginal sum. Values are calculated, not empirical frequencies.

There is another way to see the decomposition: $(A,B)\mapsto(A,A\oplus B)=(A,N)$ is a [bijection](function.md#bijection). It merely relabels the four outcomes, so it preserves [joint entropy](#joint-entropy). The [independence](random-variable.md#independent-random-variables) of $A$ and $N$ then gives $H(A,B)=H(A,N)=H(A)+H(N)=1+h_2(p)$. Describing the initial [bit](information-theory.md#bit) and the flip decision separates shared uncertainty from new uncertainty.

At $p=0$, the [bits](information-theory.md#bit) are identical: $B=A$, so $H(B\mid A)=0$ and $I(A;B)=1$. At $p=1$, they are complementary: $B=1-A$, with exactly the same [conditional entropy](information-theory.md#conditional-entropy) and [mutual information](information-theory.md#mutual-information). In either case, observing one determines the other. At $p=1/2$, all four joint [probabilities](probability-theory.md#probability) are $1/4$; the [bits](information-theory.md#bit) are [independent](random-variable.md#independent-random-variables), $H(A,B)=2$, and $I(A;B)=0$. Perfect disagreement is therefore just as informative as perfect agreement.

<a id="image-identical-and-complementary-bits-both-reveal-one-full-bit-of-information"></a>
![](entropy-chain-rule-dependence-curves.png)

**[Figure 8](#image-identical-and-complementary-bits-both-reveal-one-full-bit-of-information). Identical and complementary bits both reveal one full bit of information**. Original calculated curves for the constructed pair $B=A\oplus N$: [joint entropy](#joint-entropy) $1+h_2(p)$, [conditional entropy](information-theory.md#conditional-entropy) $h_2(p)$, and [mutual information](information-theory.md#mutual-information) $1-h_2(p)$, all in [bits](information-theory.md#bit). The horizontal line marks the one-bit [information entropy](information-entropy.md) of either [marginal distribution](probability-distribution.md#marginal-distribution). Reflection about $p=1/2$ exchanges likely agreement with likely disagreement while preserving these quantities.

For $p>1/2$, guessing $A=1-B$ succeeds with [probability](probability-theory.md#probability) $p$, better than guessing $A=B$. Changing $B$ to $1-B$ replaces $p$ by $1-p$ and preserves [mutual information](information-theory.md#mutual-information), since the relabeling is invertible. What matters is how well the observation distinguishes the input, rather than how often its symbol matches the input. The same symmetry makes the [binary entropy](#binary-entropy) curve peak at [independence](random-variable.md#independent-random-variables), while the [mutual information](information-theory.md#mutual-information) curve reaches its minimum there.

## Subadditivity of information entropy

↑ **Parent:** [Information entropy](information-entropy.md)

The [chain rule for information entropy](#chain-rule-for-information-entropy) and [conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy) give

$$
H(X,Y)\leq H(X)+H(Y),
$$

with equality exactly when $X$ and $Y$ are [independent](random-variable.md#independent-random-variables).

## Concavity of information entropy

↑ **Parent:** [Information entropy](information-entropy.md)

For probability mass functions $P_1,\ldots,P_m$ and convex weights $\alpha_i$, information entropy satisfies

$$
H\!\left(\sum_i\alpha_iP_i\right)\geq\sum_i\alpha_iH(P_i).
$$

This follows from the [concavity](real-analysis.md#concave-function) of $-t\log t$.

## Maximum entropy distribution on a finite set

↑ **Parent:** [Information entropy](information-entropy.md)

Among [probability distributions](probability-distribution.md) on a finite set of $m$ elements, the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) uniquely maximizes [information entropy](information-entropy.md), attaining $\log m$.

### Maximum entropy distribution with a prescribed finite mean

↑ **Parent:** [Maximum entropy distribution on a finite set](#maximum-entropy-distribution-on-a-finite-set)

For a finite list of real values $y_i$, maximize [information entropy](information-entropy.md) $H=-\sum_i p_i\log p_i$ with $p_i>0$, $\sum_i p_i=1$, and $\sum_i p_i y_i=Y$. [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier) give

$$
p_i=\frac{e^{-by_i}}{Z(b)},\qquad
Z(b)=\sum_j e^{-by_j},\qquad
Y=-\frac{d}{db}\log Z(b).
$$

The constrained second variation is $-\sum_i(\delta p_i)^2/p_i<0$ for any nonzero tangent perturbation, proving uniqueness of the entropy maximum whenever a feasible interior solution exists. The mean has derivative $-\operatorname{Var}_b(y)$, so for nonconstant $y_i$ it decreases strictly with $b$ and ranges between the largest and smallest $y_i$ as $b$ ranges over the real line. Thus a finite $b$ exists uniquely exactly when $\min_i y_i<Y<\max_i y_i$.

At an extreme mean, strictly positive probabilities are impossible unless all $y_i$ coincide. If all $y_i=y_0$, the mean constraint is redundant when $Y=y_0$, the maximum is uniform, and $b$ is not identifiable. This finite [exponential family](exponential-family.md) is an [exponential tilting](probability-distribution.md#exponential-tilting) of the uniform distribution.

### Maximum entropy on a finite alphabet

↑ **Parent:** [Maximum entropy distribution on a finite set](#maximum-entropy-distribution-on-a-finite-set)

An [information entropy](information-entropy.md) on at most $m$ outcomes is at most $\log_2m$, with equality for the uniform distribution on all $m$ outcomes. For the uniform reference $u$, the [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) is $D(p\|u)=\log_2m-H(p)\geq0$, proving the bound.

## Maximum entropy distribution on the nonnegative integers

↑ **Parent:** [Information entropy](information-entropy.md)

Among distributions on $\{0,1,2,\ldots\}$ with fixed [expected value](expected-value.md) $\mu$, the [geometric distribution](discrete-probability-distribution.md#geometric-distribution) with success probability $1/(1+\mu)$ uniquely maximizes [information entropy](information-entropy.md). Its entropy is

$$
(1+\mu)h_2\!\left(\frac1{1+\mu}\right).
$$

## ↑ Ancestors (5)

1. [Information theory](information-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (78)

- [An observation can increase entropy](information-theory.md#an-observation-can-increase-entropy)
- [Asymptotic equipartition property](information-theory.md#asymptotic-equipartition-property)
- [Binary entropy](#binary-entropy)
- [Binary Markov source](information-theory.md#binary-markov-source)
- [Bit](information-theory.md#bit)
- [Chain rule for information entropy](#chain-rule-for-information-entropy)
- [Channel capacity](information-theory.md#channel-capacity)
- [Coloring entropy weight](graph-coloring.md#coloring-entropy-weight)
- [Compression of an entropy sum](information-theory.md#compression-of-an-entropy-sum)
- [Conditional entropy](information-theory.md#conditional-entropy)
- [Conditional entropy rate](information-theory.md#conditional-entropy-rate)
- [Conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy)
- [Correlated binary variables](#correlated-binary-variables)
- [Cross-entropy](#cross-entropy)
- [Cross-entropy equals entropy plus relative entropy](#cross-entropy-equals-entropy-plus-relative-entropy)
- [Differential entropy](#differential-entropy)
- [Differential entropy of a uniform law](#differential-entropy-of-a-uniform-law)
- [Entropy bound for graphs with isolated-vertex-free intersections](information-theory.md#entropy-bound-for-graphs-with-isolated-vertex-free-intersections)
- [Entropy bounds for a type class](information-theory.md#entropy-bounds-for-a-type-class)
- [Entropy monotonicity under independent addition](#entropy-monotonicity-under-independent-addition)
- [Entropy rate](information-theory.md#entropy-rate)
- [Entropy rate and coding length](information-theory.md#entropy-rate-and-coding-length)
- [Entropy rate of a fully observed Markov source](information-theory.md#entropy-rate-of-a-fully-observed-markov-source)
- [Equal-width bin entropy](#equal-width-bin-entropy)
- [Equality in the entropy conditioning inequality](information-theory.md#equality-in-the-entropy-conditioning-inequality)
- [Historical source for total correlation](information-theory.md#historical-source-for-total-correlation)
- [Independent revelation of a binary variable](information-theory.md#independent-revelation-of-a-binary-variable)
- [Independent-set bound for biregular graphs](bipartite-graph.md#independent-set-bound-for-biregular-graphs)
- [Indexing within a type class](information-theory.md#indexing-within-a-type-class)
- [Information entropy](information-entropy.md)
- [Information theory](information-theory.md)
- [Innovations in a binary Markov source](information-theory.md#innovations-in-a-binary-markov-source)
- [Input distribution optimization for a binary symmetric channel](information-theory.md#input-distribution-optimization-for-a-binary-symmetric-channel)
- [Joint entropy](#joint-entropy)
- [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence)
- [Lossless source coding](information-theory.md#lossless-source-coding)
- [Maximum entropy distribution on a finite set](#maximum-entropy-distribution-on-a-finite-set)
- [Maximum entropy distribution on the nonnegative integers](#maximum-entropy-distribution-on-the-nonnegative-integers)
- [Maximum entropy distribution with a prescribed finite mean](#maximum-entropy-distribution-with-a-prescribed-finite-mean)
- [Maximum entropy on a finite alphabet](#maximum-entropy-on-a-finite-alphabet)
- [Method of types](information-theory.md#method-of-types)
- [Mutual information](information-theory.md#mutual-information)
- [Nat (unit)](information-theory.md#nat-unit)
- [Normalized speed of a hereditary hypergraph property](hypergraph.md#normalized-speed-of-a-hereditary-hypergraph-property)
- [Normalized subset entropy](f-divergence.md#normalized-subset-entropy)
- [Parity constraint and total correlation](information-theory.md#parity-constraint-and-total-correlation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-13.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-15.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-15.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#11k/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#3i/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#3k/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-224.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#12h/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#19/b/solution)
- [Poisson entropy monotonicity](discrete-probability-distribution.md#poisson-entropy-monotonicity)
- [Probability of a type class](information-theory.md#probability-of-a-type-class)
- [Shannon's rate-distortion theorem](information-theory.md#shannon-s-rate-distortion-theorem)
- [Stationarity without ergodicity in an information source](information-theory.md#stationarity-without-ergodicity-in-an-information-source)
- [Total correlation](information-theory.md#total-correlation)
- [Uniform-reference information projection maximizes entropy](information-theory.md#uniform-reference-information-projection-maximizes-entropy)
