<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a cohomological [spectral sequence](../../../../../spectral-sequence.md), $d_r:E_r^{p,q}\to E_r^{p+r,q-r+1}$ and the next page is its cohomology. In the bounded setting, [convergence of a spectral sequence](../../../../../convergence-of-a-spectral-sequence.md) to $H^*$ means that each $H^n$ has a finite decreasing, exhaustive and separated filtration with

$$
\boxed{E_\infty^{p,q}\cong F^pH^{p+q}/F^{p+1}H^{p+q}.}
$$

Here $E_\infty^{p,q}$ is the eventual stable value. This determines the [associated graded module](../../../../../associated-graded-module.md) of $H^n$, rather than automatically a canonical direct-sum decomposition of $H^n$. For unbounded filtrations additional completeness/convergence conditions are necessary; boundedness removes those issues here.

The [bounded filtered-complex convergence theorem](../../../../../bounded-filtered-complex-convergence-theorem.md) states the following. If $F^pC$ is a decreasing filtration by [cochain subcomplexes](../../../../../cochain-subcomplex.md), preserved by the differential, finite in each cochain degree (uniform bounds $F^aC=C$, $F^bC=0$ are sufficient), then there is a [spectral sequence](../../../../../spectral-sequence.md)

$$
E_0^{p,q}=F^pC^{p+q}/F^{p+1}C^{p+q},\qquad E_1^{p,q}=H^{p+q}(F^pC/F^{p+1}C),\qquad E_r^{p,q}\Rightarrow H^{p+q}(C).
$$

The abutment filtration is $F^pH^n(C)=\operatorname{im}[H^n(F^pC)\to H^n(C)]$. Its finite length ensures stabilization and the displayed limiting-page identification. The [filtered cochain complex](../../../../../filtered-cochain-complex.md) need not itself be bounded in cochain degree. In the degreewise finite version, the bounds in degrees $n-1,n,n+1$ suffice to stabilize the terms of total degree $n$.

For a [double cochain complex](../../../../../double-cochain-complex.md) $D^{p,q}$ bounded in both indices, form the [total cochain complex](../../../../../total-cochain-complex.md) $\operatorname{Tot}^nD=\bigoplus_{p+q=n}D^{p,q}$ with anticommuting differentials $d_h,d_v$ and total differential $d_h+d_v$. If the original differentials commute, inserting the usual sign in one of them gives this convention. Filtering by the first index gives $E_1^{p,q}=H_v^q(D^{p,*})$ and then $E_2^{p,q}=H_h^p(H_v^qD)$. Filtering by the second index gives the [spectral sequence](../../../../../spectral-sequence.md) taking horizontal cohomology first and vertical cohomology next. Both filtrations are finite, so both converge to $H^*(\operatorname{Tot}D)$. This is the [two spectral sequences of a bounded double complex](../../../../../two-spectral-sequences-of-a-bounded-double-complex.md) construction.

**The printed left/left tensor expression needs a handedness repair.** Over an arbitrary ring, a [tensor product of modules](../../../../../tensor-product-of-modules.md) over $R$ pairs a right module with a left module. To retain the order of the printed formula, take $P$ to be a bounded [cochain complex](../../../../../cochain-complex.md) of projective right $R$-modules and $M$ a left $R$-module. Alternatively, keep $P$ left, take $M$ right, and write $M\otimes_RP$ and $\operatorname{Tor}^R_{-p}(M,H^qP)$. For a commutative ring no repair is needed. We prove the first, correctly typed formulation.

Finite [projective dimension](../../../../../projective-dimension.md) gives a finite [projective resolution](../../../../../projective-resolution.md) $Q_\bullet\to M$ by left modules. Form $D^{p,q}=P^q\otimes_RQ_{-p}$ for $-d\leq p\leq0$. On $x\otimes y$ take $d_v=d_P\otimes1$ and $d_h=(-1)^q1\otimes d_Q$. These anticommute, and the [double cochain complex](../../../../../double-cochain-complex.md) is bounded in both directions. Projective modules are [flat modules](../../../../../flat-module.md), so taking vertical cohomology first gives

$$
E_1^{p,q}=H^q(P)\otimes_R Q_{-p},\qquad\boxed{E_2^{p,q}=\operatorname{Tor}_{-p}^R(H^qP,M).}
$$

The first identification uses flatness of $Q_{-p}$; the second is the [Tor functor](../../../../../tor-functor.md) computed by resolving its left-module argument $M$. Balancedness of the [Tor functor](../../../../../tor-functor.md) allows either correctly sided projective resolution to compute it, by the double-resolution argument.

Taking horizontal cohomology first instead uses flatness of $P^q$. The resolution $Q_\bullet$ then leaves only $P^q\otimes_RM$ in column $p=0$. Its remaining differential is $d_P\otimes1$, so the augmentation $\operatorname{Tot}D\to P\otimes_RM$ is a [quasi-isomorphism](../../../../../quasi-isomorphism.md). Apply the convergence theorem to this underlying abelian-group double complex. The two [spectral sequences](../../../../../spectral-sequence.md) therefore prove **the Künneth spectral sequence**:

$$
\boxed{E_2^{p,q}=\operatorname{Tor}_{-p}^R(H^qP,M)\Rightarrow H^{p+q}(P\otimes_RM).}
$$

These are abelian groups in general; an extra module structure requires appropriate bimodule hypotheses. The index $p$ is nonpositive, so $-p$ is the nonnegative homological index of the [Tor functor](../../../../../tor-functor.md).

Finally write the [cycle modules](../../../../../cycle-module.md) as $Z^q=\ker d^q$ and the [boundary modules](../../../../../boundary-module.md) as $B^q=\operatorname{im}d^{q-1}$. If every [boundary module](../../../../../boundary-module.md) $B^q$ is projective, the [short exact sequence](../../../../../short-exact-sequence.md) $0\to Z^q\to P^q\to B^{q+1}\to0$ splits. Thus $Z^q$ is projective. The [short exact sequence](../../../../../short-exact-sequence.md) $0\to B^q\to Z^q\to H^qP\to0$ is now a length-one [projective resolution](../../../../../projective-resolution.md), so $\operatorname{Tor}_i^R(H^qP,M)=0$ for $i\geq2$. The $E_2$ page occupies only columns $p=-1,0$. Every $d_r$ for $r\geq2$ goes $r$ columns to the right, hence has zero source or zero target. Therefore

$$
\boxed{E_2=E_\infty.}
$$

This [two-column degeneration of a Künneth spectral sequence](../../../../../two-column-degeneration-of-a-kunneth-spectral-sequence.md) gives the edge [short exact sequences](../../../../../short-exact-sequence.md)

$$
0\longrightarrow H^nP\otimes_RM\longrightarrow H^n(P\otimes_RM)\longrightarrow\operatorname{Tor}_1^R(H^{n+1}P,M)\longrightarrow0.
$$

Degeneration itself does not supply a canonical splitting. Projective boundaries also do not force $H^qP$ to be projective: a complex with differential multiplication by $2$ over $\mathbb Z$ has projective boundary but a $\mathbb Z/2\mathbb Z$ cohomology group.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
