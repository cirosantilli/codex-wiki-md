<h1 id="16f/solution">Solution</h1>

↑ **Parent:** [16F](../16f.md)

The [Axiom of foundation](../../../../../axiom-of-regularity.md) states that every nonempty set $A$ has a member $a$ disjoint from $A$. The principle of membership induction states that a property $P$ satisfying $\forall x[(\forall y\in x\ P(y))\Rightarrow P(x)]$ holds for every set.

Assume Foundation and suppose a progressive property fails at a set $x$. In the transitive closure of $\{x\}$, form the nonempty set of counterexamples by Separation. Foundation selects a counterexample $a$ with no counterexample among its members. Transitivity makes those members belong to the closure, so each satisfies $P$, and progressiveness gives $P(a)$, a contradiction. Conversely, if a nonempty $A$ had no member disjoint from it, the property $P(x):x\notin A$ would be progressive: a member of $A$ necessarily has a member in $A$. Membership induction would then say no set belongs to $A$, a contradiction. Thus **Foundation and membership induction are equivalent**.

Apply induction to the property that a set belongs to some stage of the [cumulative hierarchy](../../../../../cumulative-hierarchy.md). For each member $y$ of $x$, choose its least stage ordinal. Replacement collects these ordinals into a set; take an ordinal $\gamma$ large enough that all members lie in $V_\gamma$. Then $x\subseteq V_\gamma$ and $x\in V_{\gamma+1}$. This proves every set appears in the hierarchy.

For finite stages let $a_n=|V_n|$. Then $\boxed{a_0=0,\quad a_{n+1}=2^{a_n}}$, giving $0,1,2,4,16,65536,\ldots$. The stage $V_\omega$ is countably infinite, as the union of the finite stages. Thus $|V_{\omega+1}|=2^{\aleph_0}=|\mathbb R|$. Cantor's theorem makes $|V_{\omega+2}|$ strictly larger, and every later stage contains it. Earlier stages have at most countable size. Therefore $\boxed{|V_\alpha|=|\mathbb R|\iff\alpha=\omega+1}$.

## ↑ Ancestors (10)

1. [16F](../16f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
