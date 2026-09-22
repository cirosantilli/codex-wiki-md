<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For permutation characters, [Burnside lemma](../../../../../../burnside-s-lemma.md) on a product gives

$$
\langle\pi_k,\pi_l\rangle_G
=\#\bigl(G\backslash(X_k\times X_l)\bigr).
$$

Two pairs $(A,B)$ and $(A',B')$ lie in the same $S_n$-orbit exactly when

$$
|A\cap B|=|A'\cap B'|.
$$

When $0\leq l\leq k\leq n/2$, every value $0,1,\ldots,l$ is possible because $k+l\leq n$. Therefore the [symmetric-group subset permutation representation](../../../../../../symmetric-group-subset-permutation-representation.md) satisfies

$$
\boxed{\langle\pi_k,\pi_l\rangle_G=l+1.}
$$

For $1\leq r\leq n/2$, the [inclusion map between subset permutation modules](../../../../../../inclusion-map-between-subset-permutation-modules.md) embeds $\mathbb C[X_{r-1}]$ into $\mathbb C[X_r]$, so

$$
\chi_r=\pi_r-\pi_{r-1}
$$

is a character. Its norm is

$$
\begin{aligned}
\langle\chi_r,\chi_r\rangle
&=\langle\pi_r,\pi_r\rangle
-2\langle\pi_r,\pi_{r-1}\rangle
+\langle\pi_{r-1},\pi_{r-1}\rangle\\
&=(r+1)-2r+r=1.
\end{aligned}
$$

By [character orthogonality](../../../../../../character-orthogonality.md), $\chi_r$ is the character of an irreducible representation.

For $r>n/2$, complementation is an $S_n$-equivariant bijection $X_r\cong X_{n-r}$, so

$$
\pi_r=\pi_{n-r}.
$$

Consequently

$$
\pi_r-\pi_{r-1}
=-\bigl(\pi_{n-r+1}-\pi_{n-r}\bigr),
$$

the negative of one of the irreducible characters just found, and is not itself the character of a representation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
