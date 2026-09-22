# Bi-Lipschitz distortion

↑ **Parent:** [Metric embedding](metric-embedding-split.md)

For an [injective function](injective-function.md) between [metric spaces](metric-space.md) with at least two source points, consider all distance ratios

$$
r_f(x,y)=\frac{d_Y(f(x),f(y))}{d_X(x,y)},\qquad x\ne y.
$$

If constants $0<a\leq b<\infty$ satisfy

$$
a\leq r_f(x,y)\leq b\qquad(x\ne y),
$$

then $f$ is a [bi-Lipschitz map](bi-lipschitz-map.md): both $f$ and its inverse on $f(X)$ are [Lipschitz maps](lipschitz-continuity.md). The bound $b/a$ compares the most expanded pair with the most contracted pair. To define the [bi-Lipschitz distortion](bi-lipschitz-distortion.md) of this particular [metric embedding](metric-embedding-split.md), use the sharp bounds $a=\inf_{x\ne y}r_f(x,y)$ and $b=\sup_{x\ne y}r_f(x,y)$:

$$
\operatorname{dist}(f)=\frac ba
=\operatorname{Lip}(f)\operatorname{Lip}(f^{-1})\geq1.
$$

Here the [Lipschitz constant](lipschitz-constant.md) of $f^{-1}:f(X)\to X$ is $1/a$. If no positive finite bounds exist, the [bi-Lipschitz distortion](bi-lipschitz-distortion.md) is infinite. For a finite source, every [injective function](injective-function.md) has finite [bi-Lipschitz distortion](bi-lipschitz-distortion.md), but its size can depend on the source. Matoušek gives the equivalent definition using one scale factor and a multiplicative error bound. [Matoušek, Section 1.1: distortion and Lipschitz maps](lecture-notes-on-metric-embeddings-by-jiri-matousek.md)

Changing units is harmless: replacing $d_Y$ by $\lambda d_Y$, with $\lambda>0$, multiplies both $a$ and $b$ by $\lambda$ and leaves $b/a$ unchanged. In a [normed vector space](normed-vector-space-split.md) this can be achieved by multiplying every output [vector](vector.md) by $\lambda$. Thus [bi-Lipschitz distortion](bi-lipschitz-distortion.md) one means that all distances change by the same factor; an [isometric embedding](isometric-embedding.md) additionally requires that factor to be one. A [stretch factor](stretch-factor.md) with a specified normalization is a related quantity; when comparing sources, check which overall scale has been fixed.

Take the four corners $A=(0,0)$, $B=(1,0)$, $C=(1,1)$, $D=(0,1)$ of a [square](square.md), with [Euclidean distance](euclidean-distance.md) in both source and target. For the [linear map](linear-map.md) $f(x,y)=(2x,y)$, the six unordered pairs exhaust the possibilities: the two vertical sides $AD,BC$ have ratio $1$, the two horizontal sides $AB,CD$ have ratio $2$, and the two diagonals $AC,BD$ have ratio $\sqrt5/\sqrt2=\sqrt{5/2}$. Consequently $a=1$, $b=2$, and $\operatorname{dist}(f)=2$. In contrast, $g(x,y)=(3x,3y)$, three times the [identity function](identity-function.md), gives ratio $3$ for every pair and has [bi-Lipschitz distortion](bi-lipschitz-distortion.md) $3/3=1$.

<a id="image-uniform-scaling-keeps-distortion-one-unequal-coordinate-scaling-gives-distortion-two"></a>
![](metric-embedding-distance-ratios.png)

**[Figure 1](#image-uniform-scaling-keeps-distortion-one-unequal-coordinate-scaling-gives-distortion-two). Uniform scaling keeps distortion one; unequal coordinate scaling gives distortion two**.

The ratio chart makes the reason visible: a common multiplier moves every ratio together, while unequal coordinate scaling spreads the ratios apart. More generally, in a [normed vector space](normed-vector-space-split.md), the ratio bounds give

$$
\frac1{b/a}d_X(x,y)\leq\left\|\frac{f(x)}b-\frac{f(y)}b\right\|\leq d_X(x,y).
$$

This normalization gives [Lipschitz constant](lipschitz-constant.md) one and inverse [Lipschitz constant](lipschitz-constant.md) $b/a$. It is only a change of scale, so it cannot improve the [bi-Lipschitz distortion](bi-lipschitz-distortion.md).

The best possible [bi-Lipschitz distortion](bi-lipschitz-distortion.md) of a source into a specified target is a separate quantity:

$$
c_Y(X)=\inf_{f:X\hookrightarrow Y}\operatorname{dist}(f).
$$

The [infimum](infimum.md) runs over all [injective functions](injective-function.md), and need not be attained. The notation $c_p(X)$ means the analogous [infimum](infimum.md) over [metric embeddings](metric-embedding-split.md) into an [Lp space](lp-space.md). A calculation for one chosen $f$ gives an upper bound for $c_Y(X)$; proving optimality also requires a lower bound for every possible $f$.

**Table of contents**

- [Stretch factor](stretch-factor.md)

## ↑ Ancestors (6)

1. [Metric embedding](metric-embedding-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Bi-Lipschitz distortion](bi-lipschitz-distortion.md)
- [Bi-Lipschitz map](bi-lipschitz-map.md)
- [Coarse embedding](coarse-embedding.md)
- [Finite-set example of the Johnson–Lindenstrauss lemma](finite-set-example-of-the-johnson-lindenstrauss-lemma.md)
- [Hamming cube as an L1 and L2 metric](hamming-cube-as-an-l1-and-l2-metric.md)
- [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
- [Metric embedding](metric-embedding-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-132/4/a/solution.md)
- [Stretch factor](stretch-factor.md)
