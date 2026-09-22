# Min-entropy

↑ **Parent:** [Information entropy](information-entropy-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Min-entropy)

For a [discrete random variable](discrete-random-variable.md) $X$ with a finite or countable [alphabet](alphabet.md) and [probability mass function](probability-mass-function.md) $p_x=\mathbb P(X=x)$, define $p_{\max}=\max_xp_x$. Its [min-entropy](min-entropy.md), using base-two [logarithms](logarithm.md), is

$$
H_\infty(X)=-\log_2p_{\max}
=\min_{x:p_x>0}(-\log_2p_x).
$$

The unit is the [bit](bit.md). This is the smallest [information content](information-content.md) of any possible outcome: it records the easiest outcome to predict, whereas [Shannon entropy](information-entropy-split.md) averages [information content](information-content.md) over all outcomes. A normalized countable [probability mass function](probability-mass-function.md) has an attained positive maximum, so $H_\infty(X)$ is finite even when [Shannon entropy](information-entropy-split.md) is infinite. Outcomes of zero [probability](probability.md) cannot minimize the surprise and are omitted from the minimum; including extra impossible symbols changes neither quantity.[Pass and shelat, A Course in Cryptography, Section 8.3.2, Definition 148.1](https://www.cs.cornell.edu/courses/cs6830/2009fa/lecnotes.pdf)

Suppose someone knows the [probability mass function](probability-mass-function.md) but receives no observation correlated with $X$, and must name exactly one outcome. Naming $x$ succeeds with [probability](probability.md) $p_x$, so naming a most likely outcome is optimal:

$$
p_{\mathrm{guess}}(X)=\max_x\mathbb P(X=x)=2^{-H_\infty(X)}.
$$

Tied maxima give equally good guesses. Randomizing independently among guesses cannot improve success: if the guess has [probability mass function](probability-mass-function.md) $q_x$, its success [probability](probability.md) is $\sum_xq_xp_x\leq p_{\max}\sum_xq_x=p_{\max}$. This is the simplest instance of [maximum a posteriori decoding](maximum-a-posteriori-decoding.md). The identity gives [min-entropy](min-entropy.md) an operational meaning: $H_\infty(X)\geq k$ [bits](bit.md) means every single guess succeeds with [probability](probability.md) at most $2^{-k}$, under these information assumptions.[König, Renner and Schaffner, The operational meaning of min- and max-entropy, Section I.3.1, equation (18) and the no-side-information case](https://arxiv.org/html/0807.1338)

For an exact analytical example on symbols $A,B,C,D,E$, compare the two [probability mass functions](probability-mass-function.md)

$$
u=(1/4,1/4,1/4,1/4,0),\qquad b=(1/2,1/8,1/8,1/8,1/8).
$$

Under $u$, each possible outcome has [information content](information-content.md) $2$ [bits](bit.md); under $b$, $A$ has [information content](information-content.md) $1$ [bit](bit.md) and each other outcome has $3$ [bits](bit.md). Consequently their [Shannon entropies](information-entropy-split.md) agree exactly,

$$
H(u)=4\frac14\cdot2=2,\qquad H(b)=\frac12\cdot1+4\frac18\cdot3=2,
$$

but $H_\infty(u)=2$ and $H_\infty(b)=1$ [bits](bit.md). A best single guess therefore succeeds with [probability](probability.md) $1/4$ under $u$ and $1/2$ under $b$. The same average surprise can hide a factor of two in immediate predictability. The zero entry in $u$ contributes zero to [Shannon entropy](information-entropy-split.md), using $0\log_2 0=0$.

<a id="image-two-exact-probability-models-have-the-same-average-surprise-but-different-best-single-guesses"></a>
![](min-entropy-guessing-equal-average.png)

**[Figure 5](#image-two-exact-probability-models-have-the-same-average-surprise-but-different-best-single-guesses). Two exact probability models have the same average surprise but different best single guesses**.

For the [discrete uniform distribution](discrete-uniform-distribution.md) on $m$ possible outcomes, $H_\infty=\log_2m$ [bits](bit.md) and the best single guess succeeds with [probability](probability.md) $1/m$. A certain outcome has $H_\infty=0$ and success [probability](probability.md) one. Thus [min-entropy](min-entropy.md) is useful when a common outcome could defeat an attempt to make outputs unpredictable, even if rare alternatives raise [Shannon entropy](information-entropy-split.md).

For [cryptography](cryptography.md), this unconditional calculation alone does not certify security: an observer might know $X$ already. If a report $Y=X$ reveals a uniform four-outcome source, its unconditional [min-entropy](min-entropy.md) remains $2$ [bits](bit.md) but guessing after the report succeeds with [probability](probability.md) one. For finite classical reports, the appropriate success calculation uses [conditional probabilities](conditional-probability.md) and [maximum a posteriori decoding](maximum-a-posteriori-decoding.md):

$$
p_{\mathrm{guess}}(X\mid Y)=\sum_{y:p_Y(y)>0}p_Y(y)\max_x\mathbb P(X=x\mid Y=y).
$$

The [conditional entropy](conditional-entropy.md) $H(X\mid Y)$ instead averages remaining surprise. A security argument must specify the observer's information and the protocol's required guarantee; neither unconditional [min-entropy](min-entropy.md) nor [Shannon entropy](information-entropy-split.md) supplies those assumptions.

**Table of contents**

- [Information entropy dominates min-entropy](information-entropy-dominates-min-entropy.md)

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Information entropy dominates min-entropy](information-entropy-dominates-min-entropy.md)
- [Min-entropy](min-entropy.md)
