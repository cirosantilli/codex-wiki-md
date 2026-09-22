<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Subgroups $U,V$ of a finite [group](../../../../../group-split.md) $T$ have [Gassmann equivalence](../../../../../gassmann-equivalence.md) when

$$
|U\cap C|=|V\cap C|\quad\hbox{for every conjugacy class }C\subseteq T.
$$

Summing over the [conjugacy classes](../../../../../conjugacy-class.md) gives $|U|=|V|$. Equivalently, their coset [permutation representations](../../../../../permutation-representation.md) have the same [character of a representation](../../../../../character-of-a-representation.md). In particular, [almost conjugate subgroups](../../../../../gassmann-equivalence.md) need not be conjugate.

Put $p=\operatorname{ord}A$, $q=\operatorname{ord}B$, and $r=\operatorname{ord}(AB)$. Begin with the sphere punctured at three points. Its [fundamental group](../../../../../fundamental-group.md) is $\langle a,b,c\mid abc=1\rangle$, and the epimorphism sending $a,b,c$ to $A,B,(AB)^{-1}$ defines a connected regular $|T|$-sheeted [covering space](../../../../../covering-space.md). Around the punctures the monodromies have cycles of lengths $p,q,r$. Fill each lifted puncture by a disk, using the local [branched covering](../../../../../branched-covering.md) models $z\mapsto z^p$, $z\mapsto z^q$ and $z\mapsto z^r$. This produces a closed oriented surface $M$, with $T$ acting by [homeomorphisms](../../../../../homeomorphism.md) that are smooth in these local models. This construction works even if one of $p,q,r$ is one.

Triangulate the base sphere with the three marked points as vertices and two faces. Lifting this triangulation gives

$$
F=2|T|,\qquad E=3|T|,\qquad V=|T|(p^{-1}+q^{-1}+r^{-1}),
$$

so the [Euler characteristic](../../../../../euler-characteristic.md) is

$$
\boxed{\chi(M)=|T|\bigl(p^{-1}+q^{-1}+r^{-1}-1\bigr).}
$$

In the hyperbolic case $1/p+1/q+1/r<1$, this is equivalently the [triangle cover construction for Sunada surfaces](../../../../../triangle-cover-construction-for-sunada-surfaces.md). Take the [hyperbolic triangle group](../../../../../hyperbolic-triangle-group.md)

$$
\Delta=\langle a,b,c\mid a^p=b^q=c^r=abc=1\rangle
$$

and its epimorphism $\theta:\Delta\to T$ with the same images. All finite-order elements of $\Delta$ are conjugate to powers of its three elliptic generators. Because their images have the same exact orders, $K=\ker\theta$ is torsion-free and $M=K\backslash\mathbb H^2$. It can be assembled from $2|T|$ [hyperbolic triangles](../../../../../hyperbolic-triangle.md) of angles $\pi/p,\pi/q,\pi/r$. Both examples below belong to this hyperbolic case.

For $M_1=U\backslash M$ and $M_2=V\backslash M$ to be smooth surfaces normally covered by $M$, the subgroup actions must be free. The precise condition is that neither subgroup meet any conjugate in $T$ of a nonidentity power of $A$, $B$ or $AB$. These are exactly the possible point stabilizers. Then $M\to M_1$ and $M\to M_2$ are [regular coverings](../../../../../regular-covering.md), with [deck transformation groups](../../../../../deck-transformation-group.md) $U,V$ respectively. **No normality of $U,V$ in $T$ is needed**: normality would concern the further covering of the base [orbifold](../../../../../orbifold.md), not these coverings from $M$. For a free subgroup $W$,

$$
\chi(W\backslash M)=[T:W]\bigl(p^{-1}+q^{-1}+r^{-1}-1\bigr).
$$

Choose any $T$-invariant smooth [Riemannian metric](../../../../../riemannian-metric.md) on $M$, for example by averaging an arbitrary metric. It descends to both quotients. On functions let $R_t$ be the unitary action of $t\in T$, and let $E=e^{-s\Delta_M}$ for $s>0$. The averaging operator $P_W=|W|^{-1}\sum_{w\in W}R_w$ projects orthogonally onto the $W$-invariant functions, which identify with functions on $W\backslash M$. The trace formula underlying the [Sunada theorem](../../../../../sunada-theorem.md) is

$$
\boxed{\operatorname{Tr}(e^{-s\Delta_{W\backslash M}})=\frac1{|W|}\sum_{w\in W}\operatorname{Tr}(R_we^{-s\Delta_M}).}
$$

The expression $\operatorname{Tr}(R_we^{-s\Delta_M})$ is a class function, because $\Delta_M$ commutes with $T$. Thus [Gassmann equivalence](../../../../../gassmann-equivalence.md) makes the two sums identical. Alternatively, apply the same averaging formula to each finite-dimensional [Laplacian](../../../../../laplacian.md) [eigenspace](../../../../../eigenspace.md): its invariant dimension is $|W|^{-1}\sum_{w\in W}\chi_\lambda(w)$. This proves equality of every [eigenvalue multiplicity](../../../../../eigenvalue-multiplicity.md) and hence **isospectrality of the two quotient metrics**.

