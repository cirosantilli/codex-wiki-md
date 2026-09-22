# Mutual information

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mutual_information)

For finite [discrete random variables](discrete-random-variable.md), mutual information is the reduction of [information entropy](information-entropy.md) provided by observing the other variable:

$$
I(X;Y)=H(Y)-H(Y\mid X)
=H(X)+H(Y)-H(X,Y).
$$

The last expression makes the symmetry $I(X;Y)=I(Y;X)$ visible. It is nonnegative and is zero exactly when $X$ and $Y$ are [independent random variables](independent-random-variables.md). One way to see both facts is

$$
I(X;Y)=\sum_{x,y:p(x,y)>0}p(x,y)\log_2\frac{p(x,y)}{p_X(x)p_Y(y)}
=D(p_{X,Y}\Vert p_Xp_Y),
$$

where $D$ is the [Kullback-Leibler divergence](kullback-leibler-divergence.md) with base-two [logarithms](logarithm.md). The [Gibbs inequality](gibbs-inequality.md) gives nonnegativity; equality means that the joint [probability distribution](probability-distribution.md) factors. The statement extends to more general distributions via [relative entropy](kullback-leibler-divergence.md), but differences of infinite [information entropies](information-entropy.md) must not be used as if they were finite numbers.

A [binary symmetric channel](binary-symmetric-channel.md) gives a useful example. Let $X$ be a fair [bit](bit.md), let $N$ be an [independent](independent-random-variables.md) [Bernoulli random variable](bernoulli-distribution.md) with error [probability](probability.md) $q$, and set $Y=X\oplus N$, where $\oplus$ is [exclusive or](exclusive-or.md). The output is also a fair [bit](bit.md), but knowing the input leaves just the error uncertainty:

$$
H(Y)=1,\qquad H(Y\mid X)=h_2(q),\qquad I(X;Y)=1-h_2(q).
$$

Here $h_2$ is [binary entropy](binary-entropy.md). At $q=0.1$, $h_2(q)\approx0.469$, so the output carries about $0.531$ [bits](bit.md) of [mutual information](mutual-information.md) about the input per use. This is an average uncertainty reduction, not a claim that each observed symbol can be divided into fractional physical [bits](bit.md).

<a id="image-binary-entropy-and-retained-information-distinguish-noisy-transmission-from-predictable-bit-inversion"></a>
![](binary-channel-information.png)

**[Figure 6](#image-binary-entropy-and-retained-information-distinguish-noisy-transmission-from-predictable-bit-inversion). Binary entropy and retained information distinguish noisy transmission from predictable bit inversion**.

At $q=1/2$, every output is equally likely for either input, so $I(X;Y)=0$. At $q=1$, the output is always the inverted input: knowing this rule lets the receiver recover the input exactly, so $I(X;Y)=1$ again. A high raw error rate need not mean low [mutual information](mutual-information.md) when the errors are predictable. For this particular channel the fair input is optimal, giving the [binary symmetric channel capacity](binary-symmetric-channel-capacity.md) $1-h_2(q)$.

[Mutual information](mutual-information.md) detects dependence that ordinary [correlation](pearson-correlation-coefficient.md) can miss. Let $X$ be uniform on $\{-1,0,1\}$ and $Y=X^2$. Symmetry gives $\mathbb E[X]=\mathbb E[XY]=0$, hence zero [covariance](covariance.md) and zero [correlation](pearson-correlation-coefficient.md), while $Y$ is completely determined by $X$. Thus $I(X;Y)=H(Y)=h_2(1/3)>0$. This distinction is useful whenever a relationship is nonlinear: knowing one variable can reveal another without a linear trend.

**Table of contents**

- [Entropy submodularity](entropy-submodularity.md)
  - [Compression of an entropy sum](compression-of-an-entropy-sum.md)
    - [Balister–Bollobás entropy inequality](balister-bollobas-entropy-inequality.md)
      - [Madiman–Tetali entropy inequality](madiman-tetali-entropy-inequality.md)
  - [Shearer's inequality](shearer-s-inequality.md)
    - [Entropy bound for graphs with isolated-vertex-free intersections](entropy-bound-for-graphs-with-isolated-vertex-free-intersections.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Chain rule for mutual information](chain-rule-for-mutual-information.md)
- [Data processing inequality](data-processing-inequality.md)
  - [Equality in data processing inequality](equality-in-data-processing-inequality.md)
  - [Conditional data-processing inequality](conditional-data-processing-inequality.md)
- [Incremental information in a twofold binary repetition code](incremental-information-in-a-twofold-binary-repetition-code.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (53)

- [An observation can increase entropy](an-observation-can-increase-entropy.md)
- [Bell correlations versus a classical mixture](bell-correlations-versus-a-classical-mixture.md)
- [Binary entropy](binary-entropy.md)
- [Binary Markov source](binary-markov-source.md)
- [Binary rate-distortion function](binary-rate-distortion-function.md)
- [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
- [Bit](bit.md)
- [Chain decomposition of total correlation](chain-decomposition-of-total-correlation.md)
- [Chain rule for mutual information](chain-rule-for-mutual-information.md)
- [Channel capacity](channel-capacity.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Conditioning and differential entropy](conditioning-and-differential-entropy.md)
- [Data processing inequality](data-processing-inequality.md)
- [Entropy weight of a graph cover](entropy-weight-of-a-graph-cover.md)
- [Equality in data processing inequality](equality-in-data-processing-inequality.md)
- [Fano's inequality](fano-s-inequality.md)
- [Finite-alphabet erasure channel](finite-alphabet-erasure-channel.md)
- [Graph entropy](graph-entropy.md)
- [Independent revelation of a binary variable](independent-revelation-of-a-binary-variable.md)
- [Information theory](information-theory-split.md)
- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
- [Joint entropy](joint-entropy.md)
- [List-decoding Fano inequality](list-decoding-fano-inequality.md)
- [Mutual information](mutual-information.md)
- [Noisy parity total correlation](noisy-parity-total-correlation.md)
- [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33/5/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-15/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-15/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/ii/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/3g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/3i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-224/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/11i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/1/a/solution.md)
- [Quantum information](quantum-information.md)
- [Rate-distortion function](rate-distortion-function.md)
- [Rate-distortion theory](rate-distortion-theory.md)
- [Relative entropy and coordinate dependence](relative-entropy-and-coordinate-dependence.md)
- [Shannon's rate-distortion theorem](shannon-s-rate-distortion-theorem.md)
- [Test channel (information theory)](test-channel-information-theory.md)
- [Total correlation](total-correlation.md)
- [Zero-rate distortion threshold](zero-rate-distortion-threshold.md)
