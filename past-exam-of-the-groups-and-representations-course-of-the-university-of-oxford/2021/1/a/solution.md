<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T(v\otimes w)=w\otimes v$ on the [tensor product](../../../../tensor-product.md) $V\otimes V$. The [linear map](../../../../linear-map.md) $R(g)\otimes R(g)$ commutes with $T$, so preserves its $+1$ and $-1$ [eigenspaces](../../../../eigenspace.md), namely the [symmetric square](../../../../symmetric-square.md) $S^2V$ and the [exterior square](../../../../exterior-square.md) $\wedge^2V$. Restricting the [tensor product representation](../../../../tensor-product-of-group-representations.md) to these [invariant subspaces](../../../../invariant-subspace.md) defines $S^2R$ and $\wedge^2R$. The [representation](../../../../group-representation.md) identity follows by restricting $(R(g)\otimes R(g))(R(h)\otimes R(h))=R(gh)\otimes R(gh)$.

For a [finite group](../../../../finite-group.md), $g$ has finite order $m$, so $R(g)^m=I$. Over the [complex numbers](../../../../complex-number.md), the [polynomial](../../../../polynomial-split.md) $t^m-1$ has distinct roots; hence $R(g)$ is [diagonalizable](../../../../diagonalizable-matrix.md). Choose an [eigenbasis](../../../../eigenbasis.md) $v_1,\ldots,v_n$ with [eigenvalues](../../../../eigenvalue.md) $\lambda_1,\ldots,\lambda_n$. A [basis](../../../../basis.md) of the [symmetric square](../../../../symmetric-square.md) consists of $v_i\otimes v_i$ and $v_i\otimes v_j+v_j\otimes v_i$ for $i<j$. A [basis](../../../../basis.md) of the [exterior square](../../../../exterior-square.md) consists of $v_i\otimes v_j-v_j\otimes v_i$ for $i<j$. Their [eigenvalues](../../../../eigenvalue.md) are respectively $\lambda_i^2,\lambda_i\lambda_j$ and $\lambda_i\lambda_j$. Taking [traces](../../../../matrix-trace.md),

$$
\chi_{S^2R}(g)=\sum_i\lambda_i^2+\sum_{i<j}\lambda_i\lambda_j,
\qquad \chi_{\wedge^2R}(g)=\sum_{i<j}\lambda_i\lambda_j.
$$

But $\chi(g)^2=\sum_i\lambda_i^2+2\sum_{i<j}\lambda_i\lambda_j$ and $\chi(g^2)=\sum_i\lambda_i^2$. Thus the [characters](../../../../character-of-a-representation.md) are

$$
\boxed{\chi_{S^2R}(g)=\tfrac12[\chi(g)^2+\chi(g^2)],\qquad
\chi_{\wedge^2R}(g)=\tfrac12[\chi(g)^2-\chi(g^2)].}
$$

At $g=e$, these also give the [dimensions](../../../../dimension-vector-space.md) $n(n+1)/2$ and $n(n-1)/2$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
