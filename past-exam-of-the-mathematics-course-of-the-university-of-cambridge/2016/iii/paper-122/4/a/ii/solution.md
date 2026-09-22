<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [braid group](../../../../../../../braid-group.md) $B_n$ has generators $\sigma_1,\ldots,\sigma_{n-1}$ and relations

$$
\sigma_i\sigma_j=\sigma_j\sigma_i\ (|i-j|>1),\qquad\sigma_i\sigma_{i+1}\sigma_i=\sigma_{i+1}\sigma_i\sigma_{i+1}.
$$

In the [strict monoidal category](../../../../../../../strict-monoidal-category.md) $\mathcal C$, put $X^{\otimes0}=I$ and send

$$
\boxed{n\longmapsto X^{\otimes n},\qquad\sigma_i\longmapsto1_X^{\otimes(i-1)}\otimes y\otimes1_X^{\otimes(n-i-1)}.}
$$

The images are invertible because the [Yang–Baxter operator](../../../../../../../yang-baxter-operator.md) $y$ is invertible. Distant images commute by the tensor interchange law, and adjacent images satisfy the [braid group relations](../../../../../../../braid-group-relations.md) by the [Yang–Baxter operator](../../../../../../../yang-baxter-operator.md) equation tensored with the remaining identities. Thus these assignments define [group homomorphisms](../../../../../../../group-homomorphism.md) $B_n\to\operatorname{Aut}(X^{\otimes n})$, and hence a [functor](../../../../../../../functor.md) $\mathbf B\to\mathcal C$.

Juxtaposition of braids puts generators into the corresponding two blocks of tensor factors, so their images are the tensor products of their images. Strictness of $\mathcal C$ gives $X^{\otimes(m+n)}=X^{\otimes m}\otimes X^{\otimes n}$ and $X^{\otimes0}=I$ exactly. **The resulting functor is strict monoidal and sends $1$ to $X$.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 122](../../../../paper-122-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
