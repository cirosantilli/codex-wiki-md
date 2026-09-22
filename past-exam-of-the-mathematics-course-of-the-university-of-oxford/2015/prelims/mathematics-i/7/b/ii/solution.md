<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [free group action](../../../../../../../free-group-action.md), every [stabilizer subgroup](../../../../../../../stabilizer-subgroup.md) is $\{e\}$. By the [orbit-stabilizer theorem](../../../../../../../orbit-stabilizer-theorem.md), every [orbit of a group action](../../../../../../../orbit-group-theory.md) has [cardinality](../../../../../../../cardinality.md) $|G|$. Hence the two [free group actions](../../../../../../../free-group-action.md) have the same number

$$
r=\frac{|S|}{|G|}
$$

of [orbits of a group action](../../../../../../../orbit-group-theory.md). Choose one representative $s_i$ from each $\cdot$ [orbit of a group action](../../../../../../../orbit-group-theory.md) and one representative $t_i$ from each $*$ [orbit of a group action](../../../../../../../orbit-group-theory.md), and match them using $1\leq i\leq r$.

Every $s\in S$ has a unique expression $s=g\cdot s_i$. The [orbit of a group action](../../../../../../../orbit-group-theory.md) determines $i$, and the [free group action](../../../../../../../free-group-action.md) property determines $g$: if $g\cdot s_i=h\cdot s_i$, then $(h^{-1}g)\cdot s_i=s_i$, forcing $g=h$. Therefore the rule

$$
\boxed{f(g\cdot s_i)=g*t_i}
$$

defines a [function](../../../../../../../function-split.md) $f:S\to S$ without ambiguity. For $h\in G$,

$$
f\bigl(h\cdot(g\cdot s_i)\bigr)
=f\bigl((hg)\cdot s_i\bigr)
=(hg)*t_i
=h*(g*t_i)
=h*f(g\cdot s_i),
$$

which proves the required identity for every $s$.

Indeed, $f$ is a [bijection](../../../../../../../bijection.md): its inverse is $g*t_i\mapsto g\cdot s_i$, well defined because the second is also a [free group action](../../../../../../../free-group-action.md). If $S$ is empty, the unique empty [function](../../../../../../../function-split.md) already satisfies the identity. Thus the result holds in every case, and proves the stronger statement that [free finite actions with equal cardinality are isomorphic](../../../../../../../free-finite-actions-with-equal-cardinality-are-isomorphic.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
