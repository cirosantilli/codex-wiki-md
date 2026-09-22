<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use integral coefficients throughout, allowing a nontrivial orientation character. A dimension-$d$ [Poincare duality group](../../../../../poincare-duality-group.md) has a finite resolution by finitely generated projective group-ring modules and

$$
H^j(G;\mathbb ZG)=0\quad(j\ne d),\qquad H^d(G;\mathbb ZG)\cong\mathbb Z
$$

as [abelian groups](../../../../../abelian-group.md). The action on the top copy of $\mathbb Z$ may be by signs. This group-ring criterion is particularly suited to the [Lyndon–Hochschild–Serre spectral sequence](../../../../../lyndon-hochschild-serre-spectral-sequence.md).

Apply that sequence to the extension with coefficient module $\mathbb ZG$:

$$
E_2^{a,b}=H^a\bigl(Q;H^b(N;\mathbb ZG)\bigr)
\Longrightarrow H^{a+b}(G;\mathbb ZG).
$$

As an $N$-module, $\mathbb ZG$ is a [direct sum](../../../../../direct-sum.md) of copies of $\mathbb ZN$ indexed by the cosets in $Q$. [Cohomology](../../../../../cohomology-split.md) of $N$ commutes with this [direct sum](../../../../../direct-sum.md) because its [projective resolution](../../../../../projective-resolution.md) is finitely generated. Hence the inner [cohomology](../../../../../cohomology-split.md) vanishes except when $b=n$, where it is a [direct sum](../../../../../direct-sum.md) of rank-one groups indexed by $Q$. The $Q$-action shifts these summands freely and transitively, with possible signs from the orientation module. Choosing a generator in one summand and transporting it by $Q$ identifies the resulting left $Q$-module with its regular module $\mathbb ZQ$. The residual right [group action](../../../../../group-action.md) records the orientation twist; it need not be trivial.

Now the duality of $Q$ says that the only nonzero $E_2$ term is $(a,b)=(q,n)$ and that this term is $\mathbb Z$ as an [abelian group](../../../../../abelian-group.md). No differential can enter or leave it. Therefore $H^*(G;\mathbb ZG)$ has exactly the duality pattern in degree $n+q$. The usual extension-resolution construction also supplies a resolution by [finitely generated projective modules](../../../../../finite-projective-module.md): combine the finite [kernel](../../../../../kernel-of-a-linear-map.md) and quotient resolutions, lift the quotient differentials and add the necessary [homotopy](../../../../../homotopy.md) corrections. Its total length is at most $n+q$. Alternatively, the same [spectral sequence](../../../../../spectral-sequence.md) for arbitrary coefficient modules gives the dimension bound, while the extension finiteness lemma supplies finite generation of the resolution. The surviving top term makes the bound sharp. This proves the [extension rule for Poincare duality groups](../../../../../extension-rule-for-poincare-duality-groups.md):

$$
\boxed{G\text{ is a }PD^{n+q}\text{ group}.}
$$

Requiring a trivial top orientation action would need an additional orientation condition; the untwisted conclusion is not implicit in the hypotheses.

We next need two precise auxiliary dimension results. The [Strebel infinite-index subgroup theorem](../../../../../strebel-infinite-index-subgroup-theorem.md) says that an infinite-index subgroup of an integral $PD^d$ group has [integral cohomological dimension](../../../../../integral-cohomological-dimension-of-a-group.md) at most $d-1$. The [Stallings-Swan theorem](../../../../../stallings-swan-theorem.md) says that a group of [integral cohomological dimension](../../../../../integral-cohomological-dimension-of-a-group.md) at most one is free, including the trivial group. Since $G/N$ contains an element of infinite order, $N$ has infinite index in $G$, so $\operatorname{cd}N\leq2$. If its dimension is at most one, the required free-group conclusion follows, with finite rank because $N$ is finitely presented.

Suppose instead that $\operatorname{cd}N=2$. [Finite presentation](../../../../../finite-presentation-of-a-module.md) gives a partial [free resolution](../../../../../free-resolution.md) with finitely generated modules through degree two. The [kernel](../../../../../kernel-of-a-linear-map.md) in degree one is finitely generated and, because the [integral cohomological dimension](../../../../../integral-cohomological-dimension-of-a-group.md) is two, projective. Truncating at this [kernel](../../../../../kernel-of-a-linear-map.md) gives a finite resolution by [finitely generated projective modules](../../../../../finite-projective-module.md). Thus $N$ has the finiteness needed for group-ring [cohomology](../../../../../cohomology-split.md) to commute with [direct sums](../../../../../direct-sum.md).

