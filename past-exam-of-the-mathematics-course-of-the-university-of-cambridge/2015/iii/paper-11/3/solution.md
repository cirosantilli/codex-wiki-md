<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We use the standard convention that a [two-intersecting family](../../../../../two-intersecting-family.md) satisfies $|A\cap B|\geq2$ for every pair of members, including $A=B$. In particular every member has at least two elements.

**An [intersecting shadow lemma](../../../../../intersecting-shadow-lemma.md).** If $\mathcal F$ is an [intersecting family](../../../../../intersecting-family.md) of $r$-sets, $r\geq1$, then

$$
|\partial\mathcal F|\geq|\mathcal F|.
$$

Here is a proof, so no additional shadow theorem is being assumed. For $i<j$, an [elementary set shift](../../../../../elementary-set-shift.md) replaces a member $A$ containing $j$ but not $i$ by $(A\setminus\{j\})\cup\{i\}$ exactly when that replacement is not already in the family. This preserves cardinality and the [intersecting family](../../../../../intersecting-family.md) property. The only potentially troublesome pair consists of a moved member and an unmoved member $B$ containing $j$ but not $i$. But then $B$'s replacement was already present, and the two original members obtained by using that replacement would have been disjoint if the new pair were disjoint.

Also

$$
\partial(S_{ij}\mathcal F)\subseteq S_{ij}(\partial\mathcal F),
$$

so an [elementary set shift](../../../../../elementary-set-shift.md) cannot increase the [lower shadow](../../../../../lower-shadow.md). For completeness, a shadow set containing neither $i,j$ or both has an unchanged witness in the original [lower shadow](../../../../../lower-shadow.md). A shadow set containing $i$ but not $j$ is either originally present or the replacement of an originally present shadow set. If a shadow set contains $j$ but not $i$, its witnessing member survived the [elementary set shift](../../../../../elementary-set-shift.md); either that member contains both coordinates, or its replacement was already present. In either case both the shadow set and its replacement were originally present, so the former survives in the shifted [lower shadow](../../../../../lower-shadow.md).

Repeated [elementary set shifts](../../../../../elementary-set-shift.md) terminate because the sum of the elements of all members decreases whenever the family changes. In the resulting [shifted set family](../../../../../shifted-set-family.md) $\mathcal H$, if $a_1<\cdots<a_r$ is a member and $b_1<\cdots<b_r$ satisfies $b_i\leq a_i$ for every $i$, then $\{b_1,\ldots,b_r\}$ is also a member. Every $A\in\mathcal H$ has a prefix $[2q-1]$ containing $q$ of its elements. Otherwise its sorted elements satisfy $a_i\geq2i$, and the first $r$ elements outside $A$ form a disjoint member componentwise no larger than $A$, contradicting the [intersecting family](../../../../../intersecting-family.md) property.

Choose the first such prefix and reflect membership inside it:

$$
D=\bigl(A\setminus[2q-1]\bigr)\cup\bigl([2q-1]\setminus A\bigr).
$$

This has size $r-1$. The set $D\cup\{2q-1\}$ is componentwise no larger than $A$: before the first excess, the prefix counts of $A$ are at most half the prefix length, and reflection only moves selected positions to the left. Thus $D$ belongs to $\partial\mathcal H$. This [ballot reflection injection](../../../../../ballot-reflection-injection.md) is injective: in $D$, the reflected prefix ends at the first position where unselected positions outnumber selected ones, and reflecting it again recovers $A$. Consequently $|\partial\mathcal H|\geq|\mathcal H|=|\mathcal F|$. Since [elementary set shifts](../../../../../elementary-set-shift.md) did not increase the [lower shadow](../../../../../lower-shadow.md), this proves the [intersecting shadow lemma](../../../../../intersecting-shadow-lemma.md).

