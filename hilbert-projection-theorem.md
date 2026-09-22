# Hilbert projection theorem

↑ **Parent:** [Hilbert space](hilbert-space-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_projection_theorem)

For every nonempty [closed convex set](closed-convex-set.md) $C$ in a [Hilbert space](hilbert-space-split.md) and every $x$ in that space, there is a unique $p\in C$ satisfying

$$
\|x-p\|=\inf_{z\in C}\|x-z\|.
$$

Closedness and completeness let a limiting approximation attain the infimum; [convexity](convex-function.md) prevents two different minimizers. The proof idea is to choose a sequence approaching the infimum. The [parallelogram identity](parallelogram-law.md) and the admissible midpoint make it a [Cauchy sequence](cauchy-sequence.md); applying the same identity to two putative minimizers proves uniqueness.

For a [closed subspace of a Hilbert space](closed-subspace-of-a-hilbert-space.md), this nearest-point map is an [orthogonal projection](orthogonal-projection.md) and is [linear](linearity.md). For a general [closed convex set](closed-convex-set.md) it need not be [linear](linearity.md): projecting the real line onto $[0,1]$ clips values below zero to zero and values above one to one. The theorem is therefore useful for both linear approximation and constrained nearest-point problems.[Rodriguez, MIT 18.102, lecture 17: minimizers and orthogonal complements](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/resources/18102-sp21-lecture-17/)

Closedness is essential even in familiar examples. For the open [interval](interval-mathematics.md) $(0,1)\subseteq\mathbb R$ and $x=0$, the distance infimum is zero but no nearest point exists. The same obstruction appears when approximating $(1/k)_{k\geq1}$ by [finitely supported sequences](finitely-supported-sequence.md): the infimum is zero, but the limit lies outside that subspace until we take its [Hilbert space completion](hilbert-space-completion.md).

**Table of contents**

- [Orthogonal decomposition by a closed subspace](orthogonal-decomposition-by-a-closed-subspace.md)
  - [Orthogonal complement](orthogonal-complement.md)
    - [Double orthogonal complement](double-orthogonal-complement.md)
  - [Orthogonal projection](orthogonal-projection.md)
    - [Directed subspace angle](directed-subspace-angle.md)
      - [Complementarity from two directed subspace angles](complementarity-from-two-directed-subspace-angles.md)
    - [Smallest angle between two subspaces](smallest-angle-between-two-subspaces.md)
      - [Kitaev geometrical lemma](kitaev-geometrical-lemma.md)
    - [Powers of a product of two orthogonal projections](powers-of-a-product-of-two-orthogonal-projections.md)

## ↑ Ancestors (6)

1. [Hilbert space](hilbert-space-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Closed convex set](closed-convex-set.md)
- [Hilbert space](hilbert-space-split.md)
- [Parallelogram law](parallelogram-law.md)
