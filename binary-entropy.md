# Binary entropy

↑ **Parent:** [Information entropy](information-entropy.md)

The binary entropy function is the [information entropy](information-entropy.md) of a [Bernoulli random variable](bernoulli-distribution.md):

$$
h_2(p)=-p\log_2p-(1-p)\log_2(1-p),\qquad 0\leq p\leq1,
$$

with endpoint values zero. It is symmetric under $p\mapsto1-p$, reaches one [bit](bit.md) at $p=1/2$, and has

$$
h_2'(p)=\log_2\frac{1-p}{p},\qquad h_2''(p)=-\frac1{(\ln2)p(1-p)}<0
$$

in the interior. Its strict [concavity](concave-function.md) expresses why an even mixture of two outcomes has more uncertainty than a strong bias toward either one. The curve in [mutual information](mutual-information.md) also shows how this same uncertainty becomes the loss term in [binary symmetric channel capacity](binary-symmetric-channel-capacity.md).

## ↑ Ancestors (6)

1. [Information entropy](information-entropy.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (50)

- [An observation can increase entropy](an-observation-can-increase-entropy.md)
- [Bernoulli typical-set example](bernoulli-typical-set-example.md)
- [Binary cross-entropy](binary-cross-entropy.md)
- [Binary entropy product inequality](binary-entropy-product-inequality.md)
- [Binary rate-distortion function](binary-rate-distortion-function.md)
- [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
- [Collective advantage over independent two-qubit filtering](collective-advantage-over-independent-two-qubit-filtering.md)
- [Data processing inequality](data-processing-inequality.md)
- [Entropy bound for a binary mixture](entropy-bound-for-a-binary-mixture.md)
- [Entropy bound with one prescribed probability](entropy-bound-with-one-prescribed-probability.md)
- [Entropy function for a q-ary alphabet](entropy-function-for-a-q-ary-alphabet.md)
- [Entropy of a binary diagonal qubit mixture](entropy-of-a-binary-diagonal-qubit-mixture.md)
- [Entropy rate and coding length](entropy-rate-and-coding-length.md)
- [Fano's inequality](fano-s-inequality.md)
- [Fano's inequality via an error indicator](fano-s-inequality-via-an-error-indicator.md)
- [Information entropy dominates min-entropy](information-entropy-dominates-min-entropy.md)
- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
- [Joint entropy](joint-entropy.md)
- [Mutual information](mutual-information.md)
- [Noisy parity total correlation](noisy-parity-total-correlation.md)
- [One-shot classical-quantum coding converse](one-shot-classical-quantum-coding-converse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/4/i/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/3k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/11k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2/12k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-323/3/ii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-323/4/c/iii/solution.md)
- [Rate-distortion function](rate-distortion-function.md)
