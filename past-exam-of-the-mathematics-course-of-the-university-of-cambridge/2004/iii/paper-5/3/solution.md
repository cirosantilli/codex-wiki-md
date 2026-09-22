<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Nagao module theorem](../../../../../nagao-module-theorem.md) states that if $e\in Z(kG)$ is a [central idempotent](../../../../../central-idempotent.md), $eM=M$, and $C_G(Q)\leq K\leq N_G(Q)$, then $\operatorname{Br}_Q(e)$ is central in $kK$ and

$$
M\downarrow_K=\operatorname{Br}_Q(e)M\oplus(1-\operatorname{Br}_Q(e))M.
$$

Every indecomposable summand of the second term is relatively projective for some subgroup of $K$ not containing $Q$. In particular, if $Q\leq K$, the error term has no summand with [module vertex](../../../../../vertex-of-an-indecomposable-module.md) containing $Q$. This is the Nagao version of the second main theorem; it identifies the [modular block](../../../../../block-of-a-group-algebra.md) of a [module vertex](../../../../../vertex-of-an-indecomposable-module.md)-$Q$ [Green correspondent](../../../../../green-correspondent-of-a-module.md).

Let $e_B$ be the identity of $B$, $N=N_G(D)$, and $b$ its [Brauer correspondent of a block](../../../../../brauer-correspondent-of-a-block.md) in $kN$. Because $D\triangleleft N$, the ideal $J(kD)kN$ is nilpotent: normality allows moving $kN$ past $J(kD)$ and the augmentation ideal of the p-group is nilpotent. Hence $b$ has nonzero image in $k(N/D)$. Choose an indecomposable summand $U$ of $b\,k[N/D]$. It is projective over $k(N/D)$ and belongs to [modular block](../../../../../block-of-a-group-algebra.md) $b$ after inflation.

Since $k[N/D]=\operatorname{Ind}_D^Nk$ is a [permutation module](../../../../../permutation-module.md), its summand $U$ has trivial [module source](../../../../../source-of-an-indecomposable-module.md) and [module vertex](../../../../../vertex-of-an-indecomposable-module.md) contained in $D$. As $D$ acts trivially, all its proper-subgroup traces vanish and its [Brauer quotient of a module](../../../../../brauer-quotient-of-a-module.md) is $U(D)=U\ne0$. The [module vertex](../../../../../vertex-of-an-indecomposable-module.md) must also contain $D$, so it is exactly $D$. This is [inflated quotient projectives have trivial source](../../../../../inflated-quotient-projectives-have-trivial-source.md).

