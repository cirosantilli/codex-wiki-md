<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in the [homotopy](../../../../../homotopy.md) category of [simply connected](../../../../../simply-connected-space.md) [CW complexes](../../../../../cw-complex.md). This is one of the permitted assumptions on the [fundamental group](../../../../../fundamental-group.md); it makes every coefficient system below untwisted. A [rational space](../../../../../rational-space.md) is a [simply connected](../../../../../simply-connected-space.md) space whose [homotopy groups](../../../../../homotopy-group.md) are [vector spaces](../../../../../vector-space-split.md) over $\mathbb Q$. A [rationalization of a topological space](../../../../../rationalization-of-a-topological-space.md) is a map $r:X\to X_{\mathbb Q}$ to such a space which induces

$$
\boxed{\pi_i(X_{\mathbb Q})\cong\pi_i(X)\otimes\mathbb Q\quad(i\ge2).}
$$

Its purpose includes a universal mapping property, which will be described after the construction.

An [Eilenberg–MacLane space](../../../../../eilenberg-maclane-space.md) $K(A,n)$ has exactly one nonzero [homotopy group](../../../../../homotopy-group.md), $\pi_n=A$, where $A$ is abelian when $n\ge2$. The representability theorem says $[B,K(A,n)]\cong H^n(B;A)$, naturally in $B$ and $A$. More generally, a [principal fibration](../../../../../principal-fibration.md) is a [homotopy pullback](../../../../../homotopy-pullback.md) of a [path-space fibration](../../../../../path-space-fibration.md) $PC\to C$ along a map from its base to $C$; the fibre $\Omega C$ acts on the fibre paths by concatenation. For the [Postnikov tower](../../../../../postnikov-tower.md) construction take $C=K(A,n+1)$. A [principal Eilenberg–MacLane fibration](../../../../../principal-eilenberg-maclane-fibration.md) with fibre $K(A,n)$ is the [homotopy pullback](../../../../../homotopy-pullback.md) of the [path fibration](../../../../../path-space-fibration.md) of $K(A,n+1)$. Equivalently, its total space is the [homotopy fibre](../../../../../homotopy-fiber.md) of a map $k:B\to K(A,n+1)$. It is classified by the [cohomology class](../../../../../cohomology-class.md) $[k]\in H^{n+1}(B;A)$; there is no nontrivial action of the base [fundamental group](../../../../../fundamental-group.md) on the fibre coefficients in this principal description.

The [Postnikov tower](../../../../../postnikov-tower.md) theorem supplies spaces $P_nX$ and compatible maps

$$
X\longrightarrow\cdots\longrightarrow P_nX\longrightarrow P_{n-1}X
\longrightarrow\cdots\longrightarrow P_1X\simeq *
$$

with $\pi_i(P_nX)=\pi_i(X)$ for $i\le n$ and zero for $i>n$. For a [simply connected](../../../../../simply-connected-space.md) $X$, the fibre of $P_nX\to P_{n-1}X$ is $K(\pi_nX,n)$, and the fibration is principal. Its [Postnikov invariant](../../../../../postnikov-invariant.md) is

$$
k_n\in H^{n+1}(P_{n-1}X;\pi_nX),
$$

represented by $P_{n-1}X\to K(\pi_nX,n+1)$, whose [homotopy fibre](../../../../../homotopy-fiber.md) is $P_nX$. Thus the [homotopy groups](../../../../../homotopy-group.md) alone are not the tower data: the classes $k_n$ specify how each new group is attached. For instance a zero class gives a product with $K(\pi_nX,n)$.

State also the standard rational comparison results used in constructing the tower: $K(A,n)\to K(A\otimes\mathbb Q,n)$ is a [rational homology](../../../../../rational-homology.md) equivalence; a map between [simply connected](../../../../../simply-connected-space.md) spaces is a [rational homology](../../../../../rational-homology.md) equivalence if and only if it induces isomorphisms on all [rational homotopy groups](../../../../../rational-homotopy-group.md); and a [rational homology](../../../../../rational-homology.md) equivalence induces isomorphisms in [cohomology](../../../../../cohomology-split.md) with any constant rational vector-space coefficients. The last assertion uses the universal coefficient theorem over the [field](../../../../../field.md) $\mathbb Q$. These results are used here without proof, as allowed for this essay.

