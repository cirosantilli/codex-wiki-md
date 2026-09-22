# Orthogonal transformation in a nonorthonormal basis

↑ **Parent:** [Orthogonal transformation](orthogonal-transformation.md)

Let $b_1,\ldots,b_n$ be an arbitrary [basis](basis.md) of a real [inner product space](inner-product-space.md), with [Gram matrix](gram-matrix.md) $G=(\langle b_i,b_j\rangle)$. If a [linear map](linear-map.md) $T$ has [matrix](matrix.md) $A$ in this [basis](basis.md), then

$$
\langle Tu,Tv\rangle=[u]^TA^TGA[v],\qquad
\langle u,v\rangle=[u]^TG[v].
$$

Consequently $T$ is an [orthogonal transformation](orthogonal-transformation.md) exactly when $A^TGA=G$. The simpler [orthogonal matrix](orthogonal-matrix.md) condition $A^TA=I$ applies directly when the chosen [basis](basis.md) is an [orthonormal basis](orthonormal-basis.md), so that $G=I$.

For example, take a two-dimensional [vector space](vector-space-split.md) with [weighted Euclidean inner product](weighted-euclidean-inner-product.md) having $G=\operatorname{diag}(1,4)$. Then

$$
A=\begin{pmatrix}0&2\\-1/2&0\end{pmatrix}
$$

satisfies $A^TGA=G$, but $A^TA=\operatorname{diag}(1/4,4)\ne I$. Thus it represents an [orthogonal transformation](orthogonal-transformation.md) even though it is not an [orthogonal matrix](orthogonal-matrix.md).

## ↑ Ancestors (8)

1. [Orthogonal transformation](orthogonal-transformation.md)
2. [Orthogonal matrix](orthogonal-matrix.md)
3. [Orthogonal group](orthogonal-group.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/4/c/iii/solution.md)