Choose an infinite-order element $\bar t\in G/N$, lift it to $t\in G$, and let $H$ be the preimage of $\langle\bar t\rangle$. Then $H=N\rtimes\langle t\rangle$. Restriction of $\mathbb ZH$ to $N$ yields copies of $\mathbb ZN$ indexed by all powers of $t$. For every $j$, the quotient generator acts on $H^j(N;\mathbb ZH)$ by shifting this [direct sum](../../../../../direct-sum.md), possibly with an automorphism on each copy. Its invariants vanish, since an invariant finite-support sequence must be zero. Its coinvariants are one copy of $H^j(N;\mathbb ZN)$: the shift relations identify successive copies, and any twists can be removed by transporting the identifications along the integer index.

The [infinite cyclic group](../../../../../infinite-cyclic-group.md) has [integral cohomological dimension](../../../../../integral-cohomological-dimension-of-a-group.md) one, so only columns zero and one occur in the [spectral sequence](../../../../../spectral-sequence.md). Column zero vanishes and column one consists of these coinvariants. We obtain the [cyclic-extension shift of group-ring cohomology](../../../../../cyclic-extension-shift-of-group-ring-cohomology.md)

$$
H^{j+1}(H;\mathbb ZH)\cong H^j(N;\mathbb ZN)
$$

as [abelian groups](../../../../../abelian-group.md). Moreover $H^2(N;\mathbb ZN)\ne0$. Here is a useful proof of that last point: if top [cohomology](../../../../../cohomology-split.md) of a finite [projective resolution](../../../../../projective-resolution.md) were zero, its last dual differential would be onto. Its target is projective, so that differential splits. Dualizing back splits the last injection of the original resolution, shortening it and contradicting [integral cohomological dimension](../../../../../integral-cohomological-dimension-of-a-group.md) two.

It follows that $H^3(H;\mathbb ZH)\ne0$, and hence $\operatorname{cd}H=3$. Strebel's theorem forces $H$ to have finite index in $G$. It is therefore itself a $PD^3$ group, by [finite-index invariance of Poincare duality for torsion-free groups](../../../../../finite-index-invariance-of-poincare-duality-for-torsion-free-groups.md). The displayed shift now makes $H^j(N;\mathbb ZN)$ zero except for $j=2$, where it is $\mathbb Z$. Together with its finite [projective resolution](../../../../../projective-resolution.md), this proves

$$
\boxed{N\text{ is either free or a }PD^2\text{ group}.}
$$

The [classification of two-dimensional Poincare duality groups](../../../../../classification-of-two-dimensional-poincare-duality-groups.md) identifies the latter with the [fundamental group](../../../../../fundamental-group.md) of a closed [aspherical](../../../../../aspherical-space.md) surface. This classification includes orientation-twisted [surface groups](../../../../../fundamental-group-of-a-surface.md); it does not include the two-sphere or real projective plane, whose [fundamental groups](../../../../../fundamental-group.md) do not have [integral cohomological dimension](../../../../../integral-cohomological-dimension-of-a-group.md) two.

In this latter case we have also proved that $G/N$ is virtually infinite cyclic, since $H/N=\langle\bar t\rangle$ has finite index. If necessary replace the [surface group](../../../../../fundamental-group-of-a-surface.md) by its characteristic index-two orientable subgroup and take the subgroup generated by it and $t$. This still has finite index in $G$ and is a semidirect product of an orientable closed [aspherical](../../../../../aspherical-space.md) [surface group](../../../../../fundamental-group-of-a-surface.md) by $\mathbb Z$. The [Dehn-Nielsen-Baer theorem for closed orientable surfaces](../../../../../dehn-nielsen-baer-theorem-for-closed-orientable-surfaces.md) realizes the [outer automorphism](../../../../../outer-automorphism-of-a-group.md) defined by conjugation by $t$ as a surface [homeomorphism](../../../../../homeomorphism.md) $f$. For the [torus](../../../../../torus.md) this is just realization of $GL_2(\mathbb Z)$ by linear [homeomorphisms](../../../../../homeomorphism.md). Changing the chosen lift accounts for an [inner automorphism](../../../../../inner-automorphism.md). The [mapping torus](../../../../../mapping-torus.md)

$$
M_f=(S\times[0,1])/((x,1)\sim(f(x),0))
$$

is a surface bundle over $S^1$ with [fundamental group](../../../../../fundamental-group.md) $\pi_1(S)\rtimes_{f_*}\mathbb Z$. Thus **a [finite-index subgroup](../../../../../finite-index-subgroup.md) of $G$ is the [fundamental group](../../../../../fundamental-group.md) of a surface fibration over the circle**. Taking a further double cover of the base if required makes the [monodromy](../../../../../monodromy.md) orientation-preserving.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
