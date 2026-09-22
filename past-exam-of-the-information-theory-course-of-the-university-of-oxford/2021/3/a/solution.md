<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [discrete memoryless channel](../../../../discrete-memoryless-channel.md) with [transition probabilities](../../../../transition-probability.md) $M(y\mid x)$, the [conditional probability](../../../../conditional-probability.md) of a length-$n$ output given a length-$n$ input factors as

$$
\mathbb P(Y_1=y_1,\ldots,Y_n=y_n\mid X_1=x_1,\ldots,X_n=x_n)=\prod_{j=1}^n M(y_j\mid x_j).
$$

The same [transition probabilities](../../../../transition-probability.md) apply at each use. Its [channel capacity](../../../../channel-capacity.md) is

$$
\boxed{C=\max_{p_X}I(X;Y)=\max_{p_X}\sum_{x,y}p_X(x)M(y\mid x)\log_2\frac{M(y\mid x)}{\sum_{x'}p_X(x')M(y\mid x')} .}
$$

The unit is [bits](../../../../bit.md) per channel use. For [finite alphabets](../../../../finite-alphabet.md) the maximum exists by [continuity](../../../../continuous-function.md) on the [probability simplex](../../../../probability-simplex.md); with more general [alphabets](../../../../alphabet.md) one uses a [supremum](../../../../supremum.md) when appropriate.

An $(m,n)$ [channel code](../../../../channel-code.md) consists of an [encoder](../../../../channel-encoder.md) $c:\mathcal V_m\to\mathcal X^n$ and a [decoder](../../../../channel-decoder.md) $d:\mathcal Y^n\to\mathcal V_m$. It represents each of $m$ messages by $n$ input symbols and recovers a message from the $n$ observed output symbols. Its [code rate](../../../../code-rate.md) is **$R=(\log_2m)/n$ [bits](../../../../bit.md) per use**. For each message $w$, its conditional error [probability](../../../../probability.md) is $\mathbb P(d(Y^n)\ne w\mid W=w)$; an average error also specifies the message [probability distribution](../../../../probability-distribution-split.md), while the maximum error takes the largest conditional error.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
