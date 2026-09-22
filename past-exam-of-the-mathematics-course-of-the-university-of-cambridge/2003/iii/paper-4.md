# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper4.pdf)

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

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Here is [Witt's lemma](../../../linear-algebra.md#witt-s-theorem) with the hypotheses appropriate to the [classical groups](../../../group-theory.md#classical-group). Let $V$ be finite-dimensional with a nonsingular [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form), a nonsingular [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) in [characteristic](../../../algebra.md#characteristic-of-a-field) different from two, or a nonsingular [Hermitian form](../../../linear-algebra.md#hermitian-form) with nontrivial involution. Every [isometry of a space with a form](../../../linear-algebra.md#isometry-of-a-space-with-a-form) $\phi:U\to U'$ between [vector subspaces](../../../vector-space.md#vector-subspace) extends to a form-preserving [automorphism](../../../algebra.md#automorphism) of $V$. For [quadratic forms](../../../linear-algebra.md#quadratic-form), the same statement holds in every [characteristic](../../../algebra.md#characteristic-of-a-field) when the [polar bilinear form of a quadratic form](../../../linear-algebra.md#polar-bilinear-form-of-a-quadratic-form) is nonsingular and the [isometry of a space with a form](../../../linear-algebra.md#isometry-of-a-space-with-a-form) preserves the [quadratic form](../../../linear-algebra.md#quadratic-form) itself. **The restricted forms on $U,U'$ may be degenerate.** We prove these versions, including the characteristic-two quadratic case needed later.

For an [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) $B$, split the restricted space as $U=H\oplus R$, where $R=U\cap U^\perp$ and $B|_H$ is nonsingular. Choose a [symplectic basis](../../../linear-algebra.md#symplectic-basis) for $H$ and a [basis](../../../vector-space.md#basis) $r_1,\ldots,r_t$ of $R$. The [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) form on $V$ supplies vectors $s_j$ in $H^\perp$ with $B(r_i,s_j)=\delta_{ij}$. Adding linear combinations of the $r_i$ to the $s_j$ makes $B(s_i,s_j)=0$: for each pair $i<j$ one may cancel its pairing by adding an appropriate multiple of $r_i$ to $s_j$, without disturbing the dual pairings or previously treated pairs. This uses no division by two. Thus $H$ together with the pairs $(r_i,s_i)$ is nonsingular and its [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form) has a [symplectic basis](../../../linear-algebra.md#symplectic-basis).

Apply the same construction to $\phi(H),\phi(r_i)$, choosing partners $s_i'$ there. The two completed [bases](../../../vector-space.md#basis) have identical alternating [Gram matrices](../../../linear-algebra.md#gram-matrix) and equal remaining [dimensions](../../../vector-space.md#dimension-vector-space). The [linear map](../../../vector-space.md#linear-map) matching these [bases](../../../vector-space.md#basis) preserves $B$ and agrees with $\phi$ on $H\oplus R=U$. This proves the alternating version over an arbitrary [field](../../../algebra.md#field), including [characteristic](../../../algebra.md#characteristic-of-a-field) two.

For a [quadratic form](../../../linear-algebra.md#quadratic-form) $Q$, define its [polar bilinear form of a quadratic form](../../../linear-algebra.md#polar-bilinear-form-of-a-quadratic-form) by $B(x,y)=Q(x+y)-Q(x)-Q(y)$. Its symmetry

$$
s_a(x)=x-\frac{B(x,a)}{Q(a)}a\qquad(Q(a)\ne0)
$$

preserves $Q$. The zero-dimensional case is immediate. Induct on $\dim U$: choose $Q(t)\ne0$ and a [hyperplane](../../../vector-space.md#hyperplane) $K\subseteq U\cap t^\perp$. Extending $\phi|_K$ first reduces to $\phi|_K=I$. Put $U=K\oplus Fu$, $v=\phi(u)$, $d=u-v\in S=K^\perp$. If $Q(d)\ne0$, $s_d$ completes the extension. Otherwise $B(u,d)=B(v,d)=0$. The [hyperplanes](../../../vector-space.md#hyperplane) $H=S\cap u^\perp$, $H'=S\cap v^\perp$ are proper because $S^\perp=K$.

For $a\in S\setminus(H\cup H')$ with $Q(a)\ne0$, set $c=u-s_a(v)$. Then

$$
Q(c)=\frac{B(u,a)B(v,a)}{Q(a)}\ne0,
$$

and $s_as_c$ fixes $K$ and sends $u$ to $v$. If no such $a$ exists and $|F|>2$, the identity

$$
0=Q(a+\lambda z)=\lambda^2Q(z)+\lambda B(a,z),\qquad z\in H\cap H',\quad\lambda\in F
$$

forces $Q(z)=B(a,z)=0$. The complement of two [hyperplanes](../../../vector-space.md#hyperplane) spans $S$: adding a multiple of any outside vector avoids at most two forbidden scalars. Hence $d\perp S$, so $H=H'$, forcing $Q|_S=0$, contrary to $t\in S$.

Over $\mathbb F_2$, choose $a$ outside both [hyperplanes](../../../vector-space.md#hyperplane). In the remaining case $Q(a)=Q(d)=B(a,d)=0$, and $B(a,u)=B(a,v)=1$. The explicit map

$$
g(x)=x+B(d,x)a+B(a,x)d
$$

has $g^2=I$, preserves $Q$ by cancellation of its two cross terms, fixes $K$ and sends $u$ to $v$. This closes the induction. The characteristic-independent symmetry argument and its binary exceptional step are also treated in [Casselman's quadratic-form notes](https://www.math.ubc.ca/~cass/research/pdf/QForms.pdf) and [Elman, Karpenko and Merkurjev, section 8](https://www.math.ucla.edu/~rse/book/Kniga.pdf).

In odd [characteristic](../../../algebra.md#characteristic-of-a-field) a [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) is recovered by the [polarization identity](../../../linear-algebra.md#polarization-identity) for $Q(x)=B(x,x)/2$, so the quadratic proof also proves its extension theorem. For completeness, the [Hermitian form](../../../linear-algebra.md#hermitian-form) case has a similarly explicit induction. Take $h$ linear in the first variable, with conjugation $a\mapsto\bar a$. For [anisotropic vectors for a form](../../../linear-algebra.md#anisotropic-vector-for-a-form) $u,v$ with equal value $A=h(u,u)=h(v,v)\ne0$, let $d=u-v$ and $c=h(u,d)$. When $c\ne0$, the rank-one map

$$
g(x)=x-\frac{h(x,d)}c\,d
$$

sends $u$ to $v$ and preserves $h$, since $h(d,d)=c+\bar c$ and the extra coefficient in $h(gx,gy)$ is

$$
-\frac1c-\frac1{\bar c}+\frac{c+\bar c}{c\bar c}=0.
$$

When $c=0$, insert $\lambda u$ with $\lambda\bar\lambda=1$, $\lambda\ne1$, and use two such maps. Such a scalar exists for a nontrivial involution: $\lambda=a/\bar a$ with $a\ne\bar a$ works. If the source [vector subspace](../../../vector-space.md#vector-subspace) contains an [anisotropic vector for a form](../../../linear-algebra.md#anisotropic-vector-for-a-form), align it this way and induct in its nonsingular [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form).

If instead every source vector is isotropic, the Hermitian [polarization identity](../../../linear-algebra.md#polarization-identity) makes its whole restricted form zero. Choose $e$ in its [basis](../../../vector-space.md#basis) and a partner $f$ pairing to one with $e$ and to zero with the remaining source [basis](../../../vector-space.md#basis). Make $h(f,f)=0$ by replacing $f$ by $f-te$, where $t+\bar t=h(f,f)$. The trace map is onto the fixed [field](../../../algebra.md#field): in odd [characteristic](../../../algebra.md#characteristic-of-a-field) divide by two; in [characteristic](../../../algebra.md#characteristic-of-a-field) two scale a nonzero trace. Choose $a+\bar a\ne0$. The orthogonal vectors $e+af$ and $e-\bar af$ have nonzero values $a+\bar a$ and its negative, so the preceding rank-one construction aligns this entire [hyperbolic pair](../../../linear-algebra.md#hyperbolic-pair) with its target pair. The remaining source [basis](../../../vector-space.md#basis) lies in the pair's [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form); induction finishes the Hermitian proof.

The hypotheses matter. For example, the identity-matrix [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) on $\mathbb F_2^3$ has canonical vector $c=(1,1,1)$ characterized by $B(x,c)=B(x,x)$, so every [isometry of a space with a form](../../../linear-algebra.md#isometry-of-a-space-with-a-form) fixes $c$. The one-dimensional map $e_1\mapsto c$ preserves the restricted [bilinear form](../../../linear-algebra.md#bilinear-form) but cannot extend. Thus “all symmetric forms in [characteristic](../../../algebra.md#characteristic-of-a-field) two” is not a correct replacement for the quadratic or alternating versions proved above.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**The isomorphic pair is $A_8\cong PSL_4(2)$; $PSL_3(4)$ is different.** All three have order $20160$, so order alone does not settle the question; explicitly $|PSL_3(4)|=(64-1)(64-4)(64-16)/(3\cdot3)=20160$. We give a concrete realization and an element-order distinction.

On $W=\bigwedge^2\mathbb F_2^4$, the [Pfaffian](../../../linear-algebra.md#pfaffian) is

$$
Q(x)=x_{12}x_{34}+x_{13}x_{24}+x_{14}x_{23}.
$$

It is a nonsingular plus-type [quadratic form](../../../linear-algebra.md#quadratic-form): the three displayed pairs give a hyperbolic decomposition. Change of [basis](../../../vector-space.md#basis) multiplies the [Pfaffian](../../../linear-algebra.md#pfaffian) by the [determinant](../../../linear-algebra.md#determinant), which is always one in $GL_4(2)$. Hence the [exterior-square realization of PSL4 over F2](../../../finite-group-theory.md#exterior-square-realization-of-psl4-over-f2) embeds $GL_4(2)$ into $O_6^+(2)$. The [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is trivial: an element acting trivially on the [exterior square](../../../linear-algebra.md#exterior-square) fixes every decomposable two-space, then every one-space as an intersection of two-spaces, and hence is a scalar; over $\mathbb F_2$ this scalar is one.

For a second model let $E$ be the even-weight [vector subspace](../../../vector-space.md#vector-subspace) of $\mathbb F_2^8$ and quotient by the all-one vector. The dot product descends to a [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) on the six-dimensional quotient, and

$$
q(\bar x)=\operatorname{wt}(x)/2\pmod2
$$

is well defined, since complementing an even subset changes half its weight from $w/2$ to $4-w/2$. It has $(1+70+1)/2=36$ zero vectors, so is plus type. Coordinate [permutations](../../../combinatorics.md#permutation) give a [faithful](../../../group-theory.md#faithful-group-action) $S_8$ action: fixing the quotient fixes each weight-two subset, because its complement has weight six, and fixing all two-subsets forces the identity [permutation](../../../combinatorics.md#permutation).

From the independently derived symplectic order and quadratic orbit count below,

$$
|O_6^+(2)|=\frac{|Sp_6(2)|}{36}=40320,
\qquad |GL_4(2)|=(16-1)(16-2)(16-4)(16-8)=20160.
$$

Thus $O_6^+(2)\cong S_8$ and the image of $GL_4(2)=SL_4(2)=PSL_4(2)$ is its index-two [subgroup](../../../group.md#subgroup) $A_8$. The index-two [subgroup](../../../group.md#subgroup) is unique: a nontrivial [group homomorphism](../../../group-theory.md#group-homomorphism) $S_8\to C_2$ sends every [transposition](../../../combinatorics.md#transposition-permutation) to the same nonidentity element and is the sign map.

To separate $PSL_3(4)$, observe that $A_8$ contains $(12345)(678)$ of order 15. An odd-order projective element of $PSL_3(4)$ lifts to a [semisimple linear operator](../../../vector-space.md#semisimple-linear-operator), since its order upstairs divides three times an odd order in [characteristic](../../../algebra.md#characteristic-of-a-field) two. The possible [eigenspace](../../../linear-operator-theory.md#eigenspace) degree patterns are $1+1+1$, $2+1$ and $3$. In the split case all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have order dividing three, so the projective element has no order 15. In the $2+1$ case the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\lambda,\lambda^4,\lambda^{-5}$ with $\lambda\in\mathbb F_{16}^\times$; its fifth power is scalar because $\lambda^{15}=1$, so its projective order divides five. In the irreducible case the determinant-one torus has order $4^2+4+1=21$ and quotienting its scalar [subgroup](../../../group.md#subgroup) of order three gives projective order dividing seven. **There is therefore no element of order 15 in $PSL_3(4)$.**

Several small-parameter coincidences connect the finite [classical groups](../../../group-theory.md#classical-group) to [permutation groups](../../../finite-group-theory.md#permutation-group). The projective-line action immediately gives $PSL_2(2)\cong S_3$, $PSL_2(3)\cong A_4$, $PGL_2(3)\cong S_4$ and $PSL_2(4)\cong A_5$ by [faithful](../../../group-theory.md#faithful-group-action) actions of degrees three, four and five and their orders. Also $PSL_2(5)\cong A_5$: its involutions have Klein-four [centralizers](../../../group-theory.md#centralizer), giving five [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup); their [conjugation action](../../../group-theory.md#conjugation-action) is [faithful](../../../group-theory.md#faithful-group-action) and embeds its order-60 [simple group](../../../finite-group-theory.md#simple-group) into $S_5$. Simplicity here can be checked from class sizes $1,15,20,12,12$: no proper nontrivial normal class union has order dividing 60. The same five-subgroup action extends to $PGL_2(5)$, with trivial [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) and order 120, giving $S_5$. Indeed its kernel intersects $PSL_2(5)$ trivially, so centralizes that normal [subgroup](../../../group.md#subgroup). Commuting projectively with both upper and lower elementary unipotents forces a representing matrix to be scalar, so this kernel is trivial.

The less immediate coincidence $PSL_2(9)\cong A_6$ can be exhibited on the ten unordered triple partitions used in Question 4. Let $a=(123)$, $b=(456)$, $w=(12)(36)$, assign $\infty$ to $123\mid456$ and $0$ to $126\mid345$, and label the other partitions by applying $a^xb^y$ to the zero partition, with $t=x+iy\in\mathbb F_9$ and $i^2=-1$. Inspection of these nine partitions gives

$$
a:t\mapsto t+1,\qquad b:t\mapsto t+i,\qquad w:t\mapsto-1/t.
$$

Translations and inversion generate $PSL_2(9)$: conjugating the upper unitriangular matrices by inversion gives the lower ones, and elementary elimination generates $SL_2(9)$. Their projective action has order $9(9^2-1)/2=360$. These partition [permutations](../../../combinatorics.md#permutation) come from even [permutations](../../../combinatorics.md#permutation) of six letters, whose partition action is [faithful](../../../group-theory.md#faithful-group-action) as proved below; hence they fill $A_6$.

Finally, on the even-weight module of $\mathbb F_2^6$ modulo its all-one vector, coordinate [permutations](../../../combinatorics.md#permutation) preserve a [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) in [dimension](../../../vector-space.md#dimension-vector-space) four and act faithfully, again by the weight-two-subset argument. Both $S_6$ and $Sp_4(2)$ have order 720, proving $Sp_4(2)\cong S_6$, with [commutator subgroup](../../../group-theory.md#commutator-subgroup) $A_6$. These examples illustrate both the need to quotient [group centers](../../../group-theory.md#center-of-a-group) and the low-rank exceptions to general simplicity. They do not make equal orders sufficient for [group isomorphism](../../../algebra.md#group-isomorphism), as the two order-20160 examples already demonstrate.

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $B$ be a [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) on $V$ of [dimension](../../../vector-space.md#dimension-vector-space) $2m$ over $\mathbb F_q$. A [symplectic basis](../../../linear-algebra.md#symplectic-basis) has $B(e_i,f_j)=\delta_{ij}$ and all $e_i,e_j$ and $f_i,f_j$ pairings zero. Such [bases](../../../vector-space.md#basis) are built by choosing a nonzero $e_1$, finding $f_1$ with $B(e_1,f_1)=1$, and continuing in their nonsingular [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form). In these coordinates the group preserving $B$ is

$$
Sp_{2m}(q)=\{g:g^{\mathsf T}Jg=J\},\qquad
J=\begin{pmatrix}0&I\\-I&0\end{pmatrix}.
$$

Its action on [symplectic bases](../../../linear-algebra.md#symplectic-basis) is regular. There are $q^{2m}-1$ choices for $e_1$ and $q^{2m-1}$ for $f_1$, so induction gives the [finite symplectic group order](../../../symplectic-geometry.md#finite-symplectic-group-order)

$$
|Sp_{2m}(q)|=(q^{2m}-1)q^{2m-1}|Sp_{2m-2}(q)|,
\qquad\boxed{|Sp_{2m}(q)|=q^{m^2}\prod_{j=1}^m(q^{2j}-1).}
$$

The [center of a group](../../../group-theory.md#center-of-a-group) consists of $aI$ with $a^2=1$, and has order $\gcd(2,q-1)$. To see there are no other central elements, a central element commutes with every [symplectic transvection](../../../finite-group-theory.md#symplectic-transvection) and hence fixes every [symplectic transvection](../../../finite-group-theory.md#symplectic-transvection) center line; a [linear map](../../../vector-space.md#linear-map) fixing every line is scalar. Consequently the [projective symplectic group over a finite field](../../../finite-group-theory.md#projective-symplectic-group-over-a-finite-field) has this order divided by $\gcd(2,q-1)$.

Here is a proof of the main ingredients in simplicity. The [symplectic transvection](../../../finite-group-theory.md#symplectic-transvection)

$$
T_{v,c}(x)=x+cB(x,v)v
$$

preserves $B$, has inverse $T_{v,-c}$, and fixes $v^\perp$ pointwise. These transformations generate $Sp_{2m}(q)$. Indeed if $B(u,w)\ne0$, then $T_{w-u,\,1/B(u,w)}$ sends $u$ to $w$. If the pairing is zero, choose an intermediate vector having nonzero pairing with both, so two [symplectic transvections](../../../finite-group-theory.md#symplectic-transvection) suffice. This aligns the first vector of any [symplectic basis](../../../linear-algebra.md#symplectic-basis). For partners $f,f'$ of the same $e$, their difference lies in $e^\perp$. If $B(f,f')\ne0$ a [symplectic transvection](../../../finite-group-theory.md#symplectic-transvection) centered at $f'-f$ aligns them and fixes $e$. If it is zero and the partners differ, $h=f+e$ pairs nontrivially with both and still pairs to one with $e$; two such [symplectic transvections](../../../finite-group-theory.md#symplectic-transvection) work. After fixing the pair, induction in its [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form) aligns the rest of the [basis](../../../vector-space.md#basis).

The projective action on one-spaces is [faithful](../../../group-theory.md#faithful-group-action). For $m\ge2$, a line [stabilizer](../../../group-theory.md#stabilizer-subgroup) has three orbits: the line itself, the other lines perpendicular to it, and the lines not perpendicular to it. [Witt's lemma](../../../linear-algebra.md#witt-s-theorem) proves transitivity within the latter two orbits by matching the two-dimensional restricted form. This action is [primitive](../../../group-theory.md#primitive-group-action). A block containing distinct perpendicular lines $L,M$ is invariant under both [stabilizers](../../../group-theory.md#stabilizer-subgroup) and therefore contains a line perpendicular to $M$ but not to $L$. A block containing distinct nonperpendicular lines likewise contains a line perpendicular to $L$ but not to $M$, by using the $M$ [stabilizer](../../../group-theory.md#stabilizer-subgroup). Such lines exist by nonsingularity in [dimension](../../../vector-space.md#dimension-vector-space) at least four. Either possibility makes the block contain both nontrivial [stabilizer](../../../group-theory.md#stabilizer-subgroup) orbits, hence every line. For $m=1$ the action on the [projective line](../../../finite-group-theory.md#projective-line) is [two-transitive](../../../group-theory.md#two-transitive-group-action) and thus [primitive](../../../group-theory.md#primitive-group-action).

[Symplectic transvections](../../../finite-group-theory.md#symplectic-transvection) with one fixed center line form an [Abelian](../../../group.md#abelian-group) [normal subgroup](../../../group-theory.md#normal-subgroup) of its [stabilizer](../../../group-theory.md#stabilizer-subgroup), and their conjugates generate the whole group. The [Iwasawa simplicity lemma](../../../finite-group-theory.md#iwasawa-simplicity-lemma) now reduces simplicity to being [perfect](../../../group-theory.md#perfect-group). Its short proof is useful: any nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of a [faithful](../../../group-theory.md#faithful-group-action) [primitive](../../../group-theory.md#primitive-group-action) group is transitive, since its orbits are blocks. Writing $G=NH$, where $H$ is a point [stabilizer](../../../group-theory.md#stabilizer-subgroup), shows that all conjugates of the specified [Abelian](../../../group.md#abelian-group) [subgroup](../../../group.md#subgroup) have the same image modulo $N$. Thus $G/N$ is [Abelian](../../../group.md#abelian-group). If $G$ is [perfect](../../../group-theory.md#perfect-group), $N=G$.

The groups can also be shown to be [perfect](../../../group-theory.md#perfect-group) concretely. For $q>3$ choose $a$ with $a^2\ne1$ and let $D$ scale $e$ by $a$ and $f$ by $a^{-1}$. Then

$$
DT_{e,c}D^{-1}T_{e,c}^{-1}=T_{e,(a^2-1)c},
$$

so every [symplectic transvection](../../../finite-group-theory.md#symplectic-transvection) is a [group commutator](../../../group.md#group-commutator). For $q=3,m\ge2$, [symplectic transvections](../../../finite-group-theory.md#symplectic-transvection) of coefficient one are conjugate, have order three, and the four with centers $e_1,e_2,e_1+e_2,e_1-e_2$ in a two-dimensional [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace) multiply to the identity. They commute, and the sum of their rank-one terms is zero modulo three. Their common class in the [abelianization](../../../group-theory.md#abelianization) is therefore annihilated by both three and four, hence is zero. For $q=2,m\ge3$, use the seven nonzero vectors of a three-dimensional [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace). The [symplectic transvections](../../../finite-group-theory.md#symplectic-transvection) commute and their product is the identity, because each diagonal coefficient occurs four times and each cross coefficient twice. Their common abelianized class is annihilated by two and seven, hence is zero. Generation now proves these groups are [perfect](../../../group-theory.md#perfect-group).

It follows that

$$
\boxed{PSp_{2m}(q)\text{ is simple except for }(m,q)=(1,2),(1,3),(2,2).}
$$

The exceptions are $S_3$, $A_4$ and $S_6$ respectively. For odd $q$ the full [symplectic group over a finite field](../../../finite-group-theory.md#symplectic-group-over-a-finite-field) has nontrivial [center of a group](../../../group-theory.md#center-of-a-group), so simplicity refers to its [quotient group](../../../group-theory.md#quotient-group); for even $q$ the [center of a group](../../../group-theory.md#center-of-a-group) is trivial.

A [symplectic parabolic subgroup](../../../symplectic-geometry.md#symplectic-parabolic-subgroup) stabilizes a flag of [totally isotropic subspaces](../../../linear-algebra.md#totally-isotropic-subspace). The maximal such [parabolic subgroups](../../../lie-theory.md#parabolic-subgroup) $P_r$ stabilize a single $r$-space, $1\le r\le m$. In an adapted [basis](../../../vector-space.md#basis) their [Levi subgroup](../../../lie-theory.md#levi-subgroup) is $GL_r(q)\times Sp_{2m-2r}(q)$, with an arbitrary block of $r(2m-2r)$ parameters and a remaining symmetric block of $r(r+1)/2$ parameters. Thus

$$
P_r=U_r\rtimes\bigl(GL_r(q)\times Sp_{2m-2r}(q)\bigr),\qquad
|U_r|=q^{2r(m-r)+r(r+1)/2}.
$$

These are the single-member flag [stabilizers](../../../group-theory.md#stabilizer-subgroup), equivalently the standard maximal [parabolic subgroups](../../../lie-theory.md#parabolic-subgroup) obtained by omitting one node of the symplectic [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram). Two particular cases have transparent descriptions.

For the [symplectic point stabilizer](../../../symplectic-geometry.md#symplectic-point-stabilizer), write $V=\langle e,f\rangle\perp W$. Its [unipotent radical](../../../lie-theory.md#unipotent-radical) consists of

$$
u(b,t):\quad e\mapsto e,\quad w\mapsto w-B(w,b)e,\quad f\mapsto f+b+te,
\qquad b\in W,\ t\in\mathbb F_q.
$$

All pairings are preserved by direct substitution. The product law is $(b,t)(b',t')=(b+b',t+t'+B(b,b'))$, so this radical has order $q^{2m-1}$. With [group commutator](../../../group.md#group-commutator) convention $uvu^{-1}v^{-1}$, its commutator has central parameter $2B(b,b')$: it is Heisenberg-type in odd [characteristic](../../../algebra.md#characteristic-of-a-field), but [Abelian](../../../group.md#abelian-group) in [characteristic](../../../algebra.md#characteristic-of-a-field) two. A [Levi subgroup](../../../lie-theory.md#levi-subgroup) scales $e,f$ inversely and acts as $Sp(W)$, giving

$$
\boxed{P_1=U_1\rtimes\bigl(\mathbb F_q^\times\times Sp_{2m-2}(q)\bigr),\qquad
[Sp_{2m}(q):P_1]=\frac{q^{2m}-1}{q-1}.}
$$

This index counts the one-spaces, all of which are isotropic for an [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form).

For a [Lagrangian subspace](../../../symplectic-geometry.md#lagrangian-subspace) $E=\langle e_1,\ldots,e_m\rangle$, the [symplectic Lagrangian stabilizer](../../../symplectic-geometry.md#symplectic-lagrangian-stabilizer) has block form

$$
\begin{pmatrix}A&AS\\0&A^{-\mathsf T}\end{pmatrix},\qquad
A\in GL_m(q),\quad S=S^{\mathsf T}.
$$

Substituting into $g^{\mathsf T}Jg=J$ proves both the inverse-transpose lower block and symmetry of $S$. The [unipotent radical](../../../lie-theory.md#unipotent-radical) is the additive group of [symmetric matrices](../../../linear-algebra.md#symmetric-matrix), and $A$ acts by $S\mapsto ASA^{\mathsf T}$. Therefore

$$
\boxed{|P_m|=q^{m(m+1)/2}|GL_m(q)|,\qquad
[Sp_{2m}(q):P_m]=\prod_{j=1}^m(q^j+1).}
$$

The last identity follows by canceling $q$-powers and $(q^j-1)$ factors in the two order formulas; it counts maximal [totally isotropic subspaces](../../../linear-algebra.md#totally-isotropic-subspace).

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the [degree-ten partition action of S6](../../../group-theory.md#degree-ten-partition-action-of-s6), take unordered partitions of six letters into two triples. There are $\binom63/2=10$. Fix $A\mid A^c$. Its [stabilizer](../../../group-theory.md#stabilizer-subgroup) is $(S_3\times S_3)\rtimes S_2=S_3\wr S_2$, permuting each triple and interchanging them. The [subgroup](../../../group.md#subgroup) generated by a 3-cycle in each triple has order nine, so is a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $S_6$. Any [normalizer](../../../group-theory.md#normalizer) preserves its two three-point orbits; conversely all the indicated within-triple [permutations](../../../combinatorics.md#permutation) and the swap normalize it. This proves the asserted [normalizer](../../../group-theory.md#normalizer) exactly.

For any different partition $C\mid C^c$, $|A\cap C|$ is one or two after excluding the identical partition. Interchanging $C$ and $C^c$ identifies these two possibilities. The [stabilizer](../../../group-theory.md#stabilizer-subgroup) of $A\mid A^c$ is transitive on each fixed intersection pattern, hence on all other nine partitions. **The degree-ten action is [two-transitive](../../../group-theory.md#two-transitive-group-action).** It is also [faithful](../../../group-theory.md#faithful-group-action): two distinct partitions have a common refinement with two singleton cells and two cells of size two. Every unordered pair of letters occurs as those singleton cells. A [permutation](../../../combinatorics.md#permutation) fixing every partition therefore fixes every pair and consequently every letter.

For the [subgroup factorization from coset transitivity](../../../group-theory.md#subgroup-factorization-from-coset-transitivity), use [cosets](../../../group-theory.md#coset) $Hg$ (right cosets) and right multiplication by $K$. The orbit of $H$ is precisely $\{Hk:k\in K\}$. This is every [coset](../../../group-theory.md#coset) if and only if every $g$ can be written $hk$, proving

$$
\boxed{G=HK\quad\Longleftrightarrow\quad K\text{ is transitive on }H\backslash G.}
$$

A natural $S_5$ fixing one letter is transitive on the ten partitions: the triple containing the fixed letter is determined by any two of the other five. Taking $H=S_3\wr S_2$, $K=S_5$ gives $S_6=HK$; inversion gives the requested order as well,

$$
\boxed{S_6=S_5(S_3\wr S_2).}
$$

Now let $B$ be the binary [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form). Its [binary quadratic refinements](../../../linear-algebra.md#binary-quadratic-refinement) form an [affine space](../../../geometry-and-topology.md#affine-space): the difference of two such forms is linear, so for a fixed $Q_0$ every one is uniquely

$$
Q_v(x)=Q_0(x)+B(v,x),\qquad v\in V.
$$

In a [symplectic basis](../../../linear-algebra.md#symplectic-basis) each refinement is

$$
Q(x,y)=\sum_{i=1}^m\bigl(x_iy_i+a_ix_i+b_iy_i\bigr),\qquad
\operatorname{Arf}(Q)=\sum_{i=1}^ma_ib_i\in\mathbb F_2.
$$

A two-dimensional summand with $(a_i,b_i)\ne(1,1)$ admits a [basis](../../../vector-space.md#basis) of singular vectors paired to one and is hyperbolic; the $(1,1)$ summand is anisotropic. Two planes spanned by [anisotropic vectors for a form](../../../linear-algebra.md#anisotropic-vector-for-a-form) together become two [hyperbolic planes of a quadratic form](../../../linear-algebra.md#hyperbolic-plane-quadratic-form): with anisotropic [basis](../../../vector-space.md#basis) pairs $(e_1,f_1),(e_2,f_2)$, the singular vectors $e_1+e_2,f_1+e_2$ pair to one; their [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form) has singular paired [basis](../../../vector-space.md#basis) $e_1+f_1+f_2,e_1+f_1+e_2+f_2$. Consequently every refinement is equivalent to either $m$ [hyperbolic planes of a quadratic form](../../../linear-algebra.md#hyperbolic-plane-quadratic-form) or $(m-1)$ [hyperbolic planes of a quadratic form](../../../linear-algebra.md#hyperbolic-plane-quadratic-form) and one anisotropic plane (all three nonzero vectors are [anisotropic vectors for a form](../../../linear-algebra.md#anisotropic-vector-for-a-form)).

These two types are different. Indeed the character sum of each plane is $+2$ or $-2$, so

$$
\sum_{x\in V}(-1)^{Q(x)}=(-1)^{\operatorname{Arf}(Q)}2^m.
$$

Thus there are exactly two symplectic orbits $Q^+(B),Q^-(B)$, the signs denoting $\operatorname{Arf}=0,1$. Counting the three coefficient pairs with product zero and the one with product one gives

$$
\boxed{|Q^\pm(B)|=\frac{4^m\pm2^m}{2}=2^{m-1}(2^m\pm1).}
$$

The same character sum gives the corresponding numbers of singular vectors, including zero, in a fixed form of either type.

Fix a form $Q$ of type $\epsilon$. Completing the square by $x\mapsto x+v$ shows

$$
\sum_x(-1)^{Q_v(x)}=(-1)^{Q(v)}\sum_x(-1)^{Q(x)},\qquad
\epsilon(Q_v)=\epsilon(Q)(-1)^{Q(v)}.
$$

The [stabilizer](../../../group-theory.md#stabilizer-subgroup) of $Q$ is exactly $O(V,Q)$. It sends the parameter $v$ by its natural linear action or inverse action according to the chosen left/right convention. Other forms of the same type correspond to nonzero singular vectors $v$, and all forms of opposite type correspond to nonsingular vectors $v$. For two nonzero vectors of the same $Q$ value, the map between their spans is an [isometry of a space with a form](../../../linear-algebra.md#isometry-of-a-space-with-a-form). [Witt's lemma](../../../linear-algebra.md#witt-s-theorem) extends it, so the orthogonal [stabilizer](../../../group-theory.md#stabilizer-subgroup) is transitive on each of these two vector sets. This proves the [two-transitive binary quadratic-form actions](../../../linear-algebra.md#two-transitive-binary-quadratic-form-actions): the [symplectic group over a finite field](../../../finite-group-theory.md#symplectic-group-over-a-finite-field) is transitive on each type and its point [stabilizer](../../../group-theory.md#stabilizer-subgroup) is transitive on all other members of that type.

In particular $O^-_{2m}(2)$ is transitive on the plus orbit. Identify that orbit with the [cosets](../../../group-theory.md#coset) (right cosets) of a plus [stabilizer](../../../group-theory.md#stabilizer-subgroup), using $Q^g(x)=Q(gx)$ as a right action. The [coset](../../../group-theory.md#coset) criterion then proves

$$
\boxed{Sp_{2m}(2)=O^+_{2m}(2)O^-_{2m}(2).}
$$

Both genuine [two-transitive](../../../group-theory.md#two-transitive-group-action) actions require $m\ge2$. At $m=1$ the plus orbit has three forms and the minus orbit is a singleton; transitivity and the factorization remain true, while [two-transitive](../../../group-theory.md#two-transitive-group-action) action on the singleton is only vacuous if one's convention permits degree one. No special simplicity assertion is needed for this argument. At $m=2$ the orbit sizes are ten and six, linking these actions with $Sp_4(2)\cong S_6$ and the partition action above.

## 5

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For the [Johnson graph](../../../graph-theory.md#johnson-graph), an [edge](../../../graph-theory.md#edge-of-a-graph) exchanges one member of a $k$-set. Along one [edge](../../../graph-theory.md#edge-of-a-graph), intersection size with a fixed target can increase by at most one, so any [path in a graph](../../../graph-theory.md#path-in-a-graph) from $A$ to $B$ has length at least $k-|A\cap B|$. Replacing the elements of $A\setminus B$ successively by elements of $B\setminus A$ gives a [path in a graph](../../../graph-theory.md#path-in-a-graph) attaining that bound. Hence the [distance in a Johnson graph](../../../graph-theory.md#distance-in-a-johnson-graph) is

$$
\boxed{d(A,B)=k-|A\cap B|.}
$$

If two ordered pairs have the same distance $r$, their four regions (intersection, first-only, second-only and outside the union) have sizes $k-r,r,r,n-k-r$. Choose bijections between corresponding regions. Their union is a ground-set [permutation](../../../combinatorics.md#permutation) sending the ordered pair to the other pair and preserving [graph adjacency](../../../graph.md#graph-adjacency). **The [symmetric group](../../../finite-group-theory.md#symmetric-group) is [distance-transitive](../../../graph.md#distance-transitive-graph).** For $n\ge2k$ the [graph diameter](../../../graph-theory.md#graph-diameter) is $k$.

For the [Grassmann graph](../../../differential-geometry.md#grassmann-graph), a codimension-one exchange changes intersection [dimension](../../../vector-space.md#dimension-vector-space) with a fixed target by at most one. More explicitly, if $A,A'$ are adjacent, their common $(k-1)$-space shows $\dim(A'\cap B)\ge\dim(A\cap B)-1$, and exchanging the two gives the reverse bound. Thus distance is at least $r=k-\dim(A\cap B)$.

Choose a [basis](../../../vector-space.md#basis) $c_1,\ldots,c_{k-r}$ of $I=A\cap B$, complement it in $A$ by $a_1,\ldots,a_r$, and in $B$ by $b_1,\ldots,b_r$. These combined vectors are independent because $A\cap B=I$. The spaces

$$
A_j=I+\langle b_1,\ldots,b_j,a_{j+1},\ldots,a_r\rangle,\qquad 0\le j\le r,
$$

form a [path in a graph](../../../graph-theory.md#path-in-a-graph) of length $r$. Consequently

$$
\boxed{d(A,B)=k-\dim(A\cap B).}
$$

Equal-distance ordered pairs have the same [dimensions](../../../vector-space.md#dimension-vector-space) in this adapted [basis](../../../vector-space.md#basis) construction. Extend both combined [bases](../../../vector-space.md#basis) to [bases](../../../vector-space.md#basis) of $V$, and match them by a [invertible linear map](../../../calculus.md#invertible-linear-map). It maps the first ordered pair to the second and preserves [dimensions](../../../vector-space.md#dimension-vector-space) of intersections, hence [graph adjacency](../../../graph.md#graph-adjacency). **$GL_n(F)$ is [distance-transitive](../../../graph.md#distance-transitive-graph)**, over an arbitrary [field](../../../algebra.md#field), with [graph diameter](../../../graph-theory.md#graph-diameter) $k$ under $n\ge2k$.

For the [symplectic dual polar graph](../../../graph.md#symplectic-dual-polar-graph), [vertices](../../../graph.md#vertex-graph-theory) are Lagrangian $m$-spaces. Let $I=A\cap B$ have [dimension](../../../vector-space.md#dimension-vector-space) $m-r$. The quotient $I^\perp/I$ is a nonsingular [symplectic vector space](../../../linear-algebra.md#symplectic-vector-space) of [dimension](../../../vector-space.md#dimension-vector-space) $2r$, and $A/I,B/I$ are complementary [Lagrangian subspaces](../../../symplectic-geometry.md#lagrangian-subspace). Their mutual pairing is nonsingular: a vector orthogonal to both lies in $(A+B)^\perp=I$, so vanishes in the quotient. Choose dual [bases](../../../vector-space.md#basis) $e_1,\ldots,e_r$ in $A/I$ and $f_1,\ldots,f_r$ in $B/I$, and lift them into $A,B$. Their span is a nonsingular symplectic $2r$-space. Complete it by a [basis](../../../vector-space.md#basis) $e_{r+1},\ldots,e_m$ of $I$ and suitable dual partners. This gives the pair normal form

$$
A=\langle e_1,\ldots,e_m\rangle,\qquad
B=\langle f_1,\ldots,f_r,e_{r+1},\ldots,e_m\rangle.
$$

The spaces $A_j=\langle f_1,\ldots,f_j,e_{j+1},\ldots,e_m\rangle$ remain [totally isotropic subspace](../../../linear-algebra.md#totally-isotropic-subspace): a present $f_i$ pairs only with the absent $e_i$. They give an adjacent-step [path in a graph](../../../graph-theory.md#path-in-a-graph) of length $r$. The previous intersection-dimension lower bound still applies, proving

$$
\boxed{d(A,B)=m-\dim(A\cap B).}
$$

For two ordered pairs at the same distance, match their adapted [symplectic bases](../../../linear-algebra.md#symplectic-basis). The resulting map preserves the [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) and sends the pairs to each other, so lies in $Sp_{2m}(F)$. Equivalently, construct the [isometry of a space with a form](../../../linear-algebra.md#isometry-of-a-space-with-a-form) on $A+B$ from the displayed normal form and extend it by [Witt's lemma](../../../linear-algebra.md#witt-s-theorem). **The action of the [symplectic group over a field](../../../symplectic-geometry.md#symplectic-group-over-a-field) is [distance-transitive](../../../graph.md#distance-transitive-graph)**, over every [field](../../../algebra.md#field), and its graph has [graph diameter](../../../graph-theory.md#graph-diameter) $m$. The zero-dimensional boundary cases give a single [vertex](../../../graph.md#vertex-graph-theory) and trivial transitivity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
