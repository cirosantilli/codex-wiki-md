<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

All commutators of $H$ with $K$ lie in the central [subgroup](../../../../subgroup.md) $Y$ of $HK$. In the standard [commutator](../../../../commutator.md) identities, [conjugation](../../../../conjugation.md) by elements of $H$ or $K$ therefore acts trivially on these commutators. Since $Y$ is abelian, their order can also be reversed. Consequently

$$
[h_1h_2,k]=[h_1,k][h_2,k],\qquad
[h,k_1k_2]=[h,k_1][h,k_2].
$$

Thus the map is a [homomorphism](../../../../homomorphism.md) in each variable separately; this does not assert that it is a [homomorphism](../../../../homomorphism.md) from the direct product jointly.

It factors through $H/C_H(K)$ in the first variable and $K/C_K(H)$ in the second. If these finite [quotient](../../../../quotient.md) groups have representatives $h_1,\ldots,h_a$ and $k_1,\ldots,k_b$, then the finite collection $[h_i,k_j]$ generates $Y$. Let $e$ be an exponent of $H/C_H(K)$. For every $h,k$,

$$
[h,k]^e=[h^e,k]=1.
$$

Hence $Y$ is a finitely generated [abelian group](../../../../abelian-group.md) of bounded exponent, and **$Y$ is finite**. For instance its order is at most $e^{ab}$.

Now suppose $G$ is nilpotent and $G/\gamma_2(G)$ is finite. Induct on the [nilpotency class](../../../../nilpotency-class.md) $c$. For $c=1$, $G$ is its own [abelianization](../../../../abelianization.md) and is finite. If $c\ge2$, the [group](../../../../group-split.md) $\bar G=G/\gamma_c(G)$ has smaller class and

$$
\bar G/\gamma_2(\bar G)\cong G/\gamma_2(G),
$$

since $\gamma_c(G)\le\gamma_2(G)$. By induction $\bar G$ is finite. Apply the preceding result with $H=G=\gamma_1(G)$ and $K=\gamma_{c-1}(G)$. Their [commutator subgroup](../../../../commutator-subgroup.md) is $Y=\gamma_c(G)\le Z(G)$. Both relevant [centralizer](../../../../centralizer.md) quotients are finite, because their centralizers contain $\gamma_c(G)$ and $G/\gamma_c(G)$ is finite. Thus $\gamma_c(G)$ is finite. The extension of this finite [normal subgroup](../../../../normal-subgroup.md) by the finite [quotient](../../../../quotient.md) $\bar G$ is finite. The converse follows because a [quotient](../../../../quotient.md) of a [finite group](../../../../finite-group.md) is finite. Therefore

$$
\boxed{G\text{ finite}\iff G/\gamma_2(G)\text{ finite}\qquad(G\text{ nilpotent}).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the building infinite groups course of the University of Oxford](../../../split.md)
5. [Building infinite groups course of the University of Oxford](../../../../building-infinite-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
