<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose every component $\alpha_A$ is a [monomorphism](../../../../../../monomorphism.md) in the [Category of sets](../../../../../../category-of-sets.md), hence an [injective function](../../../../../../injective-function.md). If $\beta,\gamma:H\to F$ are [natural transformations](../../../../../../natural-transformation.md) with $\alpha\beta=\alpha\gamma$, then $\alpha_A\beta_A=\alpha_A\gamma_A$ at every object. Componentwise cancellation gives $\beta_A=\gamma_A$, so $\beta=\gamma$. Thus $\alpha$ is a [monomorphism](../../../../../../monomorphism.md) in the [functor category](../../../../../../functor-category.md).

Conversely, suppose $\alpha$ is a [monomorphism](../../../../../../monomorphism.md) and $x,y\in F(A)$ satisfy $\alpha_A(x)=\alpha_A(y)$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) supplies [natural transformations](../../../../../../natural-transformation.md) $\theta^x,\theta^y:Y(A)\to F$. Its [naturality](../../../../../../naturality.md) in $F$ identifies $\alpha\theta^x$ and $\alpha\theta^y$ with the equal elements $\alpha_A(x)$ and $\alpha_A(y)$. Cancellation by $\alpha$ gives $\theta^x=\theta^y$; evaluating at $1_A$ gives $x=y$. Therefore **a [natural transformation](../../../../../../natural-transformation.md) is a [monomorphism](../../../../../../monomorphism.md) exactly when all its components are [injective functions](../../../../../../injective-function.md)**. This is the [pointwise monomorphism in a set-valued functor category](../../../../../../pointwise-monomorphism-in-a-set-valued-functor-category.md) criterion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
