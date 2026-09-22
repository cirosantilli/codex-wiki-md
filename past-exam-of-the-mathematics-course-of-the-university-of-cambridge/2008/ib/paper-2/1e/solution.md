<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

A [linear map](../../../../../linear-map.md) preserves [linear combinations](../../../../../linear-combination.md): $\psi(av+bw)=a\psi(v)+b\psi(w)$ for all vectors and real scalars. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives $\dim V=\dim\ker\psi+\dim\operatorname{im}\psi$. For an endomorphism of the same finite-dimensional [vector space](../../../../../vector-space-split.md), surjectivity means rank $\dim V$, equivalent to zero kernel and hence injectivity.

If $\psi\phi=I$, then every $v=\psi(\phi v)$ lies in the image, so $\psi$ is surjective and consequently injective. Now $\psi(\phi\psi v)=\psi v$; injectivity implies $\phi\psi v=v$ for every $v$. Thus **the right inverse is also a left inverse:** $\boxed{\phi\psi=I}$. This is the [one-sided inverses of finite-dimensional endomorphisms](../../../../../one-sided-inverses-of-finite-dimensional-endomorphisms.md) property.

Apply it to the [linear maps](../../../../../linear-map.md) on $\mathbb R^n$ represented by $A$ and $B$: $AB=I$ implies $\boxed{BA=I}$. Equal finite dimensions are essential to the argument.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
