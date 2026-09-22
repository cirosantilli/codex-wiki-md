<h1 id="johnson-lindenstrauss-lemma">Johnson–Lindenstrauss lemma</h1>

↑ **Parent:** [Metric embedding](metric-embedding-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Johnson–Lindenstrauss_lemma)

For $0<\varepsilon<1$ and any $n$ points in a Hilbert space, there is a linear map into Euclidean dimension $O(\varepsilon^{-2}\log n)$ that multiplies every pairwise distance by a factor between $1-\varepsilon$ and $1+\varepsilon$.

The striking feature is that the target [dimension](dimension-vector-space.md) depends on the number of points and the allowed error, independently of the ambient [dimension](dimension-vector-space.md). Fix a [finite set](finite-set.md) $S=\{x_1,\ldots,x_n\}\subset\mathbb R^D$, with $n\geq2$, and $0<\varepsilon<1$. An equivalent sufficient statement uses squared [Euclidean distances](euclidean-distance.md): a [linear map](linear-map.md) $T:\mathbb R^D\to\mathbb R^k$ exists, with $k=O(\varepsilon^{-2}\log n)$, such that

$$
(1-\varepsilon)\|x_i-x_j\|_2^2
\leq\|Tx_i-Tx_j\|_2^2
\leq(1+\varepsilon)\|x_i-x_j\|_2^2
\qquad(1\leq i<j\leq n).
$$

The finite-set theorem cited here supplies an explicit sufficient target [dimension](dimension-vector-space.md) for this squared-distance formulation. [An elementary proof of a theorem of Johnson and Lindenstrauss, Theorem 2.1, p. 61: bounds for squared distances](an-elementary-proof-of-a-theorem-of-johnson-and-lindenstrauss-by-sanjoy-dasgupta-and-anupam-gupta.md)

Taking [square roots](square-root.md) gives distance factors $\sqrt{1-\varepsilon}$ and $\sqrt{1+\varepsilon}$, which lie inside $[1-\varepsilon,1+\varepsilon]$. Conversely, bounds $1\pm\varepsilon$ on distances only give squared-distance bounds $(1\pm\varepsilon)^2$; the same numerical tolerance should not be silently used for both. Under the squared-distance bounds, the [bi-Lipschitz distortion](bi-lipschitz-distortion.md) is at most $\sqrt{(1+\varepsilon)/(1-\varepsilon)}$.

The [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md) preserves this fixed [finite set](finite-set.md), rather than every [vector](vector.md) in the ambient [Euclidean space](euclidean-norm.md). A [linear map](linear-map.md) with $k<D$ has a nonzero [kernel](kernel-of-a-linear-map-split.md) by the [rank-nullity theorem](rank-nullity-theorem.md), so some nonzero [vectors](vector.md) collapse completely. For finitely many points in a real [Hilbert space](hilbert-space-split.md), apply the finite-dimensional argument on their [linear span](linear-span.md) and extend by [orthogonal projection](orthogonal-projection.md) onto that [linear span](linear-span.md). If the sufficient target [dimension](dimension-vector-space.md) exceeds the ambient [dimension](dimension-vector-space.md), the [identity map](identity-function.md) already preserves every [Euclidean distance](euclidean-distance.md) exactly, with zero padding if a larger target is requested.

**Table of contents**

- [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)
  - [Finite-set example of the Johnson–Lindenstrauss lemma](finite-set-example-of-the-johnson-lindenstrauss-lemma.md)
  - [Gaussian Johnson–Lindenstrauss concentration argument](gaussian-johnson-lindenstrauss-concentration-argument.md)
- [Net estimate for a linear operator](net-estimate-for-a-linear-operator.md)
- [Rademacher Johnson–Lindenstrauss transform](rademacher-johnson-lindenstrauss-transform.md)
- [Subgaussian concentration of the absolute Gaussian average](subgaussian-concentration-of-the-absolute-gaussian-average.md)
  - [Almost-isometric Gaussian embedding from l2 into l1](almost-isometric-gaussian-embedding-from-l2-into-l1.md)
    - [Low-dimensional L1 embedding of a finite metric space](low-dimensional-l1-embedding-of-a-finite-metric-space.md)

## ↑ Ancestors (6)

1. [Metric embedding](metric-embedding-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Finite-set example of the Johnson–Lindenstrauss lemma](finite-set-example-of-the-johnson-lindenstrauss-lemma.md)
- [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
- [Low-dimensional L1 embedding of a finite metric space](low-dimensional-l1-embedding-of-a-finite-metric-space.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-155/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-205/3/b/solution.md)