Let $M$ be the [Green correspondent](../../../../../green-correspondent-of-a-module.md) of $U$ in $G$, using the theorem proved in the next solution. It has [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$ and the same trivial [module source](../../../../../source-of-an-indecomposable-module.md). For a normal [p-subgroup](../../../../../p-subgroup.md), each central block idempotent of $kN$ equals its Brauer image: the two central idempotents agree modulo the nilpotent ideal $J(kD)kN$, because nonfixed conjugation-orbit sums map to zero in $k(N/D)$; central idempotents congruent modulo a nilpotent ideal coincide. The first main theorem therefore gives $\operatorname{Br}_D(e_B)=\operatorname{Br}_D(b)=b$.

Let $e_C$ be the block identity acting on $M$. Nagao's theorem forces $\operatorname{Br}_D(e_C)U=U$, since $U$ has [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$. But $bU=U$, and for $C\ne B$ orthogonality would give $\operatorname{Br}_D(e_C)b=\operatorname{Br}_D(e_Ce_B)=0$. Therefore **$M$ belongs to $B$, has [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $D$ and has trivial [module source](../../../../../source-of-an-indecomposable-module.md)**. For $D=1$, this supplies an indecomposable projective in the defect-zero [modular block](../../../../../block-of-a-group-algebra.md).

For the representation-type deduction, [modules in a block are projective relative to its defect group](../../../../../modules-in-a-block-are-projective-relative-to-its-defect-group.md): the block trace identity acts as a relative trace equal to the module identity, so [D. Higman criterion](../../../../../d-higman-criterion.md) gives split induction from $D$. If $D$ is cyclic of order $d$, then $kD\cong k[t]/(t^d)$, whose [indecomposable modules](../../../../../indecomposable-module.md) are the nilpotent Jordan chains $k[t]/(t^j)$, $1\leq j\leq d$. Each indecomposable in $B$ is a summand of the [module induction](../../../../../induced-representation.md) of its [module restriction](../../../../../restriction-of-a-representation.md) to $D$, and hence occurs among the summands of these finitely many fixed induced modules. Their finite [Krull-Schmidt decompositions](../../../../../krull-schmidt-decomposition.md) give [finite representation type](../../../../../finite-representation-type.md).

Conversely, the [regular defect-group bimodule inside a block](../../../../../regular-defect-group-bimodule-inside-a-block.md) gives

$$
kD\mid(kGe_B)\downarrow_{D\times D}.
$$

Indeed this [module restriction](../../../../../restriction-of-a-representation.md) is a permutation summand. Its Brauer quotient at $\Delta D$ is nonzero, because on the fixed group-basis elements $C_G(D)$ the block projection becomes multiplication by $\operatorname{Br}_D(e_B)\ne0$. Every transitive $D\times D$ orbit in $G$ has stabilizer of order at most $|D|$. A summand with a nonzero quotient at $\Delta D$ must therefore have stabilizer exactly $\Delta D$ up to conjugacy, and is the regular $kD$ [bimodule](../../../../../bimodule.md). Tensoring this split inclusion on the right with an arbitrary $kD$-module $V$ yields

$$
V\mid\operatorname{Res}_D^G\bigl(e_B\operatorname{Ind}_D^G V\bigr).
$$

If $B$ has only finitely many [indecomposable modules](../../../../../indecomposable-module.md), their restrictions contain only finitely many indecomposable summands. The displayed inclusion puts every indecomposable $V$ on that finite list, so $kD$ has finite representation type too.

A noncyclic [finite p-group](../../../../../finite-p-group.md) has a quotient $C_p\times C_p$, by the [Burnside basis theorem](../../../../../burnside-basis-theorem.md) for its [Frattini quotient](../../../../../frattini-quotient.md). Here is an explicit infinite family over any field, including a finite field. For $s\geq1$, take basis $v_0,\ldots,v_s,w_1,\ldots,w_s$ and operators $x=g-1$, $y=h-1$ defined by

$$
xv_0=0,\quad xv_i=w_i\ (1\leq i\leq s),\qquad
yv_i=w_{i+1}\ (0\leq i<s),\quad yv_s=0,
$$

and $xw_i=yw_i=0$. All products of $x,y$ vanish, so $1+x,1+y$ satisfy the group relations in characteristic $p$. The radical is $W=\langle w_1,\ldots,w_s\rangle$. An endomorphism preserves $W$, and commuting with the two shift maps forces its induced maps on $V/W$ and $W$ to be the same scalar. To see this, write the shift matrices as $X=(0\ I_s)$ and $Y=(I_s\ 0)$: the equations $CX=XA$, $CY=YA$ force the off-diagonal entries of $A,C$ to vanish and all diagonal entries to agree, by comparing successive rows, including the zero first column of $X$ and zero last column of $Y$. The remaining linear map sends the top into $W$ and has square zero. Thus the [endomorphism ring](../../../../../endomorphism-ring.md) is a scalar algebra with square-zero radical, hence local; the module is indecomposable. Inflation to $D$ preserves that ring. Its dimensions $2s+1$ are unbounded, contradicting finite representation type. Therefore **$B$ has finite representation type if and only if $D$ is cyclic**, including trivial defect.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
