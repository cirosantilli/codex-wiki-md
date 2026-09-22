<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An object $E$ in a finite-product category is [exponentiable](../../../../../exponentiable-object.md) when $-\times E$ has a right adjoint $(-)^E$. The terminal object is exponentiable. If $E$ and $F$ are exponentiable, then

$$
-\times(E\times F)\cong(-\times E)\times F
$$

has the composite of their right adjoints as a right adjoint. Hence the [product of exponentiable objects is exponentiable](../../../../../product-of-exponentiable-objects-is-exponentiable.md), including the empty product.

Suppose $0$ is both initial and terminal. Since $-\times E$ is a left adjoint for exponentiable $E$, it preserves the initial object, so $0\times E\cong0$. Since $0$ is terminal, $0\times E\cong E$. Therefore the [zero object is the only exponentiable object in a pointed category](../../../../../zero-object-is-the-only-exponentiable-object-in-a-pointed-category.md).

Let $G=\mathbf{Top}(X,S)$ for a [T0 space](../../../../../kolmogorov-space.md) $X$ and the [Sierpiński space](../../../../../sierpinski-space.md) $S$. The evaluation map

$$
e:X\longrightarrow S^G,\qquad e(x)=(g(x))_{g\in G}
$$

is injective because characteristic maps of open sets distinguish distinct points. Every open $U\subseteq X$ equals $g_U^{-1}(1)$ for its characteristic map $g_U:X\to S$, so the subspace topology induced by $e$ is the original topology. This is the [Embedding of a T0 space into a power of the Sierpiński space](../../../../../embedding-of-a-t0-space-into-a-power-of-the-sierpinski-space.md).

A subspace inclusion between $T_0$ spaces is a [regular monomorphism](../../../../../regular-monomorphism.md), hence an [equalizer](../../../../../equaliser.md). Embedding its codomain into another power of $S$ and composing the parallel pair preserves the equalizer because the embedding is monic. Consequently

$$
X\longrightarrow S^G\rightrightarrows S^H
$$

is an equalizer for suitable sets $G,H$.

If $E$ is exponentiable, $\mathbf{Top}_0(-\times E,S)$ is represented by $S^E$. Conversely, suppose it is represented by $R$. Products give

$$
\mathbf{Top}_0(Y\times E,S^G)
\cong\mathbf{Top}_0(Y,R^G).
$$

Express any $T_0$ space $X$ as the displayed equalizer $S^G\rightrightarrows S^H$ and take the corresponding equalizer $R^G\rightrightarrows R^H$. Since hom-functors preserve limits, this equalizer represents $\mathbf{Top}_0(-\times E,X)$. Thus $-\times E$ has a right adjoint on every target, proving the [Exponentiability criterion in the category of T0 spaces](../../../../../exponentiability-criterion-in-the-category-of-t0-spaces.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
