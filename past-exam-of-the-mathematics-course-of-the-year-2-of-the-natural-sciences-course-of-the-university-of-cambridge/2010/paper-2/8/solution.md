<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The [order of a finite group](../../../../order-of-a-finite-group.md) $G$ is its number of elements. [Lagrange's theorem](../../../../lagrange-s-theorem.md) states that for a [subgroup](../../../../subgroup.md) $K\leq G$,

$$
|G|=[G:K]|K|,
$$

so $|K|$ divides $|G|$. In particular the [order of a group element](../../../../order-of-a-group-element.md) divides $|G|$, because it is the order of its generated [cyclic subgroup](../../../../cyclic-subgroup.md).

For $|G|=4$, if some element has order four it generates the whole group, which is therefore the [cyclic group](../../../../cyclic-group.md) $C_4$. Otherwise every nonidentity element has order two. Choose two distinct ones $a,b$ and put $c=ab$. Cancellation shows $c\notin\{e,a,b\}$, so $c$ is the remaining element. Since $c^{-1}=c$,

$$
ab=c=c^{-1}=(ab)^{-1}=b^{-1}a^{-1}=ba.
$$

The other products follow: $ac=ca=b$, $bc=cb=a$, and $a^2=b^2=c^2=e$. Thus the second possibility is the [Klein four-group](../../../../klein-four-group.md). The two groups are not [isomorphic](../../../../isomorphism.md) because only $C_4$ has an element of order four. This proves the order-four case of the [classification of groups of order p squared](../../../../classification-of-groups-of-order-p-squared.md).

A [group homomorphism](../../../../group-homomorphism.md) $\Phi:G\to H$ obeys $\Phi(gh)=\Phi(g)\Phi(h)$. It maps identity to identity and inverses to inverses. Its [group kernel](../../../../kernel-of-a-group-homomorphism.md) $K=\{g:\Phi(g)=e_H\}$ contains $e_G$ and is closed under $ab^{-1}$, so the [subgroup test](../../../../subgroup-test.md) makes it a subgroup. For $k\in K$ and $g\in G$,

$$
\Phi(gkg^{-1})=\Phi(g)e_H\Phi(g)^{-1}=e_H.
$$

Thus $gKg^{-1}\subseteq K$; applying the same argument to $g^{-1}$ gives equality. Hence $K$ is a [normal subgroup](../../../../normal-subgroup.md).

Define $\overline\Phi:G/K\to H$ by $\overline\Phi(gK)=\Phi(g)$. If $gK=hK$, then $h^{-1}g\in K$, giving $\Phi(g)=\Phi(h)$, so this is well-defined. Coset multiplication shows it is a [group homomorphism](../../../../group-homomorphism.md). Its kernel is just the identity coset, since $\Phi(g)=e_H$ means $g\in K$. It is therefore injective, and the assumed surjectivity of $\Phi$ makes it surjective as well. This proves the [first isomorphism theorem](../../../../first-isomorphism-theorem.md) here:

$$
\boxed{G/K\cong H.}
$$

In the [quaternion group](../../../../quaternion-group.md), the element $-1=i^2=j^2=k^2$ commutes with each of $i,j,k$, because an element commutes with its square. It then commutes with their negatives too, and with $\pm1$. The set $N=\{1,-1\}$ is a subgroup because $(-1)^2=1$, and it is central, hence a [normal subgroup](../../../../normal-subgroup.md).

The four quotient [cosets](../../../../coset.md) are $N,iN,jN,kN$. They square to $N$, and $(iN)(jN)=kN$. Reversed products have the same coset: for example $(ij)^{-1}=k^{-1}=-k$, while $j^{-1}i^{-1}=(-j)(-i)=ji$, so $ji=-k$. The same calculation gives $kj=-i$ and $ik=-j$. After signs are identified, these are precisely the products in the [Klein four-group](../../../../klein-four-group.md). Define

$$
\boxed{\Phi(\pm1)=e,\qquad\Phi(\pm i)=a,\qquad\Phi(\pm j)=b,\qquad\Phi(\pm k)=c.}
$$

This preserves all products, is surjective, and has kernel exactly $N$. The [first isomorphism theorem](../../../../first-isomorphism-theorem.md) therefore gives

$$
\boxed{Q_8/\{\pm1\}\cong V.}
$$

This is the [quaternion group modulo its centre](../../../../quaternion-group-modulo-its-centre.md): the reverse-product relations also show that none of $\pm i,\pm j,\pm k$ is central, so $Z(Q_8)=N$.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