**The [nonuniform two-intersecting family bound](../../../../../nonuniform-two-intersecting-family-bound.md).** Write $\mathcal A_i=\mathcal A\cap[n]^{(i)}$. No member of $\partial\mathcal A_i$ can be the complement of a member of $\mathcal A_{n-i+1}$: such an inclusion would make the intersection of the two original members have at most one element. The [intersecting shadow lemma](../../../../../intersecting-shadow-lemma.md) therefore gives

$$
|\mathcal A_i|+|\mathcal A_{n-i+1}|
\leq|\partial\mathcal A_i|+|\mathcal A_{n-i+1}|
\leq\binom n{i-1}.
$$

For $n=2h$, sum this over $1\leq i\leq h$. These pairs cover all nonempty levels, so

$$
\boxed{|\mathcal A|\leq\sum_{j=0}^{h-1}\binom nj
=\sum_{j=h+1}^{n}\binom nj.}
$$

Equality is attained by all subsets of size at least $h+1$: any two intersect in at least two elements.

For $n=2h+1$, the same pairs cover every level except $h+1$. Complements of the members of $\mathcal A_{h+1}$ form an [intersecting family](../../../../../intersecting-family.md) of $h$-sets, since

$$
|A^c\cap B^c|=|A\cap B|-1\geq1.
$$

For $h\geq1$, the permitted [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md) bounds this middle level by $\binom{2h}{h-1}=\binom{2h}{h+1}$. Hence

$$
\boxed{|\mathcal A|\leq\binom{n-1}{(n+1)/2}
+\sum_{j=(n+3)/2}^{n}\binom nj.}
$$

Equality is attained by all $(h+1)$-sets inside $[2h]$, together with all subsets of $[2h+1]$ of size at least $h+2$. Two members of the first group intersect in at least two elements; a member from each group intersects in at least two; two members of the second group intersect in at least three. For $n=1$ the only [two-intersecting family](../../../../../two-intersecting-family.md) is empty, which also gives equality. The empty-ground-set case is likewise immediate.

**The [pair-cover bound for a two-intersecting uniform family](../../../../../pair-cover-bound-for-a-two-intersecting-uniform-family.md).** If $\mathcal A$ is nonempty, fix $A_0\in\mathcal A$, with $|A_0|=r$. Every member contains one of the $\binom r2$ pairs inside $A_0$. Each fixed pair belongs to exactly $\binom{n-2}{r-2}$ $r$-sets, so counting their union gives

$$
\boxed{|\mathcal A|\leq\binom r2\binom{n-2}{r-2}.}
$$

The empty family is immediate; a nonempty [two-intersecting family](../../../../../two-intersecting-family.md) requires $r\geq2$.

**[Witness-pair concentration for an intersecting uniform family](../../../../../witness-pair-concentration-for-an-intersecting-uniform-family.md).** Let $\mathcal A$ now be an [intersecting family](../../../../../intersecting-family.md) of $r$-sets. If it is [two-intersecting](../../../../../two-intersecting-family.md), the preceding bound, together with $\binom r2\leq(r-1)^2$ for $r\geq2$, shows that any chosen $x\in[n]$ has the required property. Otherwise there are members $A,B$ with $A\cap B=\{x\}$. Every member $C$ not containing $x$ must contain some $a\in A\setminus\{x\}$ and some $b\in B\setminus\{x\}$. These two sets of possible witnesses are disjoint. There are $(r-1)^2$ witness pairs, and each is contained in $\binom{n-2}{r-2}$ $r$-sets. Thus

$$
\boxed{|\{C\in\mathcal A:x\notin C\}|\leq(r-1)^2\binom{n-2}{r-2}.}
$$

For $r=1$, a nonempty [intersecting family](../../../../../intersecting-family.md) consists of one singleton; choose its element and the number avoiding it is zero. This is the natural separate interpretation of the degenerate case, where the printed [binomial coefficient](../../../../../binomial-coefficient.md) has lower index $-1$. For an empty family any $x\in[n]$ works, provided $n\geq1$ as usual.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
