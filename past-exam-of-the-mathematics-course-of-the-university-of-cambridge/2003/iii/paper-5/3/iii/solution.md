<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The required [quasi-isometry](../../../../../../quasi-isometry.md) is the identity on the group vertices. For each $a\in A$ choose a fixed $B$-word $T(a)$ representing it and map an $a$-edge to that word [path](../../../../../../continuous-path.md). The bounded substitutions in Q2(ii) prove the distortion inequalities.

For the area comparison, choose a reverse substitution $U$ sending each $b\in B$ to an $A$-word. Let $L$ bound the lengths of $T(a)$. Every word $U(s)$ for a defining [relator](../../../../../../relator.md) $s\in S$ is null over the first [group presentation](../../../../../../group-presentation.md). Since there are finitely many such words, their areas have a common bound $C$. Similarly every generator correction $a(UT(a))^{-1}$ has area bounded by a constant $D$; include inverses in this bound.

Let $w$ be null over $A$ with length at most $n$. Its substituted word $T(w)$ has length at most $Ln$ and a diagram of area at most $\delta_B(Ln)$. Replace each $B$-edge by its $U$-path. Each original [relator](../../../../../../relator.md) face can then be filled over $A$ using at most $C$ faces, so $UT(w)$ has area at most $C\delta_B(Ln)$. Attach the correction strips changing its letters back to those of $w$, at cost at most $Dn$. Therefore

$$
\boxed{\delta_A(n)\le C\delta_B(Ln)+Dn}.
$$

The reverse substitutions give the corresponding inequality for $\delta_B$. Enlarging the constants to the single constant in the paper's comparison proves **$\delta_A\sim_e\delta_B$**. This is [Dehn functions under a change of finite presentation](../../../../../../dehn-functions-under-a-change-of-finite-presentation.md).

Two qualifications are necessary for the printed continuation. The invariant is the optimal [isoperimetric function](../../../../../../isoperimetric-function-of-a-group-presentation.md), namely the [Dehn function](../../../../../../dehn-function.md), not arbitrary upper bounds. For example, the relator-free [group presentation](../../../../../../group-presentation.md) of $\mathbb Z$ has zero area on all null words, so both $n$ and $2^n$ are isoperimetric upper bounds for that same [group presentation](../../../../../../group-presentation.md); they are not equivalent under $\sim_e$.

Also, the comparison supplies no recursive bound unless one was available beforehand. Its actual consequence, by part (ii), is

$$
\boxed{\text{one finite presentation of }G\text{ has decidable word problem}\ \Longleftrightarrow\ \text{every finite presentation of }G\text{ does}.}
$$

The unconditional assertion that every [finitely presented group](../../../../../../finitely-presented-group.md) has a solvable [word problem](../../../../../../word-problem-for-groups.md) is false. Finitely presented counterexamples are established in the primary paper [The Word Problem](https://www.jstor.org/stable/1970103). Thus the missing solvability premise cannot be inferred from [group presentation](../../../../../../group-presentation.md) equivalence alone.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
