<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Give $\overline K_{\mathfrak p}$ the unique extension of the absolute value of $K_{\mathfrak p}$. We use two standard facts: a complete non-Archimedean absolute value extends uniquely to every finite algebraic extension, and any two embeddings of a finite separable extension into an algebraic closure are conjugate by an automorphism of that algebraic closure.

A $K$-embedding $\tau:L\to\overline K_{\mathfrak p}$ pulls back this absolute value to a finite [place of a number field](../../../../../../place-of-a-number-field.md) on $L$ extending the given place of $K$. By the permitted equivalence of places and primes, it determines a [prime ideal](../../../../../../prime-ideal.md) $\mathfrak q_\tau$ above $\mathfrak p$. Every element of $\operatorname{Gal}(\overline K_{\mathfrak p}/K_{\mathfrak p})$ preserves the absolute value by uniqueness, so $\mathfrak q_\tau$ is constant on each orbit.

Every prime $\mathfrak q$ above $\mathfrak p$ occurs: its [completion of a number field at a prime ideal](../../../../../../completion-of-a-number-field-at-a-prime-ideal.md) $L_{\mathfrak q}$ is a finite extension of $K_{\mathfrak p}$ and admits a $K_{\mathfrak p}$-embedding into $\overline K_{\mathfrak p}$. Composing with $L\hookrightarrow L_{\mathfrak q}$ gives an embedding inducing $\mathfrak q$.

Conversely, suppose two embeddings induce the same prime. Their pulled-back absolute values have the same normalization on $K$, so they extend continuously to embeddings of the same field $L_{\mathfrak q}$. To see that their images are still inside the algebraic closure rather than only its completion, the closure of $\tau(L)$ is exactly the finite complete field $K_{\mathfrak p}\tau(L)$. The two resulting embeddings of $L_{\mathfrak q}$ are conjugate by the stated separable-extension fact. Restricting the conjugacy to $L$ proves that the original embeddings are in the same orbit. Thus the [prime ideals and local embedding orbits](../../../../../../prime-ideals-and-local-embedding-orbits.md) are naturally identified:

$$
\boxed{\{\mathfrak q\subset\mathcal O_L:\mathfrak q\mid\mathfrak p\}
\cong\operatorname{Gal}(\overline K_{\mathfrak p}/K_{\mathfrak p})\backslash
\operatorname{Hom}_K(L,\overline K_{\mathfrak p}).}
$$

If $L=K(\alpha)$, an embedding is determined by the image of $\alpha$, which may be any root of its [minimal polynomial](../../../../../../minimal-polynomial.md) $f$. The orbits on these roots are exactly the root sets of the monic irreducible factors of $f$ over $K_{\mathfrak p}$. Hence

$$
\boxed{\{\mathfrak q\mid\mathfrak p\}\cong
\{\text{monic irreducible factors of }f\text{ in }K_{\mathfrak p}[T]\}.}
$$

If $f_j$ corresponds to $\mathfrak q_j$, then $L_{\mathfrak q_j}\cong K_{\mathfrak p}[T]/(f_j)$ and $[L_{\mathfrak q_j}:K_{\mathfrak p}]=\deg f_j$. This is the [local factorization and extended absolute values](../../../../../../local-factorization-and-extended-absolute-values.md) correspondence and does not require an integral power basis.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
