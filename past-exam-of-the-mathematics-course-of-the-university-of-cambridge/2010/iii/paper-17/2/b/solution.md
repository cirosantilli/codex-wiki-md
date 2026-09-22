<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each [prime number](../../../../../../prime-number.md) $p$, reduction of the [mapping cone](../../../../../../mapping-cone-homological-algebra.md) is the [mapping cone](../../../../../../mapping-cone-homological-algebra.md) of the reduced [chain map](../../../../../../chain-map.md). Part (a), whose proof works over any coefficient ring, therefore gives

$$
H_i(M\otimes\mathbb F_p)=0\qquad\text{for every }i,p.
$$

Every $M_i$ is a finitely generated [free abelian group](../../../../../../free-abelian-group.md). Multiplication by $p$ consequently gives a [short exact sequence of chain complexes](../../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow M\xrightarrow{p}M\longrightarrow M\otimes\mathbb F_p\longrightarrow0.
$$

The neighboring terms $H_{i+1}(M\otimes\mathbb F_p)$ and $H_i(M\otimes\mathbb F_p)$ in its [long exact sequence in homology](../../../../../../long-exact-sequence-in-homology.md) both vanish. Thus multiplication by $p$ on $H_i(M)$ is an [isomorphism](../../../../../../isomorphism.md) for every [prime number](../../../../../../prime-number.md) $p$.

The group $H_i(M)$ is a [finitely generated abelian group](../../../../../../finitely-generated-abelian-group.md), since it is a quotient of a subgroup of $M_i$. Write it, using the [Fundamental theorem of finitely generated abelian groups](../../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md), as

$$
H_i(M)\cong\mathbb Z^{b_i}\oplus T_i,
$$

with $T_i$ finite. If $b_i>0$, multiplication by any [prime number](../../../../../../prime-number.md) is not surjective. If $T_i\ne0$, choose a [prime number](../../../../../../prime-number.md) dividing its order; multiplication by that prime is not injective. Both contradict the preceding [isomorphism](../../../../../../isomorphism.md). Hence $H_i(M)=0$ for every $i$.

Applying part (a) integrally now proves the stronger natural conclusion

$$
\boxed{f_*:H_i(C;\mathbb Z)\xrightarrow{\ \cong\ }H_i(D;\mathbb Z)\quad\text{for every }i.}
$$

This is [prime coefficient detection of quasi-isomorphisms](../../../../../../prime-coefficient-detection-of-quasi-isomorphisms.md). The finite-generation hypothesis is used precisely when excluding nonzero groups on which every prime acts invertibly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
