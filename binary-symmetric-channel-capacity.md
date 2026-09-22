# Binary symmetric channel capacity

↑ **Parent:** [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)

A [binary symmetric channel](binary-symmetric-channel.md) independently flips each transmitted [bit](bit.md) with crossover [probability](probability.md) $p$. Its [channel capacity](channel-capacity.md) is

$$
C=1-h_2(p),\qquad 0\leq p\leq1,
$$

in [bits](bit.md) per use, where $h_2$ is [binary entropy](binary-entropy.md) and the endpoint convention is $0\log_2 0=0$. Knowing the input leaves just the uncertainty of the flip, so $H(Y\mid X)=h_2(p)$ for every input [probability distribution](probability-distribution-split.md). Since the output is a [bit](bit.md), $H(Y)\leq1$, and thus $I(X;Y)\leq1-h_2(p)$. A fair input produces a fair output and reaches the bound. This is the two-symbol case of [weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md); [Eytan Modiano, MIT 16.36, Channel Capacity and Coding, slides 4–5](https://ocw.mit.edu/courses/16-36-communication-systems-engineering-spring-2009/a49d9e2954b440def3794fe73e79756c_MIT16_36s09_lec13_14.pdf) gives this calculation.

For crossover [probabilities](probability.md) $p=0.01,0.1,0.25$, the resulting [channel capacities](channel-capacity.md) are approximately $0.91920686$, $0.53100441$, and $0.18872188$ [bits](bit.md) per use. At $p=0$, the [communication channel](communication-channel.md) is noiseless; at $p=1/2$, the output is [independent](independent-random-variables.md) of the input and the capacity is zero. At $p=1$, every [bit](bit.md) is inverted, a known reversible rule, and capacity is one again. More generally $C(p)=C(1-p)$, because inverting every received [bit](bit.md) exchanges the two crossover [probabilities](probability.md). The existing [mutual information](mutual-information.md) figure shows this full symmetric curve.

An uncoded transmission illustrates why the raw bit-error [probability](probability.md) is not itself [channel capacity](channel-capacity.md). At $p=0.1$, transmitting 100 uncoded [bits](bit.md) succeeds on all of them with [probability](probability.md) $0.9^{100}\approx0.00002656$. The [probability](probability.md) of at least one error is therefore approximately $0.99997344$. A suitable [block code](block-code.md) changes which received words count as recoverable evidence of a message; simply repeating uncoded transmission at rate one does not obtain the reliability promised at rates below $C$.

**Table of contents**

- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
- [Flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md)

## ↑ Ancestors (7)

1. [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
2. [Channel capacity](channel-capacity.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Binary entropy](binary-entropy.md)
- [Binary symmetric channel](binary-symmetric-channel.md)
- [Channel capacity](channel-capacity.md)
- [Completely noisy binary symmetric channel](completely-noisy-binary-symmetric-channel.md)
- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
- [Mutual information](mutual-information.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/3g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/11i/a/solution.md)
- [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
