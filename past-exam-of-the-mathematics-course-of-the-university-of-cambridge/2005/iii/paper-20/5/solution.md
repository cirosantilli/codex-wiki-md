<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use an oriented [geodesic](../../../../../geodesic.md) hyperbolic $2s$-gon $D$ with paired edges of equal length. Identify each pair by a length-preserving map reversing the [boundary](../../../../../boundary-of-a-set.md) directions, to make an oriented base surface $M_0$ with possibly singular vertices. Assign to the $s$ edge pairs generators $A_1,\ldots,A_s$ of $T$, with inverse labels for reversed crossings. For each $g\in T$, take a copy $D_g$ and glue its positively labelled edge of type $k$ to the corresponding mate in $D_{gA_k}$. The generators make the glued surface $M$ connected. Left multiplication $D_g\mapsto D_{hg}$ commutes with these right-labelled gluings and gives the $T$ action with quotient $M_0$.

Existence for an arbitrary finite [group](../../../../../group-split.md) can even be arranged with no cone singularities. If $T$ has $d$ generators, take $h\ge\max\{2,d\}$ and a regular [hyperbolic polygon](../../../../../hyperbolic-polygon.md) with $4h$ edges, all angles $\pi/(2h)$, paired with side word $\prod_{i=1}^h a_ib_ia_i^{-1}b_i^{-1}$. Its vertices form one cycle of angle $2\pi$, giving a smooth base of [genus](../../../../../genus-of-a-surface.md) $h$. Label the $a_i$ by the generators of $T$, padded by identities, and every $b_i$ by the identity. The single vertex word is $\prod_i[A_i,1]=1$, so every lifted vertex also has angle $2\pi$. The resulting connected ordinary [normal covering map](../../../../../normal-covering-map.md) has degree $|T|$ and deck [group](../../../../../group-split.md) $T$.

This is the [paired-polygon construction of finite surface covers](../../../../../paired-polygon-construction-of-finite-surface-covers.md). Interior and open-edge points are regular hyperbolic points; possible singularities occur only at vertices. When the base has cone points, the map is an [orbifold](../../../../../orbifold.md) covering and may be branched as a map between the underlying topological surfaces. It should not be called an unbranched [manifold](../../../../../topological-manifold.md) covering at those branch points.

A [vertex cycle of a paired polygon](../../../../../vertex-cycle-of-a-paired-polygon.md) is the collection of vertices identified to one point on $M_0$. Let $r$ be the number of cycles, $\theta_j$ the sum of the polygon angles in cycle $j$, and $C_j\in T$ the gluing word recorded on going around it. If $q_j=|C_j|$ is the order of that element, a lift closes after $q_j$ turns. It has angle $q_j\theta_j$, and there are $|T|/q_j$ such lifted vertices. The base and lifted cone orders, when they are integer [orbifold](../../../../../orbifold.md) orders, are

$$
\boxed{m_j=\frac{2\pi}{\theta_j},\qquad \widetilde m_j=\frac{2\pi}{q_j\theta_j}=\frac{m_j}{q_j}.}
$$

An [orbifold](../../../../../orbifold.md) homomorphism requires $q_j\mid m_j$. The lifted point is smooth exactly when $q_j\theta_j=2\pi$, equivalently $q_j=m_j$ in that case. For arbitrary cone metrics the angle formulas remain valid even when an angle does not correspond to an integer [orbifold](../../../../../orbifold.md) order.

Counting faces, edges and vertices gives the [Euler characteristic of a paired-polygon surface cover](../../../../../euler-characteristic-of-a-paired-polygon-surface-cover.md):

$$
\boxed{\chi(M_0)=1-s+r,\qquad \chi(M)=|T|\left(1-s+\sum_{j=1}^r\frac1{q_j}\right).}
$$

These are ordinary topological Euler characteristics, rather than [orbifold](../../../../../orbifold.md) Euler characteristics. If the lifted surface is smooth, the equivalent [orbifold](../../../../../orbifold.md) formula is

$$
\chi(M)=|T|\chi_{\rm orb}(M_0),\qquad
\chi_{\rm orb}(M_0)=\chi(M_0)-\sum_j\left(1-\frac1{m_j}\right).
$$

For a [closed](../../../../../closed-set.md) oriented smooth surface, $\chi=2-2g$ defines its [genus](../../../../../genus-of-a-surface.md). These formulas also follow from the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) by subtracting the ramification deficits $|T|-|T|/q_j$ over each base vertex.

For $U\le T$, the quotient map $M\to M_1=U\backslash M$ is an ordinary normal covering if and only if $U$ acts freely. All possible point stabilizers in this construction are conjugates of $\langle C_j\rangle$, so the concrete necessary and sufficient condition is

$$
\boxed{U\cap g\langle C_j\rangle g^{-1}=\{1\}\quad\text{for every }j\text{ and every }g\in T.}
$$

This is the [freeness criterion for a subgroup of a polygon-cover deck group](../../../../../freeness-criterion-for-a-subgroup-of-a-polygon-cover-deck-group.md). Under it the deck [group](../../../../../group-split.md) is $U$, the degree is $|U|$, and

$$
\boxed{\chi(M_1)=\frac{\chi(M)}{|U|}.}
$$

