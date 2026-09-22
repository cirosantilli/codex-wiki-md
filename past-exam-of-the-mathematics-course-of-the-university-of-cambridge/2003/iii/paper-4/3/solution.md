<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $B$ be a [nondegenerate](../../../../../nondegenerate-bilinear-form.md) [alternating bilinear form](../../../../../alternating-bilinear-form.md) on $V$ of [dimension](../../../../../dimension-vector-space.md) $2m$ over $\mathbb F_q$. A [symplectic basis](../../../../../symplectic-basis.md) has $B(e_i,f_j)=\delta_{ij}$ and all $e_i,e_j$ and $f_i,f_j$ pairings zero. Such [bases](../../../../../basis.md) are built by choosing a nonzero $e_1$, finding $f_1$ with $B(e_1,f_1)=1$, and continuing in their nonsingular [orthogonal complement for a sesquilinear form](../../../../../orthogonal-complement-for-a-sesquilinear-form.md). In these coordinates the group preserving $B$ is

$$
Sp_{2m}(q)=\{g:g^{\mathsf T}Jg=J\},\qquad
J=\begin{pmatrix}0&I\\-I&0\end{pmatrix}.
$$

Its action on [symplectic bases](../../../../../symplectic-basis.md) is regular. There are $q^{2m}-1$ choices for $e_1$ and $q^{2m-1}$ for $f_1$, so induction gives the [finite symplectic group order](../../../../../finite-symplectic-group-order.md)

$$
|Sp_{2m}(q)|=(q^{2m}-1)q^{2m-1}|Sp_{2m-2}(q)|,
\qquad\boxed{|Sp_{2m}(q)|=q^{m^2}\prod_{j=1}^m(q^{2j}-1).}
$$

The [center of a group](../../../../../center-of-a-group.md) consists of $aI$ with $a^2=1$, and has order $\gcd(2,q-1)$. To see there are no other central elements, a central element commutes with every [symplectic transvection](../../../../../symplectic-transvection.md) and hence fixes every [symplectic transvection](../../../../../symplectic-transvection.md) center line; a [linear map](../../../../../linear-map.md) fixing every line is scalar. Consequently the [projective symplectic group over a finite field](../../../../../projective-symplectic-group-over-a-finite-field.md) has this order divided by $\gcd(2,q-1)$.

Here is a proof of the main ingredients in simplicity. The [symplectic transvection](../../../../../symplectic-transvection.md)

$$
T_{v,c}(x)=x+cB(x,v)v
$$

preserves $B$, has inverse $T_{v,-c}$, and fixes $v^\perp$ pointwise. These transformations generate $Sp_{2m}(q)$. Indeed if $B(u,w)\ne0$, then $T_{w-u,\,1/B(u,w)}$ sends $u$ to $w$. If the pairing is zero, choose an intermediate vector having nonzero pairing with both, so two [symplectic transvections](../../../../../symplectic-transvection.md) suffice. This aligns the first vector of any [symplectic basis](../../../../../symplectic-basis.md). For partners $f,f'$ of the same $e$, their difference lies in $e^\perp$. If $B(f,f')\ne0$ a [symplectic transvection](../../../../../symplectic-transvection.md) centered at $f'-f$ aligns them and fixes $e$. If it is zero and the partners differ, $h=f+e$ pairs nontrivially with both and still pairs to one with $e$; two such [symplectic transvections](../../../../../symplectic-transvection.md) work. After fixing the pair, induction in its [orthogonal complement for a sesquilinear form](../../../../../orthogonal-complement-for-a-sesquilinear-form.md) aligns the rest of the [basis](../../../../../basis.md).

