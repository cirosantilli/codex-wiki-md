<h1 id="gaussian-johnson-lindenstrauss-transform">Gaussian Johnson–Lindenstrauss transform</h1>

↑ **Parent:** [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)

Draw a $k\times D$ [random matrix](random-matrix.md) $G$ whose entries are [independent random variables](independent-random-variables.md) with the [standard normal distribution](standard-normal-distribution.md), and set

$$
T(x)=\frac1{\sqrt k}Gx.
$$

The factor $1/\sqrt k$ makes the [expected value](expected-value.md) of the squared [L2 norm](l2-norm.md) equal to the original squared [L2 norm](l2-norm.md). This [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md) is a [linear map](linear-map.md), generally not an [orthogonal projection](orthogonal-projection.md): its rows are not required to be [orthogonal vectors](orthogonal-vectors.md). [Lecture notes on metric embeddings, §2.1(b), p. 21, and Lemma 2.3.1, p. 24: independent Gaussian coefficients and normalization](lecture-notes-on-metric-embeddings-by-jiri-matousek.md)

For the fixed [finite set](finite-set.md) $S$, let $0<\delta<1$ be an allowed failure [probability](probability.md), and define

$$
c(\varepsilon)=\frac{\varepsilon^2}{4}-\frac{\varepsilon^3}{6}>0.
$$

With $\log$ denoting the [natural logarithm](natural-logarithm.md), a sufficient [integer](integer.md) target [dimension](dimension-vector-space.md) is

$$
k\geq\left\lceil\frac{\log\bigl(n(n-1)/\delta\bigr)}{c(\varepsilon)}\right\rceil.
$$

Then one draw of this specified [random matrix](random-matrix.md) satisfies all the squared [Euclidean distance](euclidean-distance.md) bounds simultaneously with [probability](probability.md) at least $1-\delta$. Since $c(\varepsilon)\geq\varepsilon^2/12$, the simpler sufficient bound $k\geq\lceil12\varepsilon^{-2}\log(n(n-1)/\delta)\rceil$ also works. Both are sufficient bounds for this argument; they do not claim the smallest possible target [dimension](dimension-vector-space.md).

This is a [probability](probability.md) statement about a map drawn independently of the fixed [finite set](finite-set.md). It implies existence because the success [probability](probability.md) is positive, but permits failed draws. The set cannot be chosen after inspecting the map with this same guarantee. In particular, no single draw preserves every possible [finite set](finite-set.md) in the ambient [Euclidean space](euclidean-norm.md) when $k<D$.

**Table of contents**

- [Finite-set example of the Johnson–Lindenstrauss lemma](finite-set-example-of-the-johnson-lindenstrauss-lemma.md)
- [Gaussian Johnson–Lindenstrauss concentration argument](gaussian-johnson-lindenstrauss-concentration-argument.md)

## ↑ Ancestors (7)

1. [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
2. [Metric embedding](metric-embedding.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Finite-set example of the Johnson–Lindenstrauss lemma](finite-set-example-of-the-johnson-lindenstrauss-lemma.md)
- [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)
