<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Nagao version of Brauer second main theorem](../../../../../nagao-module-theorem.md) is the following module statement. Let $e$ be a central idempotent of $kG$, let $P$ be a [p-subgroup](../../../../../p-subgroup.md), and suppose $C_G(P)\le K\le N_G(P)$. If $eM=M$, put $b=\operatorname{Br}_P(e)$, which is central in $kK$. Then

$$
\operatorname{Res}_K^G M=b\operatorname{Res}_K^G M\oplus(1-b)\operatorname{Res}_K^G M,
$$

and every indecomposable summand of the second term has vertex not containing $P$. More precisely it is relatively projective for some $p$-subgroup of $K$ not containing $P$. In particular the vertex-$P$ [Green correspondent](../../../../../green-correspondent-of-a-module.md) lies in the block selected by the [Brauer morphism](../../../../../brauer-morphism.md). This is the precise restriction statement needed below.

Let $B$ have [defect group of a block](../../../../../defect-group-of-a-block.md) $D$, and let $b$ be its [Brauer correspondent](../../../../../brauer-correspondent-of-a-block.md) in $N=N_G(D)$. We first build a trivial-source module in $b$. The exact functor

$$
F(S)=e_b\operatorname{Ind}_D^N S
$$

is nonzero on the trivial $kD$-module. Otherwise it would vanish on every $kD$-module, since a [group algebra of a p-group in characteristic p is local](../../../../../group-algebra-of-a-p-group-in-characteristic-p-is-local.md) and all composition factors are trivial; but $F(kD)=b\ne0$. Choose an indecomposable summand $V$ of $F(k)$. Since $D\triangleleft N$, its restriction to $D$ is a nonzero direct sum of trivial modules. It is $D$-projective. It cannot have a proper vertex $Q<D$: restriction would make a trivial $D$-module relatively $Q$-projective, whereas on its endomorphisms the trace from $Q$ is multiplication by $[D:Q]=0$ in $k$, contrary to the [D. Higman criterion](../../../../../d-higman-criterion.md). Hence $V$ has vertex $D$ and trivial source.

Take its [Green correspondent](../../../../../green-correspondent-of-a-module.md) $M$ in $G$. To verify that $M$ is in the intended block rather than just some block with a large defect, let $e'$ be the global block idempotent acting on $M$. Nagao's theorem puts the vertex-$D$ summand $V$ of $M\downarrow_N$ in $\operatorname{Br}_D(e')$. Thus $e_b\operatorname{Br}_D(e')\ne0$. The first main theorem already gives $e_b=\operatorname{Br}_D(e_B)$; orthogonality of Brauer images of different global block idempotents forces $e'=e_B$. Green correspondence preserves sources, so **$B$ contains an indecomposable module with vertex $D$ and trivial source.** The same argument proves the same-block compatibility of Green correspondence for every vertex-$D$ module used below.

For [finite representation type](../../../../../finite-representation-type.md), first suppose $D$ is cyclic of order $q$. Write $D=\langle g\rangle$ and $t=g-1$. Then $kD\cong k[t]/(t^q)$, and the [indecomposable modules for a cyclic p-group](../../../../../indecomposable-modules-for-a-cyclic-p-group.md) are $k[t]/(t^j)$, $1\le j\le q$, by [Jordan normal form](../../../../../jordan-normal-form.md). Every indecomposable module in $B$ is $D$-projective by Question 1, so is a summand of an induction of one of these finitely many indecomposable $kD$-modules. Each induction has finitely many indecomposable summands. Therefore $B$ has finite representation type.

For the converse it is important to obtain infinitely many modules of full vertex $D$, and not silently assume that the field is infinite. If $D$ is noncyclic, its quotient by the [Frattini subgroup](../../../../../frattini-subgroup.md) is elementary abelian of rank at least two, so $D$ maps onto $C_p\times C_p$. A rank-one Frattini quotient would make any lift of its generator generate $D$, since every proper subgroup is contained in a maximal subgroup. Here is an explicit family of [full-vertex modules for a noncyclic p-group](../../../../../full-vertex-modules-for-a-noncyclic-p-group.md) valid over every field $k$. Set $x=g-1$, $y=h-1$ for the two quotient generators. On

$$
L_r=\langle v_0,\ldots,v_r,w_1,\ldots,w_r\rangle_k
$$

put $xv_0=0$, $xv_i=w_i$ for $1\le i\le r$, $yv_i=w_{i+1}$ for $0\le i<r$, $yv_r=0$, and $xw_i=yw_i=0$. All products of $x,y$ are zero, so the relations $x^p=y^p=0$ and $xy=yx$ hold, including when $p=2$.

These modules are indecomposable. Their common kernel and radical are $W=\langle w_i\rangle$. An endomorphism preserves $W$; let $A$ be its induced matrix on $L_r/W$ and $C$ its matrix on $W$. The equations $CX=XA$, $CY=YA$ for the two displayed shift maps force $A$ and $C$ to be the same scalar: the first and last columns give the boundary zeroes, and the recurrence $a_{j,i+1}=a_{j-1,i}$ forces all off-diagonal entries to vanish and all diagonal entries to agree. The remaining endomorphisms map the top into $W$ and vanish on $W$, so form a square-zero ideal. Thus the endomorphism ring is local. Inflate $L_r$ to $D$ and choose the infinitely many $r$ for which $p\nmid 2r+1$. Such an $L_r$ has vertex $D$: if $1=\operatorname{Tr}_Q^D(\alpha)$ for a proper $Q<D$, taking ordinary matrix traces would give

$$
2r+1=[D:Q]\operatorname{tr}(\alpha)=0\quad\text{in }k,
$$

a contradiction. Their distinct dimensions ensure distinct isomorphism classes.

Each $F(L_r)=e_b\operatorname{Ind}_D^N L_r$ is nonzero, by exactness and the already proved $F(k)\ne0$. Its restriction to $D$ is a summand of a sum of conjugates of $L_r$, by normality of $D$ and [Mackey decomposition](../../../../../mackey-restriction-formula.md). Consequently every indecomposable summand chosen from $F(L_r)$ has vertex $D$, and has a source conjugate to $L_r$. If $b$ contained only finitely many indecomposables, their restrictions to $D$ would contain only finitely many possible sources, contradicting this family. Green correspondence and Nagao's theorem then transfer infinitely many vertex-$D$ indecomposables in $b$ to distinct indecomposables in $B$. We have proved

$$
\boxed{B\text{ has finite representation type}\iff D\text{ is cyclic}.}
$$

Finally, for $C_p=\langle g\rangle$, the algebra $kC_p=k[t]/(t^p)$ has precisely the indecomposables

$$
\boxed{M_j=k[t]/(t^j),\qquad 1\le j\le p.}
$$

On $M_j$, $g$ acts as a single size-$j$ Jordan block with eigenvalue $1$. Its submodules are exactly its ideals, hence the powers of $t$: an ideal has a generator of least degree, and multiplying that generator by a unit makes it a power of $t$. Therefore its unique [composition series of a module](../../../../../composition-series-of-a-module.md) is

$$
0=t^jM_j\subset t^{j-1}M_j\subset\cdots\subset tM_j\subset M_j,
$$

with $j$ trivial one-dimensional [composition factors](../../../../../composition-factor.md). This is uniqueness of the actual chain, stronger than uniqueness of the multiset of factors. The algebra is local, so its sole [principal indecomposable module](../../../../../principal-indecomposable-module.md) is its regular module **$M_p=kC_p$**, of dimension and composition length $p$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
