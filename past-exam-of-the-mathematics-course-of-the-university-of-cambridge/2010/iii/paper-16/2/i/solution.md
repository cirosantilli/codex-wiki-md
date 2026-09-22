<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [finite morphism](../../../../../../finite-morphism.md) is a [finite type morphism](../../../../../../morphism-of-finite-type.md). It is also a [separated morphism](../../../../../../separated-morphism.md): on an [affine scheme](../../../../../../affine-scheme.md) chart $\operatorname{Spec}B\to\operatorname{Spec}A$, its [diagonal morphism](../../../../../../diagonal-morphism.md) is represented by the surjective multiplication [ring homomorphism](../../../../../../ring-homomorphism.md) $B\otimes_AB\to B$, and is therefore a [closed immersion](../../../../../../closed-immersion.md) by Question 1.

We prove the lifting condition in the [valuative criterion for properness](../../../../../../valuative-criterion-for-properness.md). Choose an [affine open subset](../../../../../../affine-open-subscheme.md) of $Y$ containing the image of the closed point of $\operatorname{Spec}V$. Every point of $\operatorname{Spec}V$ is a generalization of its closed point, so the whole map factors through this [affine open subset](../../../../../../affine-open-subscheme.md). Its inverse image under the [finite morphism](../../../../../../finite-morphism.md) is $\operatorname{Spec}B$, with $B$ a finitely generated $A$-[module](../../../../../../module-mathematics.md). Every $b\in B$ is integral over $A$: apply the [determinant trick](../../../../../../determinant-trick.md) to multiplication by $b$ on a finite set of [module](../../../../../../module-mathematics.md) generators to obtain a monic polynomial which annihilates all generators and hence annihilates $1$.

In the given valuative square, we have compatible [ring homomorphisms](../../../../../../ring-homomorphism.md) $A\to V$ and $B\to K$. The image in $K$ of each $b\in B$ satisfies a monic polynomial over $V$. To see directly why it belongs to $V$, suppose $x\in K\setminus V$. The defining property of a [valuation ring](../../../../../../valuation-ring.md) gives $x^{-1}\in V$, and it lies in the [maximal ideal](../../../../../../maximal-ideal.md) since it cannot be a unit. A monic equation for $x$, multiplied by $x^{-n}$, would then express $1$ as a sum of elements in that [maximal ideal](../../../../../../maximal-ideal.md), a contradiction. This proves that [valuation rings are integrally closed](../../../../../../valuation-rings-are-integrally-closed.md) and that $B\to K$ factors through $B\to V$. The factorization is unique because $V\hookrightarrow K$ is injective. Thus the lift exists uniquely, proving

$$
\boxed{\text{finite morphisms are proper}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