Construct rational stages inductively, with $P_1^{\mathbb Q}=*$. Suppose $r_{n-1}:P_{n-1}X\to P_{n-1}^{\mathbb Q}$ has already been constructed and is a [rational homology](../../../../../rational-homology.md) equivalence. Put $V_n=\pi_nX\otimes\mathbb Q$ and change coefficients in $k_n$ to obtain $\overline k_n\in H^{n+1}(P_{n-1}X;V_n)$. The comparison result gives an isomorphism

$$
r_{n-1}^*:H^{n+1}(P_{n-1}^{\mathbb Q};V_n)
\xrightarrow{\sim}H^{n+1}(P_{n-1}X;V_n).
$$

Let $k_n^{\mathbb Q}$ be its unique inverse image and define

$$
P_n^{\mathbb Q}=\operatorname{hofib}\bigl(
 k_n^{\mathbb Q}:P_{n-1}^{\mathbb Q}\to K(V_n,n+1)\bigr).
$$

Equality of the pulled-back classes gives a homotopy-commuting square of classifying maps, and hence a map $r_n:P_nX\to P_n^{\mathbb Q}$ over $r_{n-1}$. On the fibre it is the map induced by $\pi_nX\to V_n$. The [homotopy](../../../../../homotopy.md) exact sequences therefore show that $r_n$ tensors all [homotopy groups](../../../../../homotopy-group.md) through degree $n$ with $\mathbb Q$, while the higher groups of both stages vanish. The rational comparison theorem makes $r_n$ a [rational homology](../../../../../rational-homology.md) equivalence, allowing the induction to continue.

Take the [homotopy inverse limit](../../../../../homotopy-inverse-limit-of-a-tower.md) of the rational tower:

$$
X_{\mathbb Q}=\operatorname{holim}_n P_n^{\mathbb Q}.
$$

The convergence theorem for a [Postnikov tower](../../../../../postnikov-tower.md) gives $X\simeq\operatorname{holim}_nP_nX$ and the compatible stage maps induce $r:X\to X_{\mathbb Q}$. To see what convergence says here, fix a [homotopy](../../../../../homotopy.md) degree $i$. From stage $n\ge i$ onwards the group and its transition maps are constant; the inverse-limit group is $\pi_iX\otimes\mathbb Q$ and the associated derived-limit obstruction is zero. Thus this construction has exactly the claimed [rational homotopy groups](../../../../../rational-homotopy-group.md). Taking a [homotopy](../../../../../homotopy.md) limit, rather than an arbitrary set-theoretic inverse limit, is part of the construction.

The rational localization theorem says that this map has the universal property

$$
\boxed{r^*:[X_{\mathbb Q},Z]\xrightarrow{\sim}[X,Z]
\quad\text{for every simply connected rational space }Z.}
$$

In other words every map from $X$ to a [rational space](../../../../../rational-space.md) factors through $r$, and the factorization is unique up to [homotopy](../../../../../homotopy.md). This concerns [homotopy classes](../../../../../homotopy-class.md), not strict uniqueness of point-set maps. The theorem can be formulated as localization of the [simply connected](../../../../../simply-connected-space.md) [homotopy category](../../../../../homotopy-category.md) at [rational homotopy equivalences](../../../../../rational-homotopy-equivalence.md); [rational spaces](../../../../../rational-space.md) are its local objects. It also implies uniqueness of [rationalization of a topological space](../../../../../rationalization-of-a-topological-space.md): apply the property to two candidate [rational spaces](../../../../../rational-space.md) to obtain inverse equivalences under $X$. In particular the construction forgets torsion in [homotopy](../../../../../homotopy.md) while retaining precisely the information needed for maps to rational targets.

The same theory extends to [nilpotent spaces](../../../../../nilpotent-space.md), where the [fundamental group](../../../../../fundamental-group.md) is nilpotent and its action on higher [homotopy groups](../../../../../homotopy-group.md) is nilpotent. That version requires localization of the [fundamental group](../../../../../fundamental-group.md) and compatible treatment of its coefficient action. The [simply connected](../../../../../simply-connected-space.md) assumption chosen here avoids those additional issues and supplies the full construction and mapping property requested.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
