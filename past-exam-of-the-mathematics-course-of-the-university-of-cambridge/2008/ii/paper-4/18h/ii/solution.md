<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For odd prime $n$, every subgroup is one of $\{1\}$, $\langle\sigma\rangle$, a reflection subgroup $H_j=\langle\sigma^j\tau\rangle$ for $0\leq j<n$, or $G$. Indeed, a subgroup containing a nonidentity rotation contains all rotations; with any reflection it is then $G$. A subgroup with no nonidentity rotation contains at most one reflection, since the product of distinct reflections is a nonidentity rotation.

The [Galois correspondence](../../../../../../galois-correspondence.md) gives the following fixed fields. The trivial subgroup corresponds to $L=\mathbb C(z)$, the rotation subgroup to $\mathbb C(z^n)$, and $G$ to the base $\mathbb C(w)$. Since composition of the stated automorphisms gives $(\sigma^j\tau)(z)=\zeta_n^{-j}/z$, the reflection subgroup corresponds to

$$
\boxed{L^{H_j}=\mathbb C(z+\zeta_n^{-j}/z).}
$$

This rational invariant has degree two, hence generates the fixed field of its order-two subgroup, by the same degree argument as part (i). These fields have degrees respectively $2n,2,n,1$ over $\mathbb C(w)$.

An intermediate field is [Galois](../../../../../../finite-galois-extension.md) over the base exactly when its corresponding subgroup is normal in $G$. The trivial subgroup, the rotations and $G$ are normal; no reflection subgroup is normal because $n$ is odd and greater than two. Hence the Galois intermediate extensions and groups are

$$
\boxed{\operatorname{Gal}(L/\mathbb C(w))=G,\quad
\operatorname{Gal}(\mathbb C(z^n)/\mathbb C(w))\cong C_2,\quad
\operatorname{Gal}(\mathbb C(w)/\mathbb C(w))=\{1\}.}
$$

The $n$ reflection fixed fields are not Galois over the base.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
