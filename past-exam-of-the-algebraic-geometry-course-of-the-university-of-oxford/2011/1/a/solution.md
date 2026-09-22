<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [affine variety](../../../../affine-algebraic-set.md) in $\mathbb A_k^n$ is the common [zero set](../../../../zero-set.md) of a collection of [polynomials](../../../../polynomial-split.md) in $k[x_1,\ldots,x_n]$, with its [Zariski topology](../../../../zariski-topology.md). We use the convention of this question that such a [variety](../../../../algebraic-variety-split.md) need not be [irreducible](../../../../irreducible-topological-space.md). Its [vanishing ideal](../../../../vanishing-ideal.md) and [coordinate ring](../../../../coordinate-ring.md) are

$$
\boxed{I(X)=\{f:f(p)=0\text{ for every }p\in X\},\qquad A(X)=k[x_1,\ldots,x_n]/I(X).}
$$

The quotient identifies [polynomials](../../../../polynomial-split.md) that give the same function on $X$, so its elements are exactly [polynomial functions](../../../../polynomial-function.md) on $X$.

For affine embeddings $X\subseteq\mathbb A^n$ and $Y\subseteq\mathbb A^m$, a [morphism of affine varieties](../../../../morphism-of-affine-varieties.md) is a map $F=(f_1,\ldots,f_m)$ with $f_i\in A(X)$ and [image](../../../../image-of-a-function.md) in $Y$. [Pullback](../../../../pullback-category-theory.md) of [polynomial functions](../../../../polynomial-function.md) defines the contravariant [homomorphism](../../../../homomorphism.md)

$$
\boxed{F^\#:A(Y)\longrightarrow A(X),\qquad [g]\longmapsto g\circ F.}
$$

It is well defined because any [polynomial](../../../../polynomial-split.md) vanishing on $Y$ pulls back to zero on $X$, and it preserves addition, multiplication, one, and the constants in $k$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
