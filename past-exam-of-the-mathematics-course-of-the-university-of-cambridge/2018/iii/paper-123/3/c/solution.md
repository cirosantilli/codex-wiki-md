<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We use the following standard facts about [cyclotomic fields](../../../../../../cyclotomic-field.md). For an odd prime $\ell$, the unique quadratic subfield of $\mathbb Q(\zeta_\ell)$ is

$$
\mathbb Q\left(\sqrt{(-1)^{(\ell-1)/2}\ell}\right).
$$

Also $\mathbb Q(\zeta_{\ell^r})$ has degree $\varphi(\ell^r)=\ell^{r-1}(\ell-1)$, and $\ell$ is totally ramified, with a unique prime and residue field $\mathbb F_\ell$. These are the [quadratic subfield of a prime cyclotomic field](../../../../../../quadratic-subfield-of-a-prime-cyclotomic-field.md) and [total ramification in a prime-power cyclotomic field](../../../../../../total-ramification-in-a-prime-power-cyclotomic-field.md) results.

Take

$$
E_r=\mathbb Q(\zeta_{59^r})\quad(r\geq1).
$$

Since $59\equiv3\pmod4$, every $E_r$ contains $K=\mathbb Q(\sqrt{-59})$, through its subfield $E_1$. The unique prime above $59$ is totally ramified in $E_r/K$: the absolute ramification index is $58\cdot59^{r-1}$, the index in $K/\mathbb Q$ is $2$, and the relative index is therefore

$$
e(E_r/K)=29\cdot59^{r-1}=[E_r:K].
$$

The field $K$ has no real places. By part (b), $h_K\mid h_{E_r}$, and part (a) showed $3\mid h_K$. Thus

$$
\boxed{3\mid h_{E_r}\quad\text{for every }r\geq1.}
$$

The [ring of integers of a number field](../../../../../../ring-of-integers.md) is a [Dedekind domain](../../../../../../dedekind-domain.md), and is a [principal ideal domain](../../../../../../principal-ideal-domain.md) exactly when its [ideal class group](../../../../../../ideal-class-group.md) is trivial. Hence none of these rings of integers is principal. Finally the degrees $58\cdot59^{r-1}$ strictly increase, so the fields are pairwise distinct. The explicit infinite family of [nonprincipal cyclotomic fields of conductor a prime power](../../../../../../nonprincipal-cyclotomic-fields-of-conductor-a-prime-power.md) is

$$
\boxed{\mathbb Q(\zeta_{59}),\ \mathbb Q(\zeta_{59^2}),\ \mathbb Q(\zeta_{59^3}),\ldots.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
