<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take finite-dimensional modules over $k$ and finite $R$-free lattices over the complete valuation ring, the usual integral [modular representation theory](../../../../../modular-representation-theory.md) convention. If a completion has several local factors, use the factor supporting the [modular block](../../../../../block-of-a-group-algebra.md). A [block of a group algebra](../../../../../block-of-a-group-algebra.md) is an indecomposable two-sided ideal $B=RGb$, where $b$ is a [primitive central idempotent](../../../../../primitive-central-idempotent.md). The identity decomposes as the sum of orthogonal block idempotents, and $M=\bigoplus_b bM$ for every [module](../../../../../module-mathematics.md). Hence an [indecomposable module](../../../../../indecomposable-module.md) belongs to $B$ exactly when $bM=M$.

A [defect group of a block](../../../../../defect-group-of-a-block.md) in characteristic $p$ is a maximal [p-subgroup](../../../../../p-subgroup.md) $D$ with $\operatorname{Br}_D(b)\ne0$. Equivalently, it is minimal with $b\in\operatorname{Tr}_D^G((kG)^D)$; the [trace criterion for defect groups](../../../../../trace-criterion-for-defect-groups.md) and conjugacy are proved below. For a complete [discrete valuation ring](../../../../../discrete-valuation-ring.md), use the corresponding reduced [modular block](../../../../../block-of-a-group-algebra.md); [modular reduction of block idempotents](../../../../../modular-reduction-of-block-idempotents.md) preserves its [defect groups](../../../../../defect-group-of-a-block.md). The equivalent [bimodule](../../../../../bimodule.md) description says that the [module vertices](../../../../../vertex-of-an-indecomposable-module.md) of $B$, with $(x,y)$ acting by $a\mapsto xay^{-1}$, are conjugates of $\Delta D=\{(d,d):d\in D\}$. This basic characterization follows from the relative-projectivity trace criterion for the [bimodule](../../../../../bimodule.md) action.

Fix a [Sylow subgroup](../../../../../sylow-subgroup.md) $P$ containing $D$. The regular [group algebra](../../../../../group-algebra.md) is the [permutation module](../../../../../permutation-module.md) $R[G]$ for $G\times G$, and multiplication by $b$ is its block projection. Restriction to a subgroup containing a chosen [module vertex](../../../../../vertex-of-an-indecomposable-module.md) retains a summand with that [module vertex](../../../../../vertex-of-an-indecomposable-module.md): a [module source](../../../../../source-of-an-indecomposable-module.md) at that [module vertex](../../../../../vertex-of-an-indecomposable-module.md) is a summand of the [module restriction](../../../../../restriction-of-a-representation.md), and the [Mackey restriction formula](../../../../../mackey-restriction-formula.md) and minimality prevent all the restricted summands from having smaller [module vertices](../../../../../vertex-of-an-indecomposable-module.md). Thus $B\downarrow_{P\times P}$ has an indecomposable summand with [module vertex](../../../../../vertex-of-an-indecomposable-module.md) $\Delta D$.

For a [finite p-group](../../../../../finite-p-group.md) $Q$, the transitive [permutation module](../../../../../permutation-module.md) $k[Q/L]$ is indecomposable: the [group algebra of a p-group in characteristic p is local](../../../../../group-algebra-of-a-p-group-in-characteristic-p-is-local.md), and this module has a one-dimensional top, incompatible with a sum of two nonzero modules. Its [module vertex](../../../../../vertex-of-an-indecomposable-module.md) is $L$, because it is induced from the trivial $L$-module and its [Brauer quotient of a module](../../../../../brauer-quotient-of-a-module.md) at $L$ has the nonzero fixed [coset](../../../../../coset.md) $L$. The fixed-basis rule for this quotient follows by removing nonsingleton orbit sums, which are proper-subgroup traces. It excludes a smaller [module vertex](../../../../../vertex-of-an-indecomposable-module.md). Reduction gives the same statements for permutation lattices. Therefore [Krull-Schmidt decomposition](../../../../../krull-schmidt-decomposition.md) identifies the chosen block summand with an entire transitive $P\times P$ orbit in $G$.

Choose a point $c$ in that orbit whose stabilizer is exactly $\Delta D$. Being fixed by every $(d,d)$ gives $c\in C_G(D)$. Its full stabilizer is

$$
\{(cyc^{-1},y):y\in P\cap c^{-1}Pc\}.
$$

Equality with $\Delta D$ gives $P\cap c^{-1}Pc=D$. Conjugating, and using that $c$ centralizes $D$, proves

$$
\boxed{D=P\cap cPc^{-1},\qquad c\in C_G(D).}
$$

This is [defect groups are centralizer-conjugate Sylow intersections](../../../../../defect-groups-are-centralizer-conjugate-sylow-intersections.md).

If $Q\triangleleft G$ is a [p-subgroup](../../../../../p-subgroup.md), then $QP$ is a [p-subgroup](../../../../../p-subgroup.md) for every Sylow $P$, so $QP=P$. It lies in both Sylow factors above. Thus **every normal [p-subgroup](../../../../../p-subgroup.md) of $G$ is contained in $D$**.

Finally put $N=N_G(D)$, choose $S\in\operatorname{Syl}_p(N)$, and extend it to a Sylow $P$ of $G$. Then $D\leq S$ and $P\cap N=S$. Apply the proved intersection result to this $P$. Its element $c$ belongs to $C_G(D)\leq N$, so $cPc^{-1}\cap N=cSc^{-1}$ is Sylow in $N$ too. Hence $D=S\cap cSc^{-1}$. The [p-core](../../../../../p-core.md) $O_p(N)$ is contained in both factors, whereas normality of $D$ in $N$ gives the opposite inclusion. Therefore **$D=O_p(N_G(D))$**, so $D$ is a [p-radical subgroup](../../../../../p-radical-subgroup.md). The [centralizer](../../../../../centralizer.md) condition on the conjugating element is important for this deduction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