If $V=tUt^{-1}$ for some $t\in T$, the action of $t$ gives an [isometry](../../../../../isometry.md) between the quotients for every such metric. Nonconjugacy is therefore necessary. To make it sufficient, choose the quotient [orbifold](../../../../../orbifold.md) metric generically so that its regular locus has no nonidentity [local isometries](../../../../../local-isometry.md); this is the equivariant, or orbifold, version of the [Sunada local isometry lemma](../../../../../sunada-local-isometry-lemma.md). Smooth perturbations on regular coordinate balls provide this genericity while their lifts remain smooth on $M$. Any [isometry](../../../../../isometry.md) between $M_1$ and $M_2$, when composed locally with their projections, would then identify the same points of the base regular locus. By continuation it is an isomorphism of their coverings of that locus, and the [classification of connected covering spaces](../../../../../classification-of-connected-covering-spaces.md) forces $U,V$ to be conjugate in $T$. Thus nonconjugate subgroups give **non-isometric isospectral quotients for a suitable generic invariant metric**. The genericity belongs to the base regular locus; the covering metric on $M$ itself necessarily has the prescribed deck symmetries.

For [genus](../../../../../genus-of-a-surface.md) two, an explicit choice is the following [permutation group](../../../../../permutation-group.md) on twelve labels, with permutation products composed from right to left:

$$
\begin{aligned}
A&=(0\ 7\ 11)(1\ 5\ 6)(2\ 9\ 10)(3\ 4\ 8),\\
B&=(0\ 4\ 2)(1\ 5\ 9)(3\ 7\ 11)(6\ 10\ 8),\\
s&=(1\ 7)(4\ 10),\\
u&=(0\ 9)(2\ 11\ 8\ 5)(3\ 6)(4\ 10),\\
v&=(0\ 3\ 6\ 9)(1\ 10)(2\ 8)(4\ 7),\\
T&=\langle A,B\rangle,\qquad U=\langle s,u\rangle,\quad V=\langle s,v\rangle.
\end{aligned}
$$

These parameters are those in [Kang's genus-two construction](https://arxiv.org/abs/math/0512519). They admit a direct finite verification. Starting with $T_0=\{1\}$ and iterating $T_{j+1}=T_j\cup T_jA\cup T_jB$, the successive sizes are $1,3,7,13,23,39,61,81,93,96$, after which the set is unchanged. Thus $|T|=96$, and direct multiplication gives $(p,q,r)=(3,3,6)$ and $|U|=|V|=8$. The conjugacy-class triples $(|C|,|C\cap U|,|C\cap V|)$, obtained as $C=\{txt^{-1}:t\in T\}$, are

$$
(1,1,1),\ (3,2,2),\ (6,1,1),\ (6,1,1),\ (3,1,1),\ (6,1,1),\ (6,1,1),\ (16,0,0),\ (16,0,0),\ (16,0,0),\ (16,0,0),\ (1,0,0).
$$

This proves [Gassmann equivalence](../../../../../gassmann-equivalence.md). The subgroup $V$ fixes the labels $5,11$, whereas $U$ has no common fixed label, so they cannot be conjugate even in the full symmetric group. Both are groups of order eight, so they meet no nonidentity order-three element. The only order-two power of $AB$ is

$$
(AB)^3=(0\ 6)(1\ 7)(2\ 8)(3\ 9)(4\ 10)(5\ 11),
$$

which is central in $T$ and lies in neither subgroup. This also excludes its conjugates and proves freeness. The quotient [Euler characteristics](../../../../../euler-characteristic.md) and [genera](../../../../../genus-of-a-surface.md) are therefore

$$
\boxed{\chi(M_1)=\chi(M_2)=12(1/3+1/3+1/6-1)=-2,\qquad g(M_1)=g(M_2)=2.}
$$

The covering surface $M$ has [genus](../../../../../genus-of-a-surface.md) nine.

For [genus](../../../../../genus-of-a-surface.md) three, use $T=\operatorname{GL}_3(\mathbb F_2)$, of order $(8-1)(8-2)(8-4)=168$. Let $U$ stabilize a nonzero vector and let $V$ stabilize a two-dimensional subspace. Both have index seven and order twenty-four. An element $t$ fixes $2^{\dim\ker(t-I)}-1$ nonzero vectors. Hyperplanes correspond to nonzero dual vectors over $\mathbb F_2$, so the number fixed in the dual action is $2^{\dim\ker(t^T-I)}-1$, the same number. Equality of these [permutation characters](../../../../../permutation-character.md) proves that the [point and hyperplane stabilizers are almost conjugate](../../../../../point-and-hyperplane-stabilizers-are-almost-conjugate.md).

They are not conjugate. In coordinates where $U$ fixes $e_1$, its elements include all matrices $\begin{pmatrix}1&\alpha\\0&C\end{pmatrix}$ with arbitrary row $\alpha$ and $C\in\operatorname{GL}_2(\mathbb F_2)$. An invariant plane containing $e_1$ would project to a line invariant under every $C$, which is impossible. A plane not containing $e_1$ would be the graph of a linear functional on the quotient, and arbitrary $\alpha$ would move that graph. Thus $U$ stabilizes no plane, whereas every conjugate of $V$ does.

Choose the concrete generators

$$
A=\begin{pmatrix}0&1&0\\1&0&1\\1&0&0\end{pmatrix},\qquad
B=\begin{pmatrix}1&1&0\\1&1&1\\0&1&0\end{pmatrix}.
$$

Over $\mathbb F_2$, each of $A,B,AB$ has order seven. The same closure iteration has sizes $1,3,7,15,31,59,103,144,168$, verifying that $A,B$ generate $T$. Since seven does not divide $24$, neither stabilizer contains a nonidentity power of these generators, or any conjugate of such a power. We may therefore use $(p,q,r)=(7,7,7)$ in the [triangle cover construction for Sunada surfaces](../../../../../triangle-cover-construction-for-sunada-surfaces.md). The quotient calculation is

$$
\boxed{\chi(M_1)=\chi(M_2)=7(3/7-1)=-4,\qquad g(M_1)=g(M_2)=3.}
$$

Here the covering surface $M$ has [genus](../../../../../genus-of-a-surface.md) forty-nine. Choosing the generic invariant metrics described above completes both requested pairs.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
