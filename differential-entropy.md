# Differential entropy

↑ **Parent:** [Information entropy](information-entropy-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_entropy)

[Differential entropy](differential-entropy.md) describes the spread of a continuous [probability distribution](probability-distribution-split.md) relative to the volume scale of its coordinates. For a real [random variable](random-variable-split.md) $X$ with [probability density function](probability-density-function.md) $f$, use [natural logarithms](natural-logarithm.md) and write

$$
\boxed{h_e(X)=-\int_{\mathbb R} f(x)\ln f(x)\,dx=-\mathbb E[\ln f(X)].}
$$

The convention is $0\ln0=0$. For a finite value, require $\int f|\ln f|<\infty$; if both positive and negative contributions are infinite, the expression is undefined. Unlike a [probability](probability.md), a [probability density](probability-density.md) can exceed one. Consequently [differential entropy](differential-entropy.md) can be negative. Base-two [logarithms](logarithm.md) give $h_2=h_e/\ln2$, in [bits](bit.md) instead of [nats](nat-unit.md).[§1.3, Definition 1.5, equation (1.19) and warning, printed p. 18](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-1-information-measures-entropy-and-divergence.md)

This quantity does not give the exact number of [bits](bit.md) needed to store a real number. A recording device supplies a resolution; [equal-width bin entropy](equal-width-bin-entropy.md) connects that resolution to discrete [information entropy](information-entropy-split.md). The useful continuous quantity is what remains after removing the increasing cost of specifying finer bins. Its dependence on coordinates is visible already in [differential entropy of a uniform law](differential-entropy-of-a-uniform-law.md).

**Table of contents**

- [Differential entropy of a uniform law](differential-entropy-of-a-uniform-law.md)
- [Differential entropy of a Gaussian law](differential-entropy-of-a-gaussian-law.md)
- [Differential entropy under an increasing transformation](differential-entropy-under-an-increasing-transformation.md)
  - [Differential entropy of a squared uniform variable](differential-entropy-of-a-squared-uniform-variable.md)
- [Differential entropy under affine rescaling](differential-entropy-under-affine-rescaling.md)
- [Equal-width bin entropy](equal-width-bin-entropy.md)
- [Relative entropy and coordinate dependence](relative-entropy-and-coordinate-dependence.md)
- [Shannon's continuous-entropy coordinate convention](shannon-s-continuous-entropy-coordinate-convention.md)
- [Entropy power](entropy-power.md)
  - [Entropy power inequality](entropy-power-inequality.md)
    - [Multiplicative entropy power inequality](multiplicative-entropy-power-inequality.md)

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Conditioning and differential entropy](conditioning-and-differential-entropy.md)
- [Differential entropy](differential-entropy.md)
- [Differential entropy of a Gaussian law](differential-entropy-of-a-gaussian-law.md)
- [Differential entropy of a squared uniform variable](differential-entropy-of-a-squared-uniform-variable.md)
- [Differential entropy of a uniform law](differential-entropy-of-a-uniform-law.md)
- [Differential entropy under affine rescaling](differential-entropy-under-affine-rescaling.md)
- [Differential entropy under an increasing transformation](differential-entropy-under-an-increasing-transformation.md)
- [Entropy power](entropy-power.md)
- [Entropy power inequality](entropy-power-inequality.md)
- [Equal-width bin entropy](equal-width-bin-entropy.md)
- [Multiplicative entropy power inequality](multiplicative-entropy-power-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/4/c/solution.md)
- [Relative entropy and coordinate dependence](relative-entropy-and-coordinate-dependence.md)
- [Scope and scale of total correlation](scope-and-scale-of-total-correlation.md)
