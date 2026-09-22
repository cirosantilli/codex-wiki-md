<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Sunada theorem](../../../../../sunada-theorem.md) is the following. Let $X\to M_0$ be a finite normal [Riemannian covering](../../../../../riemannian-covering.md) of a connected closed [Riemannian manifold](../../../../../riemannian-manifold.md), with finite [deck transformation group](../../../../../deck-transformation-group.md) $T$. If $U_1,U_2\leq T$ satisfy [Gassmann equivalence](../../../../../gassmann-equivalence.md), meaning

$$
|U_1\cap C|=|U_2\cap C|\quad\text{for every conjugacy class }C\text{ of }T,
$$

then $U_1\backslash X$ and $U_2\backslash X$ have the same scalar [Laplacian spectrum](../../../../../laplacian-spectrum.md), with multiplicities. Equivalently, an epimorphism $\pi_1(M_0)\to T$ yields isospectral covers corresponding to the inverse images of $U_1,U_2$.

Here is the representation-theoretic proof. Every finite-dimensional [Laplacian eigenspace](../../../../../laplacian-eigenspace.md) $E_\lambda$ of $X$ is a [group representation](../../../../../group-representation.md) of $T$, since [isometries](../../../../../isometry.md) commute with the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md). Eigenfunctions on $U_i\backslash X$ identify with $E_\lambda^{U_i}$. Averaging gives the projection $P_i=|U_i|^{-1}\sum_{u\in U_i}u$, so

$$
\dim E_\lambda^{U_i}=\frac1{|U_i|}\sum_{u\in U_i}\chi_\lambda(u).
$$

The two subgroup orders agree, and the [character of a representation](../../../../../character-of-a-representation.md) $\chi_\lambda$ is constant on [conjugacy classes](../../../../../conjugacy-class.md). The displayed multiplicities are therefore equal for every $\lambda$. This proof also applies when $T$ has fixed points on $X$, provided the two subgroups $U_i$ act freely, so their quotients are smooth [manifolds](../../../../../topological-manifold.md). We shall use this extension for an orbifold base in Question 4.

The precise geometric test for an [isometry](../../../../../isometry.md) uses the full isometry group of a common [universal cover](../../../../../universal-cover.md). Equip the simply connected cover $\widetilde X$ of $M_0$ with the lifted metric and let $\Gamma_i$ be the subgroups of its [deck transformation group](../../../../../deck-transformation-group.md) corresponding to the two covers. Then

$$
\boxed{\Gamma_1\backslash\widetilde X\cong\Gamma_2\backslash\widetilde X\text{ isometrically}\iff
F\Gamma_1F^{-1}=\Gamma_2\text{ for some }F\in\operatorname{Isom}(\widetilde X).}
$$

Indeed, such an $F$ descends to an [isometry](../../../../../isometry.md) of the quotients. Conversely an [isometry](../../../../../isometry.md) of the quotients lifts to their simply connected covers; lift its inverse with compatible basepoints to see that the lift is bijective. Since it preserves the lifted metrics locally, it is a global [isometry](../../../../../isometry.md), and equivariance of the covering maps shows that it conjugates the deck subgroups. This proves the criterion, rather than assuming that an isometry must preserve the map to $M_0$. In particular, nonconjugacy inside $T$ alone does not establish nonisometry; the full covering space may have additional isometries. Nonisomorphic [fundamental groups](../../../../../fundamental-group.md) are a sufficient topological obstruction, and length-identified geometric configurations provide another.

For a concrete [nonisomorphic Gassmann equivalent regular subgroups](../../../../../nonisomorphic-gassmann-equivalent-regular-subgroups.md) example, fix an odd prime $p$ and take $T=S_{p^3}$. Embed $E=(C_p)^3$ and $B=\operatorname{UT}_3(\mathbb F_p)$ through their regular permutation actions. Both have order $p^3$. Every nonidentity element of $E$ has order $p$. For $B$, write its elements as $I+N$ with $N^3=0$; then

$$
(I+N)^p=I+pN+\binom p2N^2=I
$$

over $\mathbb F_p$, including $p=3$, so its nonidentity elements also have order $p$. In a regular action, each nonidentity order-$p$ element has cycle type $p^{p^2}$. Thus each subgroup meets the identity class in one element, the class of that cycle type in $p^3-1$ elements, and every other [conjugacy class](../../../../../conjugacy-class.md) in zero elements. They are [Gassmann equivalent](../../../../../gassmann-equivalence.md). They are not isomorphic: $E$ is abelian, whereas the [Heisenberg group](../../../../../heisenberg-group.md) $B$ has $[I+E_{12},I+E_{23}]=I+E_{13}\ne I$.

To obtain arbitrarily many examples in dimension five, choose $r$ distinct odd primes $p_1,\ldots,p_r$ with $2^r\geq n$. For each prime use the preceding pair $E_j,B_j\leq S_{p_j^3}$. Set

$$
T=\prod_{j=1}^r S_{p_j^3},\qquad U_\varepsilon=\prod_{j=1}^r H_{j,\varepsilon_j},\quad
H_{j,0}=E_j,\ H_{j,1}=B_j,\quad\varepsilon\in\{0,1\}^r.
$$

A [conjugacy class](../../../../../conjugacy-class.md) in a direct product is a product of [conjugacy classes](../../../../../conjugacy-class.md), and its intersection count with $U_\varepsilon$ is the product of the individual counts. Thus all $2^r$ subgroups are [Gassmann equivalent](../../../../../gassmann-equivalence.md). They are pairwise nonisomorphic: the unique Sylow $p_j$-subgroup of $U_\varepsilon$ is abelian precisely when $\varepsilon_j=0$, and an abstract [group isomorphism](../../../../../group-isomorphism.md) preserves this property at each prime.

We use the [closed-manifold realization of a finitely presented fundamental group](../../../../../closed-manifold-realization-of-a-finitely-presented-fundamental-group.md) in dimension five. Its construction here is short. From a finite presentation of $T$ with $s$ generators, start with the connected sum of $s$ copies of $S^1\times S^4$. Its [fundamental group](../../../../../fundamental-group.md) is free on those generators. Represent the finitely many relators by disjoint embedded circles, which is possible by [general position for curves in a manifold](../../../../../general-position-for-curves-in-a-manifold.md) in dimension five. Their oriented normal bundles are trivial. Perform framed circle surgery, removing $S^1\times D^4$ and inserting $D^2\times S^3$. The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) shows that each surgery kills exactly the normal closure of the corresponding relator: the attaching circle bounds the new disk, and the new $S^3$ factor contributes no fundamental group. The resulting closed connected five-manifold $M_0$ has $\pi_1(M_0)=T$.

Choose any smooth [Riemannian metric](../../../../../riemannian-metric.md) on $M_0$ and lift it to its [universal cover](../../../../../universal-cover.md) $X$. Since $T$ is finite, $X$ is a compact simply connected five-manifold on which $T$ acts freely and isometrically. The [Sunada theorem](../../../../../sunada-theorem.md) makes all $U_\varepsilon\backslash X$ isospectral, while

$$
\pi_1(U_\varepsilon\backslash X)\cong U_\varepsilon
$$

shows that they are pairwise nonhomeomorphic, hence nonisometric. Taking any $n$ members proves **for every positive integer $n$, there are $n$ pairwise nonisometric closed five-manifolds with the same Laplacian spectrum**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
