<h1 id="1/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [diagonal operator on sequence space](../../../../../../../diagonal-operator-on-sequence-space.md),

$$
\|Ku\|_2^2=\sum_{j\geq1}\frac{|u_j|^2}{j^2}\leq\|u\|_2^2.
$$

Equality holds at the first coordinate vector, so $\|K\|=1$ and $K$ is a [bounded linear operator](../../../../../../../continuous-linear-operator.md). Every diagonal entry is nonzero, giving the [null space](../../../../../../../kernel-of-a-linear-map.md) $\mathcal N(K)=\{0\}$. A datum has a preimage exactly when its weighted coordinates belong to the [l2 sequence space](../../../../../../../l2-sequence-space.md). Hence

$$
\boxed{\mathcal R(K)=\left\{f\in\ell^2:\sum_{j\geq1}j^2|f_j|^2<\infty\right\},\qquad (K^\dagger f)_j=jf_j.}
$$

Finite sequences lie in the range and are dense in $\ell^2$, so $\mathcal R(K)^\perp=\{0\}$ and

$$
\boxed{\mathcal D(K^\dagger)=\mathcal R(K),\qquad\mathcal N(K)=\{0\}.}
$$

The [sequence](../../../../../../../sequence.md) $f^{(n)}=e_n/n$ converges to zero in the data [norm](../../../../../../../norm.md), but $K^\dagger f^{(n)}=e_n$ has [norm](../../../../../../../norm.md) one. Thus **$K^\dagger$ is unbounded and discontinuous**. In particular the dense range is not closed; the datum $f_j=1/j$ also proves that it is a proper subset of $\ell^2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
