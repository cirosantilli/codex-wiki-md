<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First work on an integral component. Write the [big real divisor](../../../../../../big-real-divisor.md) as $D\sim_{\mathbb R}B+E$ with $B$ [ample real divisor](../../../../../../ample-real-divisor.md) and $E$ effective real Cartier, using [Kodaira's lemma](../../../../../../kodaira-s-lemma.md). Let $E_1,\ldots,E_k$ be the finitely many integral components of its support. For an integral [projective curve](../../../../../../projective-curve.md) $C$ not contained in this support, restriction of each effective Cartier summand to $C$ is effective, so

$$
D\cdot C=B\cdot C+E\cdot C>0.
$$

Therefore

$$
\boxed{D\cdot C<0\Longrightarrow C\subseteq E_i\text{ for some }i.}
$$

This proves [negative curves of a big real divisor lie in finitely many divisors](../../../../../../negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors.md).

Now let $A$ be the given [ample](../../../../../../ample-line-bundle.md) divisor. Openness of the [ample cone](../../../../../../ample-cone.md) gives a $\delta>0$ such that $B-\epsilon A$ is [ample](../../../../../../ample-line-bundle.md) for $0<\epsilon\le\delta$. For each of the finitely many $E_i$, the assumption that $D|_{E_i}$ is [ample](../../../../../../ample-line-bundle.md) similarly gives a $\delta_i>0$ such that $(D-\epsilon A)|_{E_i}$ is [ample](../../../../../../ample-line-bundle.md) for $0<\epsilon\le\delta_i$. Choose a single positive $\epsilon$ smaller than all these bounds.

If $C$ is contained in some $E_i$, its intersection with $D-\epsilon A$ is positive by that restriction. Otherwise

$$
(D-\epsilon A)\cdot C=(B-\epsilon A)\cdot C+E\cdot C>0.
$$

In particular $D-\epsilon A$ is [nef](../../../../../../nef-line-bundle.md):

$$
\boxed{D-\epsilon A\text{ is nef for all sufficiently small }\epsilon>0.}
$$

Only the finitely many exceptional support components are needed for the restriction test; no uniform bound over all [subvarieties](../../../../../../closed-subvariety.md) was assumed.

For a reducible [projective scheme](../../../../../../projective-scheme.md), use [componentwise bigness on a projective scheme](../../../../../../componentwise-bigness-on-a-projective-scheme.md) and repeat this argument on each reduced irreducible component. Collect their exceptional supports and take the minimum of all the finitely many positive bounds. Codimension one here is measured in the relevant irreducible component. Every integral curve lies in a component, so the same conclusion holds on $X$. Nilpotent structure does not affect these curve [intersection numbers](../../../../../../intersection-number-of-a-cartier-divisor-with-a-curve.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 134](../../../paper-134-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
