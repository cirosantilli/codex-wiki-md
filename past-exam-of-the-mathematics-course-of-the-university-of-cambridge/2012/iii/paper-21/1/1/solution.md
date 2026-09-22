<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $d=\deg A$ for the [degree of a central simple algebra](../../../../../../degree-of-a-central-simple-algebra.md), so $\dim_KA=d^2$. Choose a finite Galois [splitting field of a central simple algebra](../../../../../../splitting-field-of-a-central-simple-algebra.md) $E/K$ for $A$ and an isomorphism $\phi:A\otimes_KE\to M_d(E)$. The [reduced norm](../../../../../../reduced-norm.md) is

$$
\operatorname{Nrd}_{A/K}(a)=\det\phi(a\otimes1).
$$

The existence of a finite separable splitting field is a standard structural property of a [central simple algebra](../../../../../../central-simple-algebra.md); passing to its Galois closure supplies $E$.

Every $E$-algebra automorphism of $M_d(E)$ is inner. Here is the matrix-unit argument for the [inner automorphisms of a matrix algebra](../../../../../../inner-automorphisms-of-a-matrix-algebra.md) result. For an automorphism $h$, choose $w\ne0$ in the image of $h(E_{11})$, and set $w_i=h(E_{i1})w$. Then $h(E_{ij})w_k=\delta_{jk}w_i$. The $w_i$ are nonzero and independent, and their number is $d$, so they form a basis. Relative to that basis $h$ acts on each matrix unit in the usual way. Thus $h(T)=PTP^{-1}$ for some $P\in\operatorname{GL}_d(E)$. [Determinants](../../../../../../determinant.md) are unchanged by conjugation, proving independence of $\phi$.

For $\sigma\in\operatorname{Gal}(E/K)$, compare $\phi$ with the isomorphism obtained by applying $\sigma$ to matrix entries and $\sigma^{-1}$ to the scalar factor of $A\otimes E$. Their difference is again inner. For $a\in A$, this shows $\sigma(\det\phi(a))=\det\phi(a)$. The [determinant](../../../../../../determinant.md) therefore belongs to $K$. In fact, for a $K$-basis $a_1,\ldots,a_{d^2}$, the same comparison shows that all coefficients of

$$
\det\left(\sum_iX_i\phi(a_i)\right)
$$

are fixed by the [Galois group](../../../../../../galois-group.md), so the [reduced norm](../../../../../../reduced-norm.md) is a [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) of degree $d$ over $K$. This coefficient argument also applies over [finite fields](../../../../../../finite-field.md), where equality merely as functions would not identify polynomials.

Finally, two finite splitting fields embed into a common finite splitting extension. [Determinant](../../../../../../determinant.md) commutes with scalar extension, and over that common extension the two matrix identifications differ by an inner automorphism. Hence the resulting polynomials agree over $K$. **The [reduced norm](../../../../../../reduced-norm.md) is independent of both the splitting field and the matrix identification.** It is multiplicative, and $\operatorname{Nrd}(a)=0$ exactly when $a$ is not invertible: a matrix with nonzero [determinant](../../../../../../determinant.md) is invertible after scalar extension, and invertibility descends by the invertibility of the $K$-linear multiplication map. In a [division algebra](../../../../../../division-algebra.md) the only element of [reduced norm](../../../../../../reduced-norm.md) zero is zero.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
