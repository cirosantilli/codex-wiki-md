<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A finite-dimensional [group algebra](../../../../../group-algebra.md) has [finite representation type of a group algebra](../../../../../finite-representation-type-of-a-group-algebra.md) when there are only finitely many isomorphism classes of finite-dimensional [indecomposable modules](../../../../../indecomposable-module.md). The definition concerns all dimensions, not merely finitely many [modules](../../../../../module-mathematics.md) in each fixed dimension.

Let $e_B$ be the block [idempotent](../../../../../idempotent.md) and choose a maximal [Brauer pair](../../../../../brauer-pair.md) $(D,b_D)$: $b_D$ is a block [idempotent](../../../../../idempotent.md) of $kC_G(D)$ with $b_D\operatorname{Br}_D(e_B)\ne0$. The [inertial index of a block](../../../../../inertial-index-of-a-block.md) is

$$
\boxed{e(B)=|N_G(D,b_D):DC_G(D)|,}
$$

where $N_G(D,b_D)$ is the stabilizer of the chosen pair. Changing the pair by conjugation does not alter this number. For cyclic $D$, it is a prime-to-$p$ divisor of $p-1$. Here $n\ge1$, as required for the order-$p$ [subgroup](../../../../../subgroup.md) $Q$ to exist.

Put $H=N_G(Q)$. Since $Q$ is characteristic in $D$, $N_G(D)\le H$, so [Green correspondence](../../../../../green-correspondence.md) applies. In fact the nonprojective [modules](../../../../../module-mathematics.md) in $B$ have a particularly simple correspondence. If $g\notin H$, a nontrivial intersection $D\cap{}^gD$ would contain the unique order-$p$ [subgroup](../../../../../subgroup.md) of both cyclic [groups](../../../../../group-split.md), giving $Q={}^gQ$ and hence $g\in H$, a contradiction. Thus every such intersection is trivial. The error [modules](../../../../../module-mathematics.md) in induction are projective. In restriction, an intersection $H\cap{}^gD$ cannot contain a conjugate of a nontrivial [subgroup](../../../../../subgroup.md) of $D$ by an element of $H$: such a conjugate contains $Q$, and that would again force ${}^gQ=Q$. The general [Green correspondence](../../../../../green-correspondence.md) therefore pairs all [indecomposable modules](../../../../../indecomposable-module.md) with nontrivial [module vertex](../../../../../vertex-of-an-indecomposable-module.md) contained in a conjugate of $D$. In particular it pairs the nonprojective [modules](../../../../../module-mathematics.md) of $B$ with the nonprojective [modules](../../../../../module-mathematics.md) of its Brauer correspondent $b$ in $H$; the block-compatible form of the correspondence selects $b$. Explicitly,

$$
M\downarrow_H=f(M)\oplus M_{\mathcal Y},\qquad
f(M)\uparrow^G=M\oplus P,
$$

where $P$ is projective and the restriction error family is $\mathcal Y=\{H\cap{}^gD:g\notin H\}$. One should not replace this restriction error term by projectives without an additional argument about $H$.

For the final structure calculation we use the general cyclic-defect structure theorem, which is permitted here as a general fact: the basic [algebra](../../../../../algebra-split.md) of a split [block with cyclic defect group](../../../../../block-with-cyclic-defect-group.md) is a [Brauer tree algebra](../../../../../brauer-tree-algebra.md). Its tree has $e(B)$ edges, one simple [module](../../../../../module-mathematics.md) per edge, and exceptional multiplicity

$$
m=\frac{|D|-1}{e(B)}.
$$

For a one-edge tree the basic [algebra](../../../../../algebra-split.md) presentation is $k[t]/(t^{m+1})$. This is the local presentation of the tree [algebra](../../../../../algebra-split.md), not an assertion that an arbitrary block with one simple [module](../../../../../module-mathematics.md) is automatically uniserial.

With $e(B)=1$ the tree has one edge and $m=p^n-1$. Thus the basic [algebra](../../../../../algebra-split.md) of $B$ is

$$
A_0=k[t]/(t^{p^n}).
$$

It has exactly one simple [module](../../../../../module-mathematics.md), $k=A_0/(t)$. Its [ideals](../../../../../ideal.md) are precisely $(t^i)$: for any nonzero element, factor out its lowest power of $t$, after which the remaining factor is a unit. The regular projective therefore has the unique submodule chain

$$
A_0\supset tA_0\supset\cdots\supset t^{p^n-1}A_0\supset0,
$$

with each consecutive factor one-dimensional and simple. A [Morita equivalence](../../../../../morita-equivalence.md) from $A_0$ to $B$ preserves simple [modules](../../../../../module-mathematics.md), [projective covers](../../../../../projective-cover.md), submodule lattices and composition length. Hence

$$
\boxed{B\text{ has one simple module }S,\qquad P(S)\text{ is uniserial of length }p^n.}
$$

In the split setting one may also write $B\cong M_{\dim_k S}(A_0)$. The [projective cover](../../../../../projective-cover.md) has $p^n$ [composition factors](../../../../../composition-factor.md) all isomorphic to $S$, so its vector-space dimension is $p^n\dim_kS$, not generally $p^n$.

There is also an elementary reason why the uniserial conclusion follows once the one-simple-module conclusion and finite type are known. If the basic local [algebra](../../../../../algebra-split.md) had $\dim J/J^2\ge2$, quotienting its radical square and all but two generators would give $k[x,y]/(x,y)^2$. The two-dimensional parameter family from Question 3(b) would then give infinitely many indecomposables. Thus $J/J^2$ is one-dimensional. [Nakayama lemma](../../../../../nakayama-lemma.md) makes $J$ generated by one element $t$, so its powers yield a chain and the basic [algebra](../../../../../algebra-split.md) is $k[t]/(t^r)$. The cyclic-defect calculation above identifies $r=p^n$. This explains why finite representation type rules out branching in this [projective cover](../../../../../projective-cover.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
