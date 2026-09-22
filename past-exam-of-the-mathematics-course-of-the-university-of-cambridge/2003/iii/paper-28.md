# Paper 28

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper28.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper28.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The possible ranks and the corresponding [homeomorphism](../../../topology.md#homeomorphism) types are

$$
\boxed{n=0:\ S^3;\qquad n=1:\ S^2\times S^1;\qquad n=3:\ T^3.}
$$

There is no example for $n=2$ or $n\geq4$. The uniqueness here is topological, not uniqueness of a [Riemannian metric](../../../differential-geometry.md#riemannian-metric).

To see the restrictions, use the [prime decomposition of a closed orientable three-manifold](../../../topology.md#prime-decomposition-of-a-closed-orientable-three-manifold). Its [fundamental group](../../../algebraic-topology.md#fundamental-group) is the [free product](../../../algebraic-topology.md#free-product) of the [prime three-manifold](../../../topology.md#prime-three-manifold) groups. A [free product](../../../algebraic-topology.md#free-product) of two nontrivial groups is nonabelian, so at most one summand can have nontrivial [fundamental group](../../../algebraic-topology.md#fundamental-group). The remaining [simply connected](../../../algebraic-topology.md#simply-connected-space) summands are three-spheres by the [Poincaré conjecture](../../../topology.md#poincare-conjecture). If the nontrivial summand is not irreducible, it is $S^2\times S^1$, giving rank one. If it is irreducible and has infinite [fundamental group](../../../algebraic-topology.md#fundamental-group), the [sphere theorem for three-manifolds](../../../topology.md#sphere-theorem-for-three-manifolds) makes it [aspherical](../../../algebraic-topology.md#aspherical-space). Its [fundamental group](../../../algebraic-topology.md#fundamental-group) is then a dimension-three [Poincare duality group](../../../group-theory.md#poincare-duality-group). But $\mathbb Z^n$ is a duality group of dimension $n$, as seen from the [torus](../../../topology.md#torus) classifying space or its [Koszul resolution](../../../algebra.md#koszul-resolution), so $n=3$.

For rank three, the flat case of the [geometrization theorem](../../../topology.md#geometrization-conjecture) says that a closed irreducible orientable [three-manifold](../../../topology.md#3-manifold) with [fundamental group](../../../algebraic-topology.md#fundamental-group) $\mathbb Z^3$ admits a flat metric. Write it as $\mathbb R^3/\Gamma$. By the [Bieberbach theorem](../../../second-fundamental-form.md#bieberbach-theorem), $\Gamma$ contains a full-rank translation lattice $\Lambda$. If $g=(R,v)\in\Gamma$ commutes with translation by each $\lambda\in\Lambda$, then $R\lambda=\lambda$ for every lattice vector, forcing $R=I$. Since $\Gamma$ itself is abelian, it consists entirely of translations. Its quotient is therefore the three-torus. Rank zero follows directly from the [Poincaré conjecture](../../../topology.md#poincare-conjecture), and rank one was already determined by the [prime decomposition of a closed orientable three-manifold](../../../topology.md#prime-decomposition-of-a-closed-orientable-three-manifold). Historically, before the Poincare theorem, the uniqueness conclusions were phrased allowing [connected sums](../../../differential-geometry.md#connected-sum-of-oriented-manifolds) with [homotopy](../../../algebraic-topology.md#homotopy) three-spheres; the modern theorem removes that ambiguity.

The six flat types below mean the six **closed orientable** flat [three-manifold](../../../topology.md#3-manifold) types. There are infinitely many individual flat metrics and there are additional noncompact [flat Riemannian manifolds](../../../second-fundamental-form.md#flat-manifold). In each closed case the [universal cover](../../../algebraic-topology.md#universal-cover) is [Euclidean space](../../../functional-analysis.md#euclidean-norm) and the [deck transformation group](../../../algebraic-topology.md#deck-transformation-group) is a torsion-free crystallographic group. The [holonomy groups of closed orientable flat three-manifolds](../../../second-fundamental-form.md#holonomy-groups-of-closed-orientable-flat-three-manifolds) are $1,C_2,C_3,C_4,C_6,C_2\times C_2$.

The first is a [flat torus](../../../second-fundamental-form.md#flat-torus) $\mathbb R^3/\Lambda$, with trivial holonomy. For each cyclic case choose a planar lattice $L$ admitting the relevant rotation $R_m$, and generate the [deck transformation group](../../../algebraic-topology.md#deck-transformation-group) by translations in $L$ and the screw

$$
s_m(v,z)=(R_mv,z+1/m),\qquad m=2,3,4,6.
$$

Its $m$th power is unit translation along the axis. A nontrivial holonomy element has nonzero axial displacement modulo integers, so has no fixed point. All transformations preserve orientation. A compact prism [fundamental domain](../../../group-theory.md#fundamental-domain) gives compactness. Equivalently, the manifold is a [torus](../../../topology.md#torus) [mapping torus](../../../algebraic-topology.md#mapping-torus) with finite-order [monodromy](../../../complex-analysis.md#monodromy). In planar lattice bases one may take

$$
R_2=-I,\quad
R_3=\begin{pmatrix}-1&-1\\1&0\end{pmatrix},\quad
R_4=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\quad
R_6=\begin{pmatrix}0&-1\\1&1\end{pmatrix}.
$$

The half-turn uses any planar lattice, the quarter-turn a square lattice, and the third- and sixth-turns a hexagonal lattice. These give respectively the [half-turn flat three-manifold](../../../second-fundamental-form.md#half-turn-flat-three-manifold), [third-turn flat three-manifold](../../../second-fundamental-form.md#third-turn-flat-three-manifold), [quarter-turn flat three-manifold](../../../second-fundamental-form.md#quarter-turn-flat-three-manifold), and [sixth-turn flat three-manifold](../../../second-fundamental-form.md#sixth-turn-flat-three-manifold). Their holonomies have orders $2,3,4,6$, and their first [Betti numbers](../../../homology.md#betti-number) are all one, since the only fixed direction of holonomy is the screw axis.

The sixth type is the [Hantzsche-Wendt manifold](../../../second-fundamental-form.md#hantzsche-wendt-manifold). A concrete group is generated by

$$
\alpha(x,y,z)=(x+1/2,-y,-z),\qquad
\beta(x,y,z)=(-x,y+1/2,-z+1/2).
$$

Their linear parts are commuting half-turns about perpendicular axes. Moreover $\alpha^2$, $\beta^2$ and $(\alpha\beta)^2$ are translations by $(1,0,0)$, $(0,1,0)$ and $(0,0,-1)$. Their translation subgroup is the unit cubic lattice and their linear quotient is $C_2\times C_2$. In each nontranslation coset, the displacement along the fixed axis is a half-integer, so the action is free. The quotient is compact and orientable. No vector is fixed by both linear parts, so its first [Betti number](../../../homology.md#betti-number) is zero. Bieberbach classification gives precisely these six affine types; the explicit screw descriptions distinguish them without identifying arbitrary finite quotients with holonomy.

## 2

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [nilpotent group](../../../group-theory.md#nilpotent-group) has [lower central series](../../../group-theory.md#lower-central-series) $\gamma_1G=G$, $\gamma_{j+1}G=[G,\gamma_jG]$ terminating at the identity. A [polycyclic group](../../../group-theory.md#polycyclic-group) has a finite [subnormal series](../../../group-theory.md#subnormal-series) with cyclic factors, which may be finite or infinite.

If a [nilpotent group](../../../group-theory.md#nilpotent-group) is generated by finitely many elements, then $\gamma_jG/\gamma_{j+1}G$ is generated by the finitely many weight-$j$ iterated [commutators](../../../lie-algebra.md#commutator) in these generators. Modulo the next term, [commutator](../../../lie-algebra.md#commutator) identities make these quotients abelian and permit this collection of words. Each quotient is thus a [finitely generated abelian group](../../../group.md#finitely-generated-abelian-group). Refine each by a series with cyclic factors and splice the refinements through the finite [lower central series](../../../group-theory.md#lower-central-series). This proves that a finitely generated [nilpotent group](../../../group-theory.md#nilpotent-group) is polycyclic.

For the duality-group assertion, first prove the useful finite-index reduction. Induct on the length of a polycyclic series, taking its last proper term $H\triangleleft G$. By induction $H$ has a finite-index [poly-infinite cyclic group](../../../group-theory.md#poly-infinite-cyclic-group). Because $H$ is finitely generated, it has only finitely many subgroups of any fixed finite index. Intersect all automorphic images of that subgroup to obtain a characteristic [finite-index subgroup](../../../group.md#finite-index-subgroup) $H_0\subset H$ which is still poly-infinite cyclic. It is normal in $G$. The quotient $G/H_0$ is finite-by-cyclic. If it is finite, $H_0$ already suffices; if its cyclic quotient is infinite, the subgroup generated by a lift of its generator is infinite cyclic and has finite index. Its preimage in $G$ is an extension of $H_0$ by $\mathbb Z$, hence poly-infinite cyclic. This proves [polycyclic groups are virtually poly-infinite cyclic](../../../group-theory.md#polycyclic-groups-are-virtually-poly-infinite-cyclic).

Take such a [finite-index subgroup](../../../group.md#finite-index-subgroup) $P$ of the given dimension-three [Poincare duality group](../../../group-theory.md#poincare-duality-group). It is again a dimension-three duality group. The extension rule proved in Question 3, applied successively to its infinite cyclic series, makes $P$ a duality group of dimension equal to its [Hirsch length](../../../group-theory.md#hirsch-length). Hence that length is three. Its last quotient gives

$$
1\longrightarrow H\longrightarrow P\longrightarrow\mathbb Z\longrightarrow1,
$$

where $H$ has a poly-infinite cyclic series of length two. Thus $H\cong\mathbb Z\rtimes\mathbb Z$, with the last generator acting on the first by $+1$ or $-1$. In the first case $H=\mathbb Z^2$. In the second case $H$ is the Klein-bottle group $\langle a,b\mid bab^{-1}=a^{-1}\rangle$. Its characteristic subgroup $\langle a,b^2\rangle\cong\mathbb Z^2$ is the centralizer of its [commutator subgroup](../../../group-theory.md#commutator-subgroup) $\langle a^2\rangle$. Replace $H$ by this characteristic index-two subgroup if necessary. It remains normal in $P$, and the quotient is finite-by-infinite-cyclic. Taking the preimage of a finite-index infinite cyclic subgroup gives

$$
\boxed{1\longrightarrow\mathbb Z^2\longrightarrow P_0\longrightarrow\mathbb Z\longrightarrow1,\qquad [G:P_0]<\infty.}
$$

This extension splits: any lift $t$ of the cyclic generator supplies a section. Therefore $P_0=\mathbb Z^2\rtimes_B\mathbb Z$ for some $B\in GL_2(\mathbb Z)$.

In additive notation on $\mathbb Z^2$, $[t,v]=(B-I)v$. All its other internal [commutators](../../../lie-algebra.md#commutator) vanish, so induction gives

$$
\gamma_{j+1}P_0=(B-I)^j\mathbb Z^2\quad(j\geq1).
$$

Consequently

$$
\boxed{P_0\text{ is nilpotent}\iff(B-I)^2=0
\iff\operatorname{tr}B=2\text{ and }\det B=1.}
$$

This is the [nilpotence criterion for an abelian-by-cyclic group](../../../group-theory.md#nilpotence-criterion-for-an-abelian-by-cyclic-group). If $B=I$ the group is abelian; otherwise it is two-step nilpotent. The criterion concerns this actual semidirect product. A finite extension of it is only known to be virtually nilpotent: for example $\mathbb Z^2\rtimes_{-I}\mathbb Z$ is virtually abelian but its [lower central series](../../../group-theory.md#lower-central-series) never terminates.

Write elements of the [real Heisenberg group](../../../lie-algebra.md#heisenberg-group) as $(x,y,z)$. Direct matrix multiplication and inversion give

$$
(x,y,z)(x',y',z')=(x+x',y+y',z+z'+xy'),\qquad
(x,y,z)^{-1}=(-x,-y,-z+xy).
$$

These formulas show that $N_k=(k\mathbb Z)^3$ is a subgroup. It is discrete. For the right quotient, multiplying by $(ka,kb,kc)$ changes the coordinates to

$$
(x+ka,\ y+kb,\ z+kc+xkb).
$$

Thus $(x\bmod k,y\bmod k)$ is well defined on the quotient. Over a small base rectangle choose real lifts $x,y$ of its coordinates. Every coset above that rectangle has a representative $(x,y,z)$, and two such representatives differ precisely by $z\mapsto z+kc$. Hence

$$
U\times(\mathbb R/k\mathbb Z)\longrightarrow p^{-1}(U),\qquad
((x,y),[z])\longmapsto(x,y,z)N_k
$$

is a smooth [local trivialization](../../../fiber-bundle.md#local-trivialization). The fibres are circles, proving the locally trivial fibration over $\mathbb R^2/k\mathbb Z^2\cong T^2$. Reducing first $x,y$ and then $z$ also gives a compact fundamental region, so $N_k$ is cocompact.

The ambient [Lie group](../../../lie-theory.md#lie-group) is diffeomorphic to $\mathbb R^3$, hence [simply connected](../../../algebraic-topology.md#simply-connected-space) and contractible. Its quotient has [fundamental group](../../../algebraic-topology.md#fundamental-group) $N_k$, and the first integral [homology](../../../homology.md) is its [abelianization](../../../group-theory.md#abelianization). Let $a=(k,0,0)$, $b=(0,k,0)$ and $c=(0,0,k)$. Every element is uniquely $a^mb^nc^\ell$, since its third coordinate is $k^2mn+k\ell$. The [commutator](../../../lie-algebra.md#commutator) formula is

$$
[(x,y,z),(x',y',z')]=(0,0,xy'-x'y),
$$

so $c$ is central and $[a,b]=c^k$. Every [commutator](../../../lie-algebra.md#commutator) lies in $(0,0,k^2\mathbb Z)$, and this subgroup is generated by $[a,b]$. Thus $N_k'=\langle c^k\rangle$. The homomorphism $(x,y,z)\mapsto(x/k,y/k,z/k\bmod k)$ is surjective onto $\mathbb Z^2\oplus\mathbb Z/k$ and has exactly this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map); the cross term in multiplication is divisible by $k$ after dividing by $k$. Therefore

$$
\boxed{H_1(\mathrm{Nil}^3/N_k;\mathbb Z)\cong N_k/N_k'\cong\mathbb Z^2\oplus\mathbb Z/k.}
$$

For $k=1$ the last factor is trivial. This is the [Scaled Heisenberg lattice](../../../lie-algebra.md#scaled-heisenberg-lattice), whose fibre is central but whose total group need not split as a [direct product of groups](../../../group-theory.md#direct-product-of-groups).

## 3

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use integral coefficients throughout, allowing a nontrivial orientation character. A dimension-$d$ [Poincare duality group](../../../group-theory.md#poincare-duality-group) has a finite resolution by finitely generated projective group-ring modules and

$$
H^j(G;\mathbb ZG)=0\quad(j\ne d),\qquad H^d(G;\mathbb ZG)\cong\mathbb Z
$$

as [abelian groups](../../../group.md#abelian-group). The action on the top copy of $\mathbb Z$ may be by signs. This group-ring criterion is particularly suited to the [Lyndon–Hochschild–Serre spectral sequence](../../../group-theory.md#lyndon-hochschild-serre-spectral-sequence).

Apply that sequence to the extension with coefficient module $\mathbb ZG$:

$$
E_2^{a,b}=H^a\bigl(Q;H^b(N;\mathbb ZG)\bigr)
\Longrightarrow H^{a+b}(G;\mathbb ZG).
$$

As an $N$-module, $\mathbb ZG$ is a [direct sum](../../../vector-space.md#direct-sum) of copies of $\mathbb ZN$ indexed by the cosets in $Q$. [Cohomology](../../../cohomology.md) of $N$ commutes with this [direct sum](../../../vector-space.md#direct-sum) because its [projective resolution](../../../algebra.md#projective-resolution) is finitely generated. Hence the inner [cohomology](../../../cohomology.md) vanishes except when $b=n$, where it is a [direct sum](../../../vector-space.md#direct-sum) of rank-one groups indexed by $Q$. The $Q$-action shifts these summands freely and transitively, with possible signs from the orientation module. Choosing a generator in one summand and transporting it by $Q$ identifies the resulting left $Q$-module with its regular module $\mathbb ZQ$. The residual right [group action](../../../group-theory.md#group-action) records the orientation twist; it need not be trivial.

Now the duality of $Q$ says that the only nonzero $E_2$ term is $(a,b)=(q,n)$ and that this term is $\mathbb Z$ as an [abelian group](../../../group.md#abelian-group). No differential can enter or leave it. Therefore $H^*(G;\mathbb ZG)$ has exactly the duality pattern in degree $n+q$. The usual extension-resolution construction also supplies a resolution by [finitely generated projective modules](../../../module-theory.md#finite-projective-module): combine the finite [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and quotient resolutions, lift the quotient differentials and add the necessary [homotopy](../../../algebraic-topology.md#homotopy) corrections. Its total length is at most $n+q$. Alternatively, the same [spectral sequence](../../../algebra.md#spectral-sequence) for arbitrary coefficient modules gives the dimension bound, while the extension finiteness lemma supplies finite generation of the resolution. The surviving top term makes the bound sharp. This proves the [extension rule for Poincare duality groups](../../../group-theory.md#extension-rule-for-poincare-duality-groups):

$$
\boxed{G\text{ is a }PD^{n+q}\text{ group}.}
$$

Requiring a trivial top orientation action would need an additional orientation condition; the untwisted conclusion is not implicit in the hypotheses.

We next need two precise auxiliary dimension results. The [Strebel infinite-index subgroup theorem](../../../group-theory.md#strebel-infinite-index-subgroup-theorem) says that an infinite-index subgroup of an integral $PD^d$ group has [integral cohomological dimension](../../../group-theory.md#integral-cohomological-dimension-of-a-group) at most $d-1$. The [Stallings-Swan theorem](../../../group-theory.md#stallings-swan-theorem) says that a group of [integral cohomological dimension](../../../group-theory.md#integral-cohomological-dimension-of-a-group) at most one is free, including the trivial group. Since $G/N$ contains an element of infinite order, $N$ has infinite index in $G$, so $\operatorname{cd}N\leq2$. If its dimension is at most one, the required free-group conclusion follows, with finite rank because $N$ is finitely presented.

Suppose instead that $\operatorname{cd}N=2$. [Finite presentation](../../../module-theory.md#finite-presentation-of-a-module) gives a partial [free resolution](../../../algebra.md#free-resolution) with finitely generated modules through degree two. The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) in degree one is finitely generated and, because the [integral cohomological dimension](../../../group-theory.md#integral-cohomological-dimension-of-a-group) is two, projective. Truncating at this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) gives a finite resolution by [finitely generated projective modules](../../../module-theory.md#finite-projective-module). Thus $N$ has the finiteness needed for group-ring [cohomology](../../../cohomology.md) to commute with [direct sums](../../../vector-space.md#direct-sum).

Choose an infinite-order element $\bar t\in G/N$, lift it to $t\in G$, and let $H$ be the preimage of $\langle\bar t\rangle$. Then $H=N\rtimes\langle t\rangle$. Restriction of $\mathbb ZH$ to $N$ yields copies of $\mathbb ZN$ indexed by all powers of $t$. For every $j$, the quotient generator acts on $H^j(N;\mathbb ZH)$ by shifting this [direct sum](../../../vector-space.md#direct-sum), possibly with an automorphism on each copy. Its invariants vanish, since an invariant finite-support sequence must be zero. Its coinvariants are one copy of $H^j(N;\mathbb ZN)$: the shift relations identify successive copies, and any twists can be removed by transporting the identifications along the integer index.

The [infinite cyclic group](../../../group.md#infinite-cyclic-group) has [integral cohomological dimension](../../../group-theory.md#integral-cohomological-dimension-of-a-group) one, so only columns zero and one occur in the [spectral sequence](../../../algebra.md#spectral-sequence). Column zero vanishes and column one consists of these coinvariants. We obtain the [cyclic-extension shift of group-ring cohomology](../../../group-theory.md#cyclic-extension-shift-of-group-ring-cohomology)

$$
H^{j+1}(H;\mathbb ZH)\cong H^j(N;\mathbb ZN)
$$

as [abelian groups](../../../group.md#abelian-group). Moreover $H^2(N;\mathbb ZN)\ne0$. Here is a useful proof of that last point: if top [cohomology](../../../cohomology.md) of a finite [projective resolution](../../../algebra.md#projective-resolution) were zero, its last dual differential would be onto. Its target is projective, so that differential splits. Dualizing back splits the last injection of the original resolution, shortening it and contradicting [integral cohomological dimension](../../../group-theory.md#integral-cohomological-dimension-of-a-group) two.

It follows that $H^3(H;\mathbb ZH)\ne0$, and hence $\operatorname{cd}H=3$. Strebel's theorem forces $H$ to have finite index in $G$. It is therefore itself a $PD^3$ group, by [finite-index invariance of Poincare duality for torsion-free groups](../../../group-theory.md#finite-index-invariance-of-poincare-duality-for-torsion-free-groups). The displayed shift now makes $H^j(N;\mathbb ZN)$ zero except for $j=2$, where it is $\mathbb Z$. Together with its finite [projective resolution](../../../algebra.md#projective-resolution), this proves

$$
\boxed{N\text{ is either free or a }PD^2\text{ group}.}
$$

The [classification of two-dimensional Poincare duality groups](../../../group-theory.md#classification-of-two-dimensional-poincare-duality-groups) identifies the latter with the [fundamental group](../../../algebraic-topology.md#fundamental-group) of a closed [aspherical](../../../algebraic-topology.md#aspherical-space) surface. This classification includes orientation-twisted [surface groups](../../../algebraic-topology.md#fundamental-group-of-a-surface); it does not include the two-sphere or real projective plane, whose [fundamental groups](../../../algebraic-topology.md#fundamental-group) do not have [integral cohomological dimension](../../../group-theory.md#integral-cohomological-dimension-of-a-group) two.

In this latter case we have also proved that $G/N$ is virtually infinite cyclic, since $H/N=\langle\bar t\rangle$ has finite index. If necessary replace the [surface group](../../../algebraic-topology.md#fundamental-group-of-a-surface) by its characteristic index-two orientable subgroup and take the subgroup generated by it and $t$. This still has finite index in $G$ and is a semidirect product of an orientable closed [aspherical](../../../algebraic-topology.md#aspherical-space) [surface group](../../../algebraic-topology.md#fundamental-group-of-a-surface) by $\mathbb Z$. The [Dehn-Nielsen-Baer theorem for closed orientable surfaces](../../../algebraic-topology.md#dehn-nielsen-baer-theorem-for-closed-orientable-surfaces) realizes the [outer automorphism](../../../group-theory.md#outer-automorphism-of-a-group) defined by conjugation by $t$ as a surface [homeomorphism](../../../topology.md#homeomorphism) $f$. For the [torus](../../../topology.md#torus) this is just realization of $GL_2(\mathbb Z)$ by linear [homeomorphisms](../../../topology.md#homeomorphism). Changing the chosen lift accounts for an [inner automorphism](../../../group-theory.md#inner-automorphism). The [mapping torus](../../../algebraic-topology.md#mapping-torus)

$$
M_f=(S\times[0,1])/((x,1)\sim(f(x),0))
$$

is a surface bundle over $S^1$ with [fundamental group](../../../algebraic-topology.md#fundamental-group) $\pi_1(S)\rtimes_{f_*}\mathbb Z$. Thus **a [finite-index subgroup](../../../group.md#finite-index-subgroup) of $G$ is the [fundamental group](../../../algebraic-topology.md#fundamental-group) of a surface fibration over the circle**. Taking a further double cover of the base if required makes the [monodromy](../../../complex-analysis.md#monodromy) orientation-preserving.

## 4

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the [Loop theorem](../../../topology.md#loop-theorem), start with a nullhomotopy $f:(D^2,\partial D^2)\to(M,\partial M)$ whose boundary represents a nontrivial boundary-group element. The required conclusion is an embedded [compression disk](../../../topology.md#compression-disk), whose boundary may differ from that original loop. A tower proof proceeds as follows.

Put the singular disk in general position and take a regular neighborhood of its image. Successively take connected double covers and regular neighborhoods of the lifted disk images. Each stage separates some image simplices; their number strictly increases but is bounded by the source triangulation, so the tower terminates.

At the top there is no connected double cover, hence $H^1(-;\mathbb Z/2)=0$. Poincare-Lefschetz duality makes every boundary component a sphere. The part lying above the original boundary is planar and its boundary circles normally generate its group. Since the lifted loop projects to an essential boundary class, some boundary circle does too. Cap that circle on the sphere and push the disk inward.

Descend each double cover. The projected embedded disk has only double arcs and circles. Innermost disk exchanges and cut-and-paste surgeries remove these. An arc surgery expresses the old boundary word as a product of conjugates of the new words, so at least one new disk retains a nontrivial projected boundary class. Circle surgery retains that class. Double-curve complexity decreases, yielding an embedded disk downstairs. Iterating reaches the required [compression disk](../../../topology.md#compression-disk) in $M$.

Now let $E$ be a [knot exterior](../../../knot-theory.md#knot-exterior), and choose a meridian $\mu$ and [Seifert longitude](../../../knot-theory.md#seifert-longitude) $\lambda$ on $\partial E$. The [homology](../../../homology.md) of the exterior is $\mathbb Z$, measured by linking number with the [knot](../../../knot-theory.md#knot): $\mu$ maps to a generator and $\lambda$ to zero. This follows from [Alexander duality](../../../cohomology.md#alexander-duality), or from a [Seifert surface](../../../knot-theory.md#seifert-surface) giving the [Seifert longitude](../../../knot-theory.md#seifert-longitude) and the linking homomorphism.

If $\pi_1(\partial E)\to\pi_1(E)$ were not injective, the [Loop theorem](../../../topology.md#loop-theorem) would supply a properly embedded disk $D$ with essential boundary on the [torus](../../../topology.md#torus). An essential simple curve on a [torus](../../../topology.md#torus) has primitive slope $a\mu+b\lambda$, with $\gcd(a,b)=1$. Since $\partial D$ bounds a disk in the exterior, its [homology](../../../homology.md) image is zero, forcing $a=0$ and $b=\pm1$. Thus $\partial D$ is a [Seifert longitude](../../../knot-theory.md#seifert-longitude). Inside the tubular [solid torus](../../../topology.md#solid-torus) it cobounds an embedded annulus with the core [knot](../../../knot-theory.md#knot). Joining that annulus to $D$, and smoothing their common boundary, gives an embedded spanning disk for the [knot](../../../knot-theory.md#knot) in $S^3$. A [knot](../../../knot-theory.md#knot) bounding such a disk is the [unknot](../../../knot-theory.md#unknot). Contraposition proves

$$
\boxed{K\text{ nontrivial}\quad\Longrightarrow\quad
\pi_1(\partial E)\hookrightarrow\pi_1(E).}
$$

Finally, $S^3\setminus K$ deformation retracts onto its exterior, so their [fundamental groups](../../../algebraic-topology.md#fundamental-group) agree. For the [unknot](../../../knot-theory.md#unknot) the exterior is a [solid torus](../../../topology.md#solid-torus), with [fundamental group](../../../algebraic-topology.md#fundamental-group) $\mathbb Z$. Conversely, if the knot-complement group were $\mathbb Z$, it could not contain an injected subgroup $\pi_1(\partial E)=\mathbb Z^2$. The preceding result therefore forces the [knot](../../../knot-theory.md#knot) to be trivial. Hence

$$
\boxed{K\text{ is unknotted}\iff\pi_1(S^3\setminus K)\cong\mathbb Z.}
$$

Merely having [homology](../../../homology.md) $\mathbb Z$ would not suffice: every [knot exterior](../../../knot-theory.md#knot-exterior) has that [homology](../../../homology.md).

## 5

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a connected smooth [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) $(M,g)$ without boundary, let $I(M)$ be the group of all global [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism) $f$ with $f^*g=g$, endowed with its [compact-open topology](../../../real-analysis.md#compact-open-topology). Equivalently these maps preserve the intrinsic distance; the [Myers-Steenrod theorem](../../../riemannian-geometry.md#myers-steenrod-theorem) supplies smoothness of distance-preserving bijections and makes $I(M)$ a finite-dimensional [Lie group](../../../lie-theory.md#lie-group) acting smoothly. The group is metric-dependent: a topological manifold can carry a very symmetric metric or one with no continuous symmetries. Connectedness matters here. With infinitely many identical disconnected components, permutations of those components can produce a group which is not a finite-dimensional [Lie group](../../../lie-theory.md#lie-group).

An [isometry](../../../riemannian-geometry.md#isometry) is determined by its value and derivative at one point. To prove this, suppose $f(p)=p$ and $df_p=I$. Preservation of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) gives

$$
f(\exp_p v)=\exp_p(df_pv)=\exp_pv
$$

where the [exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) is defined locally. Thus $f$ is the identity in a normal neighborhood of $p$. The set where its value and derivative agree with the identity is both closed and, by the same argument, open. Connectedness makes it all of $M$. No completeness is needed for this determination argument.

The stabilizer $I(M)_p$ consequently acts faithfully and orthogonally on $T_pM$, so embeds in $O(n)$. More generally an [isometry](../../../riemannian-geometry.md#isometry) takes a chosen [orthonormal frame](../../../general-relativity.md#orthonormal-frame-in-spacetime) at $p$ to one at its image point, providing an injective map into the [orthonormal frame bundle](../../../fiber-bundle.md#orthonormal-frame-bundle). It is a smooth embedding, and the full [isometry](../../../riemannian-geometry.md#isometry) action is proper. The orbit-stabilizer dimension formula therefore gives

$$
\boxed{\dim I(M)\leq n+\frac{n(n-1)}2=\frac{n(n+1)}2.}
$$

Isotropy is compact. If $M$ is compact then $I(M)$ itself is compact, by the same frame description or Arzela-Ascoli applied to [isometries](../../../riemannian-geometry.md#isometry) and their inverses. Properness also means that the quotient by [isometries](../../../riemannian-geometry.md#isometry) has well-controlled local orbit structure, even though orbit dimensions may vary.

The infinitesimal equation is the [Killing equation](../../../general-relativity.md#killing-equation). Differentiating $f_t^*g=g$ at zero gives

$$
\mathcal L_Xg=0,\qquad \nabla_iX_j+\nabla_jX_i=0.
$$

Conversely a vector field satisfying this equation has local flows preserving the metric. A global one-parameter subgroup requires the field to be complete. On a geodesically complete manifold every [Killing field](../../../general-relativity.md#killing-vector-field) is complete: its length is constant along each of its own trajectories, so a finite-time trajectory has bounded speed and stays in a closed bounded ball. The [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) makes that ball compact, and the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) can then be continued. The caveat is real: on the Euclidean interval $(0,1)$, the field $\partial_x$ is Killing but its translations are not globally defined for all time. This illustrates [Killing fields on incomplete manifolds need not generate global isometries](../../../general-relativity.md#killing-fields-on-incomplete-manifolds-need-not-generate-global-isometries).

The [Killing transport](../../../general-relativity.md#killing-transport) identities determine a [Killing field](../../../general-relativity.md#killing-vector-field) from $X(p)$ and the skew-adjoint map $(\nabla X)_p$. Along a [geodesic](../../../riemannian-geometry.md#geodesic) the field is a [Jacobi field](../../../general-relativity.md#jacobi-field), so uniqueness for its second-order [differential equation](../../../differential-equation.md) propagates these [initial data](../../../general-relativity.md#initial-data-in-general-relativity). They have $n+n(n-1)/2$ components, reproducing the dimension bound infinitesimally. The important distinction on an incomplete manifold is between all local Killing solutions and the [Lie algebra](../../../lie-algebra.md) of complete global [isometry](../../../riemannian-geometry.md#isometry) flows.

In dimension three the bound is six, and rotational isotropy gives stronger information. The [Lie subalgebras](../../../lie-algebra.md#lie-subalgebra) of $\mathfrak{so}(3)$ have dimensions zero, one or three: identifying the bracket with the cross product, a two-plane is not closed under brackets. Suppose $\dim I(M)=5$. Since an orbit has dimension at most three, its stabilizer would have dimension at least two, and hence exactly three. Its connected isotropy acts as all of $SO(3)$ on the tangent space. But the orbit tangent space is invariant under that action and would have dimension $5-3=2$, impossible because the standard rotational representation is irreducible. Therefore **dimension five cannot occur**.

If the dimension is six, each orbit has dimension three and each stabilizer dimension three. All orbits are open, so connectedness makes the action transitive. At each point the isotropy is transitive on tangent two-planes, forcing [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) to be independent of the plane; transitivity makes its value independent of the point. Thus a maximally symmetric connected [three-manifold](../../../topology.md#3-manifold) has [constant sectional curvature](../../../general-relativity.md#constant-sectional-curvature). Homogeneous [Riemannian manifolds](../../../riemannian-geometry.md#riemannian-manifold) are complete, so its [simply connected](../../../algebraic-topology.md#simply-connected-space) cover is the round sphere, [Euclidean space](../../../functional-analysis.md#euclidean-norm) or [hyperbolic space](../../../geometry-and-topology.md#hyperbolic-space) after normalization. Conversely these three [simply connected](../../../algebraic-topology.md#simply-connected-space) metrics attain dimension six:

$$
I(S^3)=O(4),\qquad I(\mathbb R^3)=\mathbb R^3\rtimes O(3),\qquad
I(\mathbb H^3)=O^+(3,1).
$$

Here $O^+(3,1)$ preserves the chosen sheet of the hyperboloid; it includes orientation-reversing hyperbolic [isometries](../../../riemannian-geometry.md#isometry). Constant curvature alone does not imply that a quotient retains six-dimensional global symmetry.

Dimension four likewise forces transitivity: stabilizer dimension three would give a one-dimensional invariant orbit tangent space, again impossible for full rotational isotropy. The stabilizer thus has dimension one and the orbits are three-dimensional. Typical four-dimensional [isometry groups](../../../riemannian-geometry.md#isometry-group) occur for $S^2\times\mathbb R$ and $\mathbb H^2\times\mathbb R$, where the factor groups have dimensions three and one. The usual Nil metric has three translation symmetries and one rotational isotropy symmetry. In centred Heisenberg coordinates it is

$$
g=dx^2+dy^2+\bigl(dt+\tfrac12(y\,dx-x\,dy)\bigr)^2,
$$

which exhibits the horizontal rotations. Its distinct vertical and horizontal Ricci eigenvalues bound continuous isotropy by that rotation group, so its full [isometry](../../../riemannian-geometry.md#isometry) dimension is four. Standard metrics on $\widetilde{SL_2(\mathbb R)}$ and nonround Berger spheres also have dimension four. The standard Sol geometry has a three-dimensional translation group and only finite isotropy, giving dimension three. These examples show how a preferred vertical direction reduces rotational symmetry.

The [isometry dimensions in dimension three](../../../riemannian-geometry.md#isometry-dimensions-in-dimension-three) are precisely $0,1,2,3,4,6$, all realizable. A compact [hyperbolic three-manifold](../../../topology.md#hyperbolic-three-manifold) gives zero; the product of a circle and a closed hyperbolic surface gives one. For dimension two take $T^2\times(0,1)$ with

$$
g=dt^2+e^{2t}\,dx^2+e^{4t}\,dy^2.
$$

Its [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) is the constant $-14$, but its Ricci eigenvalues are the distinct constants $-3,-6,-5$ in the two horizontal directions and the vertical direction. Hence connected isotropy is trivial and possible [isometries](../../../riemannian-geometry.md#isometry) preserve these line distributions. A local [isometry](../../../riemannian-geometry.md#isometry) preserving them has $t'=t+c$ and would require constant dilations $e^{-c}$ and $e^{-2c}$ of the two circle coordinates. A global circle [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) with such a constant dilation has degree $\pm1$, forcing $c=0$. The identity component is therefore exactly the two circle translations. A flat three-torus gives dimension three; $S^2\times\mathbb R$ gives four; a [simply connected](../../../algebraic-topology.md#simply-connected-space) constant-curvature model gives six. This construction distinguishes local homogeneity from the smaller global [isometry group](../../../riemannian-geometry.md#isometry-group).

For quotients, let a complete [simply connected](../../../algebraic-topology.md#simply-connected-space) [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) $X$ cover $M=X/\Gamma$. Every [isometry](../../../riemannian-geometry.md#isometry) of $M$ lifts to an [isometry](../../../riemannian-geometry.md#isometry) of $X$ which normalizes the [deck transformation group](../../../algebraic-topology.md#deck-transformation-group). Conversely, every normalizing [isometry](../../../riemannian-geometry.md#isometry) descends. Two lifts differ by a [deck transformation](../../../algebraic-topology.md#deck-transformation), giving the [isometry group of a Riemannian quotient](../../../riemannian-geometry.md#isometry-group-of-a-riemannian-quotient) formula

$$
\boxed{I(X/\Gamma)=N_{I(X)}(\Gamma)/\Gamma.}
$$

Thus one should not replace the [isometry group](../../../riemannian-geometry.md#isometry-group) of a quotient by that of its model geometry. For a [flat torus](../../../second-fundamental-form.md#flat-torus), for example,

$$
I(\mathbb R^3/\Lambda)=(\mathbb R^3/\Lambda)\rtimes\{R\in O(3):R\Lambda=\Lambda\}.
$$

The second factor is finite, whereas translations give the three-dimensional identity component.

There is a useful curvature test for [compact manifolds](../../../differential-geometry.md#compact-manifold). Contracting and differentiating the [Killing equation](../../../general-relativity.md#killing-equation) gives $\nabla^*\nabla X=\operatorname{Ric}(X)$, with the nonnegative rough-Laplacian convention. Integration yields the [integrated Bochner identity for Killing fields](../../../general-relativity.md#bochner-identity-for-killing-vector-fields)

$$
\int_M|\nabla X|^2\,dV=\int_M\operatorname{Ric}(X,X)\,dV.
$$

If [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) is negative definite, no nonzero [Killing field](../../../general-relativity.md#killing-vector-field) exists. The compact [isometry group](../../../riemannian-geometry.md#isometry-group) then has dimension zero and is finite. This explains why closed hyperbolic manifolds have finite global symmetry, despite the six-dimensional [isometry group](../../../riemannian-geometry.md#isometry-group) of their [universal cover](../../../algebraic-topology.md#universal-cover). Compactness is essential to this conclusion.

For a compact [flat Riemannian manifold](../../../second-fundamental-form.md#flat-manifold), the same identity makes every [Killing field](../../../general-relativity.md#killing-vector-field) parallel. Parallel fields are exactly the vectors fixed by linear holonomy. Therefore

$$
\boxed{\dim I(M)_0=\dim(\mathbb R^3)^{\operatorname{Hol}(M)}.}
$$

Applied to the six flat types of Question 1, this gives dimensions three for the [torus](../../../topology.md#torus), one for each of the four nontrivial cyclic types, and zero for the [Hantzsche-Wendt manifold](../../../second-fundamental-form.md#hantzsche-wendt-manifold). These are identity-component dimensions; disconnected finite symmetries can still be present. Local curvature symmetry, global deck-group constraints, and completeness thus play different roles in determining the [isometry group](../../../riemannian-geometry.md#isometry-group).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
