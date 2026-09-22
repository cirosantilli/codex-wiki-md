<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $N=N_G(D)$, $C=C_G(D)$, and use the commutative transfer [ideals](../../../../../../ideal.md)

$$
I_D=\operatorname{Tr}_D^G((kG)^D)\subseteq Z(kG),\qquad
J_D=\operatorname{Tr}_D^N(kC)\subseteq(kC)^N.
$$

The target fixed [algebra](../../../../../../algebra-split.md) is commutative, because $C\le N$ makes every $N$-fixed element of $kC$ central in $kC$.

The [Brauer morphism and relative trace](../../../../../../brauer-morphism-and-relative-trace.md) identity is

$$
\operatorname{Br}_D(\operatorname{Tr}_D^G a)=\operatorname{Tr}_D^N(\operatorname{Br}_D a).
$$

Indeed let $D$ act on $G/D$ by left multiplication in the trace sum. Its fixed cosets are exactly $gD$ with $g\in N$; every other orbit has size divisible by $p$. After Brauer projection the contributions on each such nonfixed orbit are equal, so they cancel. Fixed cosets give precisely the right-hand side. Since the Brauer projection of $(kG)^D$ is all of $kC$, this proves a surjection **$I_D\twoheadrightarrow J_D$**.

We use the [trace criterion for defect groups](../../../../../../trace-criterion-for-defect-groups.md): a block [idempotent](../../../../../../idempotent.md) $e$ belongs to $I_D$ exactly when its defect [group](../../../../../../group-split.md) is conjugate into $D$; among these, $\operatorname{Br}_D(e)\ne0$ exactly when its defect [group](../../../../../../group-split.md) is $D$ up to conjugacy. The criterion can be read from the class-sum basis: if $E=C_D(x)$ then

$$
\operatorname{Tr}_D^G(\operatorname{Tr}_E^D x)
=\operatorname{Tr}_E^G x=[C_G(x):E]\,[x^G].
$$

This coefficient is nonzero exactly when $E$ is a Sylow $p$-subgroup of $C_G(x)$. Thus $I_D$ is spanned by classes whose class defect is conjugate into $D$, and the kernel of its Brauer projection is the sum of the corresponding proper-subgroup transfer [ideals](../../../../../../ideal.md). The block version follows by refinement of the [central idempotents](../../../../../../central-idempotent.md) in these [ideals](../../../../../../ideal.md).

For clarity, the refinement fact needed here is [primitive idempotents under a surjection of commutative Artinian ideals](../../../../../../primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals.md): a surjection between [ideals](../../../../../../ideal.md) of commutative Artinian [algebras](../../../../../../algebra-split.md) bijects the [primitive idempotents](../../../../../../primitive-idempotent.md) in the [module source](../../../../../../source-of-an-indecomposable-module.md) whose images are nonzero with the [primitive idempotents](../../../../../../primitive-idempotent.md) in the target. Decompose the [algebras](../../../../../../algebra-split.md) into local factors. An [ideal](../../../../../../ideal.md) in a local Artinian factor either contains the identity and is the whole factor, or lies in its nilpotent maximal [ideal](../../../../../../ideal.md) and has no nonzero [idempotents](../../../../../../idempotent.md). A surviving local factor has a local quotient, so its identity remains primitive. This proves the stated refinement fact without imposing nilpotence on the entire kernel.

The [primitive idempotents](../../../../../../primitive-idempotent.md) in $I_D$ are the block [idempotents](../../../../../../idempotent.md) with defect conjugate into $D$, and the surviving ones have defect $D$. Applying refinement to the surjection above gives

$$
\boxed{e\longmapsto\operatorname{Br}_D(e):
\{\text{blocks of }G\text{ with defect }D\}\ \longleftrightarrow\
\{\text{primitive idempotents of }J_D\}.}
$$

This is the [Brauer morphism on a defect transfer ideal](../../../../../../brauer-morphism-on-a-defect-transfer-ideal.md); the target is the transfer [ideal](../../../../../../ideal.md) $J_D$, not the entire fixed [center of an associative algebra](../../../../../../center-of-an-associative-algebra.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
