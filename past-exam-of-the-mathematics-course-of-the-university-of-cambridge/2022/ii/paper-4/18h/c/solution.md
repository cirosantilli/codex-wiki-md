<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take

$$
G=C_p\times C_{p-1}\cong C_{p(p-1)}
$$

and let $N=C_p\times\{1\}$. Take

$$
G'=\operatorname{AGL}_1(\mathbb F_p)
=\mathbb F_p\rtimes\mathbb F_p^\times,
$$

the [affine group over a finite field](../../../../../../affine-group-over-a-finite-field.md), and let $N'$ be its translation subgroup. Both normal subgroups have order $p$, and

$$
G/N\cong C_{p-1}\cong G'/N'.
$$

The groups are not isomorphic: $G$ is abelian, while $G'$ is nonabelian.

For $p=3$, let

$$
L=\mathbb Q(\zeta_7).
$$

Then $\operatorname{Gal}(L/\mathbb Q)\cong C_6=G$. The fixed field of its subgroup $N$ of order three is its unique quadratic subfield,

$$
\boxed{L^N=\mathbb Q(\sqrt{-7})}.
$$

Let

$$
L'=\mathbb Q(\sqrt[3]{2},\zeta_3),
$$

the [splitting field](../../../../../../splitting-field.md) of $X^3-2$. Its Galois group is $S_3\cong\operatorname{AGL}_1(\mathbb F_3)=G'$. The normal subgroup $N'=A_3$ fixes the quadratic discriminant field, so

$$
\boxed{(L')^{N'}=\mathbb Q(\sqrt{-3})=\mathbb Q(\zeta_3)}.
$$

Now let $p>3$. Part (a), with $r=p(p-1)$, supplies a cyclic Galois extension with group $G$. For $G'$, take the splitting field

$$
L'=\mathbb Q(\zeta_p,2^{1/p})
$$

of $X^p-2$. The prime $2$ is unramified in $\mathbb Q(\zeta_p)$, so at every prime ideal above $2$ its valuation is one. It cannot therefore be a $p$th power in the cyclotomic field. Hence

$$
[L':\mathbb Q(\zeta_p)]=p,
\qquad
[L':\mathbb Q]=p(p-1).
$$

The automorphisms

$$
\sigma(2^{1/p})=\zeta_p2^{1/p},
\quad \sigma(\zeta_p)=\zeta_p,
$$

and, for $a\in\mathbb F_p^\times$,

$$
\tau_a(2^{1/p})=2^{1/p},
\quad \tau_a(\zeta_p)=\zeta_p^a
$$

satisfy

$$
\tau_a\sigma\tau_a^{-1}=\sigma^a.
$$

They generate all $p(p-1)$ automorphisms, proving

$$
\boxed{
\operatorname{Gal}(L'/\mathbb Q)
\cong C_p\rtimes\mathbb F_p^\times
\cong\operatorname{AGL}_1(\mathbb F_p)=G'
}.
$$

This is the [affine Galois group of the splitting field of x to the p minus two](../../../../../../affine-galois-group-of-the-splitting-field-of-x-to-the-p-minus-two.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
