<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here the [degree-zero Picard group of a curve](../../../../../../degree-zero-picard-group-of-a-curve.md) uses tensor product as its group operation. The map is the [Abel map of a pointed smooth projective curve](../../../../../../abel-map-of-a-pointed-smooth-projective-curve.md). If $\alpha(p)=\alpha(q)$, then $\mathcal O(p-q)$ is trivial. By the divisor description of [line bundles](../../../../../../line-bundle.md), there is a nonzero [rational function](../../../../../../rational-function.md) $f$ with [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) $(f)=p-q$.

If $p\ne q$, this function has exactly one pole, of order one. It defines a nonconstant [morphism of algebraic varieties](../../../../../../morphism-of-algebraic-varieties.md) $X\to\mathbb P^1$: locally at a pole one uses $1/f$ as the target coordinate. The [degree of a morphism of curves](../../../../../../degree-of-a-morphism-of-curves.md) is the total pole degree, so it is one. The map is finite, since a nonconstant map of projective integral curves has finite fibers and is proper, and a degree-one finite map to the normal [projective line](../../../../../../projective-line.md) is an isomorphism. Algebraically, on a target affine chart the finite coordinate algebra lies inside the common function field and is integral over the integrally closed coordinate ring, so it equals that ring. Thus $X\cong\mathbb P^1$ and its genus is zero, contradicting $g\ge1$. Consequently

$$
\boxed{g\ge1\Longrightarrow\alpha\text{ is injective}.}
$$

This spells out why a [principal divisor with one simple zero and one simple pole](../../../../../../principal-divisor-with-one-simple-zero-and-one-simple-pole.md) cannot occur on a curve of positive genus.

If $g=0$, the chosen point $p_0$ is enough to identify $X$ with $\mathbb P^1$, even over a nonclosed field. By the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md), $h^0(\mathcal O(p_0))=2$, since the complementary canonical twist has degree $-3$ and no nonzero section. Besides constants there is a [rational function](../../../../../../rational-function.md) with its sole pole a simple pole at $p_0$, giving the same degree-one isomorphism. On $\mathbb P^1$, every degree-zero [divisor](../../../../../../divisor.md) is principal: over an algebraically closed field write a product of powers of linear forms for its finite point coefficients, with the degree-zero condition giving the coefficient at infinity. Over a general field the same construction uses irreducible polynomial factors for closed points, weighted by their degrees. Therefore

$$
\boxed{\operatorname{Pic}^0(X)=0\qquad(g=0).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
