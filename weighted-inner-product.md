# Weighted inner product

↑ **Parent:** [Inner product](inner-product.md)

For a positive weight $w$, the weighted inner product of [functions](function-split.md) is $\langle f,g\rangle_w=\int\overline f g w$. It is the usual [inner product](inner-product.md) in the [L2 space](l2-space-is-a-hilbert-space.md) for the measure $w(x)dx$. A [Sturm-Liouville eigenfunction expansion](sturm-liouville-eigenfunction-expansion.md) uses this weight to make its [eigenfunctions](eigenfunction.md) [orthogonal](orthogonal-vectors.md).

The weight specifies how different locations contribute to a squared error: $\|f-g\|_w^2=\int|f-g|^2w$. More weight makes an error in that region more costly. The [weighted Euclidean inner product](weighted-euclidean-inner-product.md) makes the same choice for a finite list of coordinates.

For an explicit real-function example on $[0,1]$, let $w(x)=1+x$ and approximate $f(x)=x$ by a [constant function](constant-function.md). The [orthogonal projection onto a finite-dimensional subspace](orthogonal-projection-onto-a-finite-dimensional-subspace.md) spanned by the function $1$ gives

$$
c=\frac{\langle x,1\rangle_w}{\langle1,1\rangle_w}
=\frac{\int_0^1x(1+x)\,dx}{\int_0^1(1+x)\,dx}
=\frac{5/6}{3/2}=\frac59.
$$

The best unweighted constant is $1/2$. Giving greater weight to larger $x$ moves the best constant upward, so a weighting choice changes the approximation even though the allowed family of [functions](function-split.md) is unchanged.

**Table of contents**

- [Weighted Euclidean inner product](weighted-euclidean-inner-product.md)

## ↑ Ancestors (6)

1. [Inner product](inner-product.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Adjoint in weighted coordinates](adjoint-in-weighted-coordinates.md)
- [Orthogonal vectors](orthogonal-vectors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/2/solution.md)
- [Weighted Euclidean inner product](weighted-euclidean-inner-product.md)
- [Weighted Neumann heat kernel with constant drift](weighted-neumann-heat-kernel-with-constant-drift.md)
