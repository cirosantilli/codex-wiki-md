# Transpose of a linear map

↑ **Parent:** [Dual space](dual-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transpose_of_a_linear_map)

For a [linear map](linear-map.md) $T:V\to W$, the [dual map](transpose-of-a-linear-map.md) $T^*:W^*\to V^*$ sends a [linear functional](linear-functional.md) $\varphi$ on the output space to the input measurement $T^*(\varphi)=\varphi\circ T$. It reverses direction because a measurement of the output can be evaluated on an input by first applying $T$:

$$
(T^*\varphi)(v)=\varphi(Tv).
$$

For $T(x,y)=(x+y,2y)$ and $\varphi(u,v)=2u-v$, the input measurement is $T^*\varphi(x,y)=2(x+y)-2y=2x$. The output measurement ignores the part of this transformation contributed by $y$.

If $T$ has [matrix](matrix.md) $A$ in specified [bases](basis.md), a row representing $\varphi$ changes to $\ell A$. Storing the coefficients of a [linear functional](linear-functional.md) as a column in the corresponding [dual basis](dual-basis.md) gives $A^T\ell^T$, explaining why the [transpose of a linear map](transpose-of-a-linear-map.md) is represented by the [matrix transpose](transpose.md). This algebraic operation uses no [inner product](inner-product.md); it agrees with a matrix transpose even over the [complex numbers](complex-number.md), rather than automatically introducing [complex conjugation](complex-conjugation.md). The [adjoint operator](adjoint-operator.md) is defined using an [inner product](inner-product.md) and is a different construction. [Treil, Linear Algebra Done Wrong, §8.3: dual transformations and transpose](https://www.math.brown.edu/streil/papers/LADW/HTML_2026_04-30/Ch8.html).

In finite [dimension](dimension-vector-space.md), the [kernel](kernel-of-a-linear-map.md) and image of the [dual map](transpose-of-a-linear-map.md) are described by [annihilators of vector subspaces](annihilator-of-a-vector-subspace.md):

$$
\ker T^*=(\operatorname{im}T)^\circ,
\qquad
\operatorname{im}T^*=(\ker T)^\circ.
$$

**Table of contents**

- [Dual image and kernel annihilator identity](dual-image-and-kernel-annihilator-identity.md)
- [Equality of row rank and column rank](equality-of-row-rank-and-column-rank.md)
  - [Simultaneous basis exchange from a nonzero minor](simultaneous-basis-exchange-from-a-nonzero-minor.md)
- [Duals of a subspace and its quotient](duals-of-a-subspace-and-its-quotient.md)

## ↑ Ancestors (6)

1. [Dual space](dual-space.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Transpose of a linear map](transpose-of-a-linear-map.md)