There is no requirement $U\triangleleft T$ for this map. That different condition characterizes normality of the intermediate cover $M_1\to M_0$. If fixed points are retained and one instead speaks of an [orbifold](../../../../../orbifold.md) covering, the quotient is regular as an [orbifold](../../../../../orbifold.md) cover, but ordinary [Euler characteristic](../../../../../euler-characteristic.md) need not divide by $|U|$; [orbifold Euler characteristic](../../../../../orbifold-euler-characteristic.md) does.

For the low-genus examples take

$$
T=\operatorname{GL}(3,\mathbb F_2)=\operatorname{PSL}(3,2),\qquad |T|=(8-1)(8-2)(8-4)=168.
$$

Let $U_1$ be a nonzero-vector stabilizer and $U_2$ a plane stabilizer. Their actions have seven points, so $|U_1|=|U_2|=24$ and $[T:U_i]=7$. They are [almost conjugate subgroups](../../../../../gassmann-equivalence.md): the numbers of fixed nonzero vectors for a matrix $A$ and its dual action $A^{-T}$ are both $2^{\dim\ker(A-I)}-1$. Thus the two coset [permutation characters](../../../../../permutation-character.md) agree, which is equivalent to [Gassmann equivalence](../../../../../gassmann-equivalence.md). They are not conjugate: a point stabilizer has a common fixed nonzero vector, whereas a plane stabilizer fixes no nonzero vector globally. In particular, since $7\nmid24$, neither [subgroup](../../../../../subgroup.md) contains any nonidentity element of a cyclic [subgroup](../../../../../subgroup.md) of order seven. All cone monodromies of exact order seven therefore act freely on the intermediate covers.

For [genus](../../../../../genus-of-a-surface.md) three, start with a [hyperbolic triangle](../../../../../hyperbolic-triangle.md) whose three angles are $\pi/7$ and double it across one edge. The resulting quadrilateral $D$ has angles

$$
\boxed{\pi/7,\ 2\pi/7,\ \pi/7,\ 2\pi/7.}
$$

The side pairings produce three base vertex cycles, each of total angle $2\pi/7$, and an underlying sphere. Choose generators $A,B$ with $|A|=|B|=|AB|=7$; the three vertex words are $A,B,(AB)^{-1}$. Hence $s=2$, $r=3$ and all $q_j=7$. The full cover is smooth, and

$$
\chi(M)=168\left(-1+\frac37\right)=-96,\qquad
\chi(U_i\backslash M)=-96/24=-4,\qquad\boxed{g_i=3.}
$$

The [hyperbolic polygon area](../../../../../hyperbolic-polygon-area.md) of $D$ is $8\pi/7$, so the seven-sheeted surfaces have [area](../../../../../surface-area.md) $8\pi$, agreeing with Gauss-Bonnet. Their equal spectra follow from the Sunada theorem. For complete numerical generator data, one possible pair is

$$
A=\begin{pmatrix}0&0&1\\0&1&1\\1&1&0\end{pmatrix},\qquad
B=\begin{pmatrix}0&0&1\\1&0&0\\0&1&1\end{pmatrix}
\quad\text{over }\mathbb F_2.
$$

These generate all of $T$ and have the required orders. This construction establishes the requested [isospectrality](../../../../../isospectral-manifolds.md); it does not establish nonisometry. In the constant-curvature triangle example a lifted reflection can identify the point and plane covers, as in [reflection intertwining of triangle-cover coset actions](../../../../../reflection-intertwining-of-triangle-cover-coset-actions.md). Breaking that symmetry with a generic metric gives nonisometric genus-three surfaces, but then the metric need not have constant curvature. Those are distinct assertions.

For [genus](../../../../../genus-of-a-surface.md) four, use the [cone-torus construction of genus-four Sunada surfaces](../../../../../cone-torus-construction-of-genus-four-sunada-surfaces.md). Take a regular hyperbolic quadrilateral with four angles

$$
\boxed{\pi/14,\ \pi/14,\ \pi/14,\ \pi/14}
$$

and pair opposite sides in the usual [torus](../../../../../torus.md) pattern $a,b,a^{-1},b^{-1}$. All four vertices belong to one cycle, whose total angle is $2\pi/7$; the underlying base is a [torus](../../../../../torus.md) with one [cone point](../../../../../cone-point.md). Choose $A,B$ of order four generating $T$, with commutator $[A,B]$ of order seven. For example,

$$
A=\begin{pmatrix}0&0&1\\0&1&0\\1&1&0\end{pmatrix},\qquad
B=\begin{pmatrix}0&0&1\\0&1&1\\1&0&0\end{pmatrix},\qquad
|A|=|B|=4,\quad |[A,B]|=7.
$$

Only the commutator is a cone monodromy, so the order-four side labels do not create cone points of order four. Here $s=2$, $r=1$, $q_1=7$, giving

$$
\chi(M)=168\left(-1+\frac17\right)=-144,\qquad
\chi(U_i\backslash M)=-144/24=-6,\qquad\boxed{g_i=4.}
$$

The quadrilateral has [area](../../../../../surface-area.md) $12\pi/7$, and each seven-sheeted smooth quotient has [area](../../../../../surface-area.md) $12\pi$. Again the order-seven cone stabilizer meets neither $U_i$ nontrivially, so the metrics are smooth and the Sunada theorem gives identical spectra. The required [group](../../../../../group-split.md) and [subgroup](../../../../../subgroup.md) orders are therefore **168 and 24 in both constructions**; the genus-three side-generator orders are **7 and 7**, and the displayed genus-four side-generator orders are **4 and 4**, with cone-word order **7** in both cases.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