The projective action on one-spaces is [faithful](../../../../../faithful-group-action.md). For $m\ge2$, a line [stabilizer](../../../../../stabilizer-subgroup.md) has three orbits: the line itself, the other lines perpendicular to it, and the lines not perpendicular to it. [Witt's lemma](../../../../../witt-s-theorem.md) proves transitivity within the latter two orbits by matching the two-dimensional restricted form. This action is [primitive](../../../../../primitive-group-action.md). A block containing distinct perpendicular lines $L,M$ is invariant under both [stabilizers](../../../../../stabilizer-subgroup.md) and therefore contains a line perpendicular to $M$ but not to $L$. A block containing distinct nonperpendicular lines likewise contains a line perpendicular to $L$ but not to $M$, by using the $M$ [stabilizer](../../../../../stabilizer-subgroup.md). Such lines exist by nonsingularity in [dimension](../../../../../dimension-vector-space.md) at least four. Either possibility makes the block contain both nontrivial [stabilizer](../../../../../stabilizer-subgroup.md) orbits, hence every line. For $m=1$ the action on the [projective line](../../../../../projective-line.md) is [two-transitive](../../../../../two-transitive-group-action.md) and thus [primitive](../../../../../primitive-group-action.md).

[Symplectic transvections](../../../../../symplectic-transvection.md) with one fixed center line form an [Abelian](../../../../../abelian-group.md) [normal subgroup](../../../../../normal-subgroup.md) of its [stabilizer](../../../../../stabilizer-subgroup.md), and their conjugates generate the whole group. The [Iwasawa simplicity lemma](../../../../../iwasawa-simplicity-lemma.md) now reduces simplicity to being [perfect](../../../../../perfect-group.md). Its short proof is useful: any nontrivial [normal subgroup](../../../../../normal-subgroup.md) of a [faithful](../../../../../faithful-group-action.md) [primitive](../../../../../primitive-group-action.md) group is transitive, since its orbits are blocks. Writing $G=NH$, where $H$ is a point [stabilizer](../../../../../stabilizer-subgroup.md), shows that all conjugates of the specified [Abelian](../../../../../abelian-group.md) [subgroup](../../../../../subgroup.md) have the same image modulo $N$. Thus $G/N$ is [Abelian](../../../../../abelian-group.md). If $G$ is [perfect](../../../../../perfect-group.md), $N=G$.

The groups can also be shown to be [perfect](../../../../../perfect-group.md) concretely. For $q>3$ choose $a$ with $a^2\ne1$ and let $D$ scale $e$ by $a$ and $f$ by $a^{-1}$. Then

$$
DT_{e,c}D^{-1}T_{e,c}^{-1}=T_{e,(a^2-1)c},
$$

so every [symplectic transvection](../../../../../symplectic-transvection.md) is a [group commutator](../../../../../group-commutator.md). For $q=3,m\ge2$, [symplectic transvections](../../../../../symplectic-transvection.md) of coefficient one are conjugate, have order three, and the four with centers $e_1,e_2,e_1+e_2,e_1-e_2$ in a two-dimensional [totally isotropic subspace](../../../../../totally-isotropic-subspace.md) multiply to the identity. They commute, and the sum of their rank-one terms is zero modulo three. Their common class in the [abelianization](../../../../../abelianization.md) is therefore annihilated by both three and four, hence is zero. For $q=2,m\ge3$, use the seven nonzero vectors of a three-dimensional [totally isotropic subspace](../../../../../totally-isotropic-subspace.md). The [symplectic transvections](../../../../../symplectic-transvection.md) commute and their product is the identity, because each diagonal coefficient occurs four times and each cross coefficient twice. Their common abelianized class is annihilated by two and seven, hence is zero. Generation now proves these groups are [perfect](../../../../../perfect-group.md).

It follows that

$$
\boxed{PSp_{2m}(q)\text{ is simple except for }(m,q)=(1,2),(1,3),(2,2).}
$$

The exceptions are $S_3$, $A_4$ and $S_6$ respectively. For odd $q$ the full [symplectic group over a finite field](../../../../../symplectic-group-over-a-finite-field.md) has nontrivial [center of a group](../../../../../center-of-a-group.md), so simplicity refers to its [quotient group](../../../../../quotient-group.md); for even $q$ the [center of a group](../../../../../center-of-a-group.md) is trivial.

A [symplectic parabolic subgroup](../../../../../symplectic-parabolic-subgroup.md) stabilizes a flag of [totally isotropic subspaces](../../../../../totally-isotropic-subspace.md). The maximal such [parabolic subgroups](../../../../../parabolic-subgroup.md) $P_r$ stabilize a single $r$-space, $1\le r\le m$. In an adapted [basis](../../../../../basis.md) their [Levi subgroup](../../../../../levi-subgroup.md) is $GL_r(q)\times Sp_{2m-2r}(q)$, with an arbitrary block of $r(2m-2r)$ parameters and a remaining symmetric block of $r(r+1)/2$ parameters. Thus

$$
P_r=U_r\rtimes\bigl(GL_r(q)\times Sp_{2m-2r}(q)\bigr),\qquad
|U_r|=q^{2r(m-r)+r(r+1)/2}.
$$

These are the single-member flag [stabilizers](../../../../../stabilizer-subgroup.md), equivalently the standard maximal [parabolic subgroups](../../../../../parabolic-subgroup.md) obtained by omitting one node of the symplectic [Dynkin diagram](../../../../../dynkin-diagram.md). Two particular cases have transparent descriptions.

For the [symplectic point stabilizer](../../../../../symplectic-point-stabilizer.md), write $V=\langle e,f\rangle\perp W$. Its [unipotent radical](../../../../../unipotent-radical.md) consists of

$$
u(b,t):\quad e\mapsto e,\quad w\mapsto w-B(w,b)e,\quad f\mapsto f+b+te,
\qquad b\in W,\ t\in\mathbb F_q.
$$

All pairings are preserved by direct substitution. The product law is $(b,t)(b',t')=(b+b',t+t'+B(b,b'))$, so this radical has order $q^{2m-1}$. With [group commutator](../../../../../group-commutator.md) convention $uvu^{-1}v^{-1}$, its commutator has central parameter $2B(b,b')$: it is Heisenberg-type in odd [characteristic](../../../../../characteristic-of-a-field.md), but [Abelian](../../../../../abelian-group.md) in [characteristic](../../../../../characteristic-of-a-field.md) two. A [Levi subgroup](../../../../../levi-subgroup.md) scales $e,f$ inversely and acts as $Sp(W)$, giving

$$
\boxed{P_1=U_1\rtimes\bigl(\mathbb F_q^\times\times Sp_{2m-2}(q)\bigr),\qquad
[Sp_{2m}(q):P_1]=\frac{q^{2m}-1}{q-1}.}
$$

This index counts the one-spaces, all of which are isotropic for an [alternating bilinear form](../../../../../alternating-bilinear-form.md).

For a [Lagrangian subspace](../../../../../lagrangian-subspace.md) $E=\langle e_1,\ldots,e_m\rangle$, the [symplectic Lagrangian stabilizer](../../../../../symplectic-lagrangian-stabilizer.md) has block form

$$
\begin{pmatrix}A&AS\\0&A^{-\mathsf T}\end{pmatrix},\qquad
A\in GL_m(q),\quad S=S^{\mathsf T}.
$$

Substituting into $g^{\mathsf T}Jg=J$ proves both the inverse-transpose lower block and symmetry of $S$. The [unipotent radical](../../../../../unipotent-radical.md) is the additive group of [symmetric matrices](../../../../../symmetric-matrix.md), and $A$ acts by $S\mapsto ASA^{\mathsf T}$. Therefore

$$
\boxed{|P_m|=q^{m(m+1)/2}|GL_m(q)|,\qquad
[Sp_{2m}(q):P_m]=\prod_{j=1}^m(q^j+1).}
$$

The last identity follows by canceling $q$-powers and $(q^j-1)$ factors in the two order formulas; it counts maximal [totally isotropic subspaces](../../../../../totally-isotropic-subspace.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
