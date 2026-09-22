# Metric embedding

↑ **Parent:** [Functional analysis](functional-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metric_embedding)

A [metric embedding](metric-embedding.md) represents the points of one [metric space](metric-space.md) $(X,d_X)$ inside another $(Y,d_Y)$ by an [injective function](injective-function.md) $f:X\to Y$. The geometric question is how faithfully the representation preserves pairwise distances. For example, [binary strings](binary-string.md) can be treated as [vectors](vector.md) so that tools from [linear algebra](linear-algebra-split.md) become available, but the chosen [norm](norm.md) determines what their separation means. A drawing of the points alone does not specify a [metric embedding](metric-embedding.md): both [metrics](metric.md) matter.

An [isometric embedding](isometric-embedding.md) preserves every distance exactly. A [metric embedding](metric-embedding.md) that is a [bi-Lipschitz map](bi-lipschitz-map.md) allows multiplicative error while keeping its [bi-Lipschitz distortion](bi-lipschitz-distortion.md) bounded over all pairs. A [coarse embedding](coarse-embedding.md) instead controls separation through possibly nonlinear functions of distance. These are different requirements: the [Hamming cube as an L1 and L2 metric](hamming-cube-as-an-l1-and-l2-metric.md) below preserves [Hamming distance](hamming-distance.md) exactly in one representation and takes its [square root](square-root.md) in another.

The usefulness is that a complicated distance comparison becomes a calculation with familiar [vectors](vector.md) and [norms](norm.md). This also helps assess a visualization: nearby points should not acquire arbitrarily large separations, and far-apart points should not collapse together. Matoušek's 2013 lecture notes describe how motivations from [computer science](computer-science-split.md), especially [approximation algorithms](approximation-algorithm.md), accelerated the study of [metric embeddings](metric-embedding.md) from the 1990s onward. [Jiří Matoušek, Lecture notes on metric embeddings, preface and Section 1.1](lecture-notes-on-metric-embeddings-by-jiri-matousek.md)

**Table of contents**

- [Bi-Lipschitz distortion](bi-lipschitz-distortion.md)
  - [Stretch factor](stretch-factor.md)
- [Coarse embedding](coarse-embedding.md)
  - [Uniform coarse embedding of a family of metric spaces](uniform-coarse-embedding-of-a-family-of-metric-spaces.md)
- [Hamming cube as an L1 and L2 metric](hamming-cube-as-an-l1-and-l2-metric.md)
- [Expander graph](expander-graph.md)
  - [Zig-zag product](zig-zag-product.md)
    - [Squaring and zig-zag iteration yields bounded-degree expanders](squaring-and-zig-zag-iteration-yields-bounded-degree-expanders.md)
  - [L1 Poincare inequality for an expander graph](l1-poincare-inequality-for-an-expander-graph.md)
    - [Layer cake representation](layer-cake-representation.md)
      - [Lp bound from a tail domination inequality](lp-bound-from-a-tail-domination-inequality.md)
    - [L1 distortion lower bound for an expander graph](l1-distortion-lower-bound-for-an-expander-graph.md)
  - [Expander graph obstruction to uniform coarse embedding](expander-graph-obstruction-to-uniform-coarse-embedding.md)
- [Finite representability of a Banach space](finite-representability-of-a-banach-space.md)
  - [Superreflexive Banach space](superreflexive-banach-space.md)
    - [Convex-block separation criterion for reflexivity](convex-block-separation-criterion-for-reflexivity.md)
      - [James's theorem](james-s-theorem.md)
        - [Principle of local reflexivity](principle-of-local-reflexivity.md)
    - [Uniform finite convex-block criterion for superreflexivity](uniform-finite-convex-block-criterion-for-superreflexivity.md)
    - [Diamond-graph characterization of superreflexivity](diamond-graph-characterization-of-superreflexivity.md)
- [Bourgain embedding theorem](bourgain-embedding-theorem.md)
  - [Fréchet embedding](frechet-embedding.md)
  - [Low-dimensional Frechet embedding into linfinity](low-dimensional-frechet-embedding-into-linfinity.md)
    - [Dimension lower bound for an expander embedded in linfinity](dimension-lower-bound-for-an-expander-embedded-in-linfinity.md)
- [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
  - [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)
    - [Finite-set example of the Johnson–Lindenstrauss lemma](finite-set-example-of-the-johnson-lindenstrauss-lemma.md)
    - [Gaussian Johnson–Lindenstrauss concentration argument](gaussian-johnson-lindenstrauss-concentration-argument.md)
  - [Net estimate for a linear operator](net-estimate-for-a-linear-operator.md)
  - [Rademacher Johnson–Lindenstrauss transform](rademacher-johnson-lindenstrauss-transform.md)
  - [Subgaussian concentration of the absolute Gaussian average](subgaussian-concentration-of-the-absolute-gaussian-average.md)
    - [Almost-isometric Gaussian embedding from l2 into l1](almost-isometric-gaussian-embedding-from-l2-into-l1.md)
      - [Low-dimensional L1 embedding of a finite metric space](low-dimensional-l1-embedding-of-a-finite-metric-space.md)

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Bi-Lipschitz distortion](bi-lipschitz-distortion.md)
- [Bi-Lipschitz map](bi-lipschitz-map.md)
- [Coarse embedding](coarse-embedding.md)
- [Hamming cube as an L1 and L2 metric](hamming-cube-as-an-l1-and-l2-metric.md)
- [Metric embedding](metric-embedding.md)
