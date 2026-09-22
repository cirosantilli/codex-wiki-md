<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) says that every [central simple algebra](../../../../../central-simple-algebra.md) $A$ over $k$ has the form $M_r(D)$ for a finite-dimensional central division algebra $D$, uniquely up to the evident data. If $A$ and $B$ are central simple, extend scalars to an algebraic closure $\bar k$. Both become full matrix algebras, hence

$$
(A\otimes_kB)\otimes_k\bar k
\cong M_{ab}(\bar k)
$$

for suitable $a,b$. Any nonzero proper ideal of $A\otimes_kB$ would extend to one in this simple matrix algebra, and faithful flatness prevents it from vanishing or becoming the whole algebra. The same scalar-extension argument shows that the center is $k$. This proves the [tensor product of central simple algebras](../../../../../tensor-product-of-central-simple-algebras.md) theorem.

The [Brauer group](../../../../../brauer-group.md) $\operatorname{Br}(k)$ consists of [Morita equivalence](../../../../../morita-equivalence.md) classes of central simple $k$-algebras. Its product is $[A][B]=[A\otimes_kB]$, its identity is $[k]$, and $[A]^{-1}=[A^{\mathrm{op}}]$ because $A\otimes_kA^{\mathrm{op}}\cong\operatorname{End}_k(A)$ is a full matrix algebra.

Let $L/k$ be a [Finite Galois extension](../../../../../finite-galois-extension.md) with [Galois group](../../../../../galois-group.md) $G_L$, and let $\phi:G_L\times G_L\to L^\times$ be a [normalized two-cocycle](../../../../../normalized-two-cocycle.md). The [crossed-product algebra of a Galois extension](../../../../../crossed-product-algebra-of-a-galois-extension.md) has underlying left $L$-vector space

$$
A(L,G_L,\phi)=\bigoplus_{\sigma\in G_L}Lu_\sigma
$$

and multiplication

$$
u_\sigma a=\sigma(a)u_\sigma,
\qquad
u_\sigma u_\tau=\phi(\sigma,\tau)u_{\sigma\tau}.
$$

The cocycle identity is exactly associativity. After scalar extension to $L$, the algebra acts by the twisted regular representation and becomes $M_{|G_L|}(L)$; Galois descent shows that it is central simple over $k$. If $\phi$ is multiplied by the coboundary of a one-cochain $b_\sigma$, rescaling $u_\sigma$ by $b_\sigma$ gives an isomorphic algebra. Hence the [cohomological construction of a Brauer class](../../../../../cohomological-construction-of-a-brauer-class.md) gives a well-defined map

$$
H^2(G_L,L^\times)\longrightarrow\operatorname{Br}(k).
$$

It remains to show that every Brauer class is torsion. For a finite group $G$, restriction and corestriction on normalized bar cochains satisfy

$$
\operatorname{cor}\circ\operatorname{res}
=\sum_{g\in G}g^*=|G|
$$

on cohomology: the first equality follows by summing the translated cochain over coset representatives, and each $g^*$ is the identity because an inner automorphism is cochain-homotopic to the identity. Restriction to the trivial subgroup is zero in positive degree, so this proves that [finite-group cohomology is annihilated by the group order](../../../../../finite-group-cohomology-is-annihilated-by-the-group-order.md). In multiplicative notation, every $\alpha\in H^2(G_L,L^\times)$ therefore satisfies $\alpha^{|G_L|}=1$.

By the permitted assumption, $[A]$ is the image of such an $\alpha$ for some $L$. Consequently $[A]^{|G_L|}=1$ in $\operatorname{Br}(k)$. By the definition of Brauer equivalence, this says that for some $n$,

$$
A^{\otimes|G_L|}\cong M_n(k),
$$

as required.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
