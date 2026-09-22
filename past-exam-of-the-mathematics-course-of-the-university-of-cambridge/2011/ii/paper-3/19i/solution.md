<h1 id="19i/solution">Solution</h1>

↑ **Parent:** [19I](../19i.md)

For a character $\psi$ of a subgroup $H\leq G$, the [induced character](../../../../../induced-character.md) is

$$
(\operatorname{Ind}_H^G\psi)(g)=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}\psi(x^{-1}gx).
$$

It is the character of the [induced representation](../../../../../induced-representation.md) $\mathbb C[G]\otimes_{\mathbb C[H]}V_\psi$, and has degree $[G:H]\psi(1)$. The character inner product is $\langle\alpha,\beta\rangle_G=|G|^{-1}\sum_g\alpha(g)\overline{\beta(g)}$. Substituting the displayed formula and putting $g=xhx^{-1}$ yields

$$
\langle\operatorname{Ind}_H^G\psi,\chi\rangle_G=\frac1{|G||H|}\sum_{x\in G}\sum_{h\in H}\psi(h)\overline{\chi(xhx^{-1})}=\frac1{|H|}\sum_{h\in H}\psi(h)\overline{\chi(h)}.
$$

Thus [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) is

$$
\boxed{\langle\operatorname{Ind}_H^G\psi,\chi\rangle_G=\langle\psi,\operatorname{Res}_H^G\chi\rangle_H.}
$$

Now assume index two, so $H$ is normal. Choose $g\notin H$ and write $\psi^g(h)=\psi(g^{-1}hg)$. Directly from the induction formula,

$$
\operatorname{Res}_H^G\operatorname{Ind}_H^G\psi=\psi+\psi^g,\qquad \langle\operatorname{Ind}\psi,\operatorname{Ind}\psi\rangle_G=1+\langle\psi,\psi^g\rangle_H.
$$

If $\psi^g\ne\psi$, this norm is one, so induction is irreducible of degree $2d$: $\psi$ is monogamous. If $\psi^g=\psi$, the norm is two. Since a norm is the sum of squared nonnegative integer multiplicities, induction is the sum of two distinct irreducibles, each once. Each is related to $\psi$, so its degree is at least $d$ by restriction and reciprocity; their degrees sum to $2d$, forcing both to have degree $d$. Thus $\psi$ is bigamous.

Every irreducible $\chi$ of $G$ restricts to a nonzero sum of irreducibles. Choose a constituent $\psi$. If $\psi$ is bigamous, $\chi$ is one of its two degree-$d$ partners; since its restriction already contains a degree-$d$ constituent, $\operatorname{Res}\chi=\psi$. If $\psi$ is monogamous, $\chi=\operatorname{Ind}\psi$ and $\operatorname{Res}\chi=\psi+\psi^g$, giving precisely two distinct monogamous partners of equal degree.

The complex irreducible character degrees of $A_5$ are $1,3,3,4,5$, with squared sum $60$. Conjugation by the outside coset preserves degrees, so it fixes the unique degree-$1$, degree-$4$ and degree-$5$ characters and either fixes or swaps the two degree-$3$ characters. The two possibilities for $G$ are

$$
\boxed{1,1,3,3,3,3,4,4,5,5\quad\text{or}\quad1,1,4,4,5,5,6.}
$$

Both lists have squared sum $120=|G|$. They occur for $A_5\times C_2$ and $S_5$ respectively; in $S_5$, odd conjugation swaps the two classes of $5$-cycles and hence the two degree-$3$ characters.

## ↑ Ancestors (10)

1. [19I](../19i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
