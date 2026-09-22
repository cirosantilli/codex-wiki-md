<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Hilbert class field](../../../../../../hilbert-class-field.md) theorem stated in part (a), and let $H_L$ be the Hilbert class field of $L$. Put $F=M\cap H_L$ inside a common algebraic closure.

Any intermediate extension of $M/L$ is totally ramified at the given prime. To verify this even when $M/L$ is not Galois, there is a unique prime of $F$ above $\mathfrak p$, its residue field embeds into the residue field at the unique prime of $M$ and therefore equals $k_{\mathfrak p}$, and the [fundamental identity for prime decomposition](../../../../../../fundamental-identity-for-prime-decomposition.md) gives ramification index $[F:L]$. On the other hand $F/L$ is a subextension of $H_L/L$, so it is unramified there. Its ramification index is consequently both $[F:L]$ and $1$, forcing

$$
\boxed{M\cap H_L=L.}
$$

Because $H_L/L$ is Galois, this intersection identity gives

$$
[MH_L:M]=[H_L:L]=h_L,\qquad
\operatorname{Gal}(MH_L/M)\cong\operatorname{Gal}(H_L/L).
$$

Thus $MH_L/M$ is abelian. We use the standard local fact that unramified extensions remain unramified under finite base extension: after base change each factor is obtained by lifting an extension of the residue field. Since $H_L/L$ is unramified at every finite prime, $MH_L/M$ is also unramified at every finite prime. There are no real places of $M$, since every embedding of $M$ restricts to an embedding of the totally imaginary field $L$. Hence there is no infinite-place obstruction.

The maximality of $H_M$ now implies $MH_L\subseteq H_M$. Taking degrees over $M$ proves the [class number divisibility under total ramification](../../../../../../class-number-divisibility-under-total-ramification.md):

$$
\boxed{h_L=[MH_L:M]\mid[H_M:M]=h_M.}
$$

The argument uses the degree of an unramified class-field extension, and does not assume that extension of ideals induces an injection of [ideal class groups](../../../../../../ideal-class-group.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
