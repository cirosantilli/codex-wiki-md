<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

Write the [Laurent series](../../../../../laurent-series.md) on the punctured disc as $f(z)=\sum_{j=-\infty}^{\infty}a_jz^j$. A [removable singularity](../../../../../removable-singularity.md) means that $f$ extends holomorphically to the origin; exactly all negative-index coefficients vanish. A [pole](../../../../../pole.md) of order $k\ge1$ means that $z^kf(z)$ extends with nonzero value at zero; exactly $a_{-k}\ne0$ and every coefficient below $-k$ vanishes. An [essential singularity](../../../../../essential-singularity.md) is neither of these cases; exactly infinitely many negative-index coefficients are nonzero.

Here is a proof of the required [Casorati-Weierstrass theorem](../../../../../casorati-weierstrass-theorem.md) consequence. If some disc of values around $w$ were missed in a punctured neighbourhood, then $|f(z)-w|\ge\varepsilon>0$ there. The [holomorphic function](../../../../../holomorphic-function.md) $q(z)=1/(f(z)-w)$ would be bounded, and hence have a [removable singularity](../../../../../removable-singularity.md). If its extension had $q(0)\ne0$, then $f=w+1/q$ would extend holomorphically. If $q(0)=0$, its zero has a finite positive order, since $q$ is not identically zero; thus $f$ would have a [pole](../../../../../pole.md). Both contradict an [essential singularity](../../../../../essential-singularity.md). Therefore every sufficiently small punctured neighbourhood has values arbitrarily close to every $w$. Choosing $0<|z_n|<\min(r/2,1/n)$ with $|f(z_n)-w|<1/n$ proves

$$
\boxed{z_n\to0,\qquad f(z_n)\to w.}
$$

The [open mapping theorem](../../../../../open-mapping-theorem-complex-analysis.md) states that a nonconstant [holomorphic function](../../../../../holomorphic-function.md) on a domain maps open sets to open sets. If $f$ were injective with an [essential singularity](../../../../../essential-singularity.md), choose a small open disc $U$ away from zero and a point $z_0\in U$. Its open image contains a disc about $w=f(z_0)$. The sequence just constructed has $z_n\to0$ outside $U$, but eventually $f(z_n)\in f(U)$. Thus some $y_n\in U$ has $f(y_n)=f(z_n)$ although $y_n\ne z_n$, contradicting injectivity. **An injective [holomorphic function](../../../../../holomorphic-function.md) cannot have an isolated [essential singularity](../../../../../essential-singularity.md).**

For an injective [entire function](../../../../../entire-function.md) $g$, apply this to $f(z)=g(1/z)$. If its singularity at zero were removable, $g$ would be bounded outside a large disc, hence bounded everywhere and constant by [Liouville's theorem](../../../../../liouville-theorem.md). This contradicts injectivity. It must therefore be a [pole](../../../../../pole.md), say of order $k$, so $|g(z)|\le C|z|^k$ for large $|z|$. For any Taylor coefficient of index $j>k$, the [Cauchy coefficient formula](../../../../../cauchy-coefficient-formula.md) gives $|a_j|\le CR^{k-j}$ on arbitrarily large circles; hence $a_j=0$. Thus $g$ is a nonconstant polynomial. Its derivative never vanishes by the allowed injectivity fact. If its degree exceeded one, the [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) would give a zero of this nonconstant derivative. Therefore [injective entire functions are affine](../../../../../injective-entire-functions-are-affine.md):

$$
\boxed{g(z)=az+b,\qquad a\ne0.}
$$

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
