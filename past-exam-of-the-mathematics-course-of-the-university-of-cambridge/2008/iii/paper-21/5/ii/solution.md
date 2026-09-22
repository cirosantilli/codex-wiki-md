<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $P\in X(k)$ and put $D=(g+1)P$. The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) gives

$$
\ell(D)=\deg D+1-g+\ell(K-D)=2+\ell(K-D)\ge2.
$$

As constants supply only a one-dimensional subspace, the [Riemann-Roch space](../../../../../../riemann-roch-space.md) $L(D)$ contains a nonconstant [rational function](../../../../../../rational-function.md) $f$. It has no poles except possibly at $P$. It must have a pole, since a global [regular function](../../../../../../regular-function.md) on an irreducible [projective variety](../../../../../../projective-variety.md) is constant. Let its pole order at $P$ be $m$; then $1\le m\le g+1$.

On the open set where $f$ is regular, define $\phi=[f:1]$. At its pole use the other affine chart, $\phi=[1:1/f]$. The [local ring of a smooth algebraic curve](../../../../../../local-ring-of-a-smooth-algebraic-curve.md) is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md), and the positive valuation of $1/f$ at $P$ makes the latter expression regular there. The two expressions agree on their overlap, so they give a regular map $X\to\mathbb P^1$.

This map is nonconstant. It is proper because its source is projective and its target is separated, so its image is closed; a nonconstant image in the projective line must be the whole line. Each finite-value fibre consists of zeros of a nonzero [rational function](../../../../../../rational-function.md) $f-a$, and the infinity fibre is the finite pole set. Hence every fibre is finite, giving a [quasi-finite morphism](../../../../../../quasi-finite-morphism.md). The proper quasi-finite criterion therefore makes $\phi$ a [finite morphism](../../../../../../finite-morphism.md).

Finally its pullback of the infinity divisor is exactly the pole divisor $mP$. The [degree of a morphism of curves](../../../../../../degree-of-a-morphism-of-curves.md) equals the degree of this pullback, or equivalently the function-field extension degree $[k(X):k(f)]$. Thus

$$
\boxed{\deg\phi=m\le g+1.}
$$

The argument includes inseparable maps: the degree here is the full field-extension degree, not just the separable degree. This proves the [gonality bound from Riemann-Roch](../../../../../../gonality-bound-from-riemann-roch.md) with an explicitly constructed finite regular map.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
