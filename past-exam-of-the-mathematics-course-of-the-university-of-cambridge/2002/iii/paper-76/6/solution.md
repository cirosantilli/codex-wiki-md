<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Böhm tree](../../../../../bohm-tree.md) $BT(M)$ is $\bot$ if $M$ is an [unsolvable lambda term](../../../../../unsolvable-lambda-term.md). Otherwise choose a [head normal form](../../../../../head-normal-form.md)

$$
M\to_\beta^*\lambda x_1\cdots x_n.yM_1\cdots M_m.
$$

Its root is labeled by the binder prefix and head variable, and its ordered children are $BT(M_1),\ldots,BT(M_m)$. Repeat recursively, possibly forever. Bound names are identified by [alpha equivalence](../../../../../alpha-equivalence.md); the [Church-Rosser theorem](../../../../../church-rosser-theorem.md) makes this tree independent of the selected head reduct. An address $\alpha$ is a finite sequence of child numbers; $M_\alpha$ denotes the corresponding argument term encountered after these head reductions.

A [Böhm transformation](../../../../../bohm-transformation.md) is a finite composition of [capture-avoiding substitutions](../../../../../capture-avoiding-substitution.md) and applications to chosen auxiliary terms. Here is a constructive [Böhm-out lemma](../../../../../bohm-out-lemma.md). Along the finite path to $\alpha$, choose $q$ at least the number of children of each preceding head node, and define

$$
U_q=\lambda z_1\cdots z_q w.wz_1\cdots z_q,\qquad P_i^q=\lambda z_1\cdots z_q.z_i.
$$

Initially replace all relevant [free variables](../../../../../free-variable.md) by $U_q$. At a head node with $n$ initial binders and $m$ children, supply its $n$ binders with $U_q$. Its head is now $U_q$ and its arguments are the substituted children $N_1,\ldots,N_m$. Apply $q-m$ extra copies of $U_q$ as padding and then $P_i^q$. Direct [beta reduction](../../../../../beta-reduction.md) gives

$$
U_qN_1\cdots N_m\underbrace{U_q\cdots U_q}_{q-m}\,P_i^q\to_\beta^*N_i.
$$

Repeat with the next child number. The term reached at each stage is the selected original child with the accumulated substitutions for its ancestors' binders. Thus the finite composite $\pi$ satisfies **$M\pi\equiv_\beta M_\alpha\sigma$ for a suitable substitution $\sigma$**. The empty path uses the identity transformation. Tupling, rather than immediately replacing a head variable by a fixed projection, is important: the same variable can occur later where a different child must be selected.

For the [Böhm separation theorem](../../../../../bohm-separation-theorem.md), two distinct closed normal forms for both [beta reduction](../../../../../beta-reduction.md) and [eta conversion](../../../../../eta-conversion.md) have finite [Böhm trees](../../../../../bohm-tree.md) with a genuine disagreement in a head label or argument structure. A [Böhm transformation](../../../../../bohm-transformation.md) first extracts their common-prefix node. Projections at a differing head variable select different supplied [Church Booleans](../../../../../church-boolean.md); differing arities are handled by padding, with the exclusion of mere eta expansions ensuring a genuine disagreement. This yields a context separating the two normal forms. Distinct beta-normal forms that differ only by [eta conversion](../../../../../eta-conversion.md) are not covered by this separation statement.

The PDF prints a free $\alpha$ in both the definitions of $K$ and $\mathsf T$. Taken literally, this makes the last request impossible. To see why, suppose $M K_\alpha\equiv_\beta K_\alpha$, where $K_\alpha=\lambda xy.\alpha$, and choose a fresh $f$. By solvability and its stability under substitution, $Mf$ has a [head normal form](../../../../../head-normal-form.md) $\lambda x_1\cdots x_n.hP_1\cdots P_r$. If $h\ne f$, substituting either $K_\alpha$ or $S$ leaves the same variable-headed spine; it cannot be $K_\alpha$ in one case and $\mathsf F$ in the other. If $h=f$, obtaining $K_\alpha$ requires $r\le2$ and $n+2-r=2$, hence $n=r$. Substituting $S=\lambda xyz.xz(yz)$ then leaves at least $n+3-r=3$ leading abstractions, whereas $\mathsf F$ has two. A variable-headed normal form cannot lose initial abstractions under [beta reduction](../../../../../beta-reduction.md). The [Church-Rosser theorem](../../../../../church-rosser-theorem.md) rules out the required equality.

For the intended closed first projection $K=\mathsf T=\lambda xy.x$ and $\mathsf F=\lambda xy.y=KI$, an explicit answer is

$$
\boxed{M=\lambda f.f(KK)(KI)I.}
$$

Indeed $MK\to_\beta^*(KK)I\to_\beta K=\mathsf T$, whereas $MS\to_\beta^*(KK)I((KI)I)\to_\beta KI=\mathsf F$. These computations solve the corrected closed-combinator version while identifying the obstruction in the literal printed one.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
