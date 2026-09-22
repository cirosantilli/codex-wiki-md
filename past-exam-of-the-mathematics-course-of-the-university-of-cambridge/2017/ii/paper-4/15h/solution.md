<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

Use the convention that the [transitive closure](../../../../../transitive-closure.md) of $x$ is the least [transitive set](../../../../../transitive-set.md) containing $x$ as a subset. Define $x_0=x$ and $x_{n+1}=\bigcup x_n$. For each [natural number](../../../../../natural-number.md) $n$, a finite sequence of length $n+1$ with these properties exists by induction, and is unique because each next entry is the uniquely determined [union](../../../../../set-union.md) of the previous entry. Thus the relation sending $n$ to its last entry is a definable function-class, not just a putative recursive specification. The [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) applied to $\omega$ gives the set of all $x_n$. The [Axiom of union](../../../../../axiom-of-union.md) then gives

$$
\boxed{\operatorname{TC}(x)=\bigcup_{n<\omega}x_n.}
$$

If $a\in x_n$ and $b\in a$, then $b\in x_{n+1}$, so this set is transitive. It contains $x=x_0$, and any [transitive set](../../../../../transitive-set.md) containing $x$ contains all $x_n$ by induction; hence it is least. The convention requiring $x$ itself as an element instead uses $\operatorname{TC}(\{x\})$.

The [Axiom of foundation](../../../../../axiom-of-regularity.md) says every nonempty set $A$ has an element $a\in A$ with $a\cap A=\varnothing$. [Epsilon induction](../../../../../epsilon-induction.md) says that for every formula $\phi$,

$$
[\forall x\,((\forall y\in x\,\phi(y))\Rightarrow\phi(x))]\Rightarrow\forall x\,\phi(x).
$$

To derive induction from Foundation, if $\phi(x)$ fails, form by [axiom schema of separation](../../../../../axiom-schema-of-specification.md) the nonempty set of counterexamples in $\operatorname{TC}(\{x\})$. A Foundation-minimal counterexample has every member satisfying $\phi$, by transitivity, contradicting the inductive hypothesis. Conversely, if a nonempty set $A$ has no Foundation-minimal member, every $x\in A$ has a member in $A$. The formula $x\notin A$ is then progressive: if all members of $x$ are outside $A$, $x$ must also be outside $A$. [Epsilon induction](../../../../../epsilon-induction.md) makes $A$ empty, a contradiction. Thus the two principles are equivalent given the other axioms.

The [epsilon-recursion theorem](../../../../../epsilon-recursion-theorem.md) states that for a definable class operation $G$ assigning a unique set to each set-indexed function, there is a unique definable function-class $F$ such that $F(x)=G(F|_x)$ for every set $x$. A version with explicit $x$ in the argument is equivalent. Foundation gives well-foundedness and Replacement makes each restriction set-sized. Its ordinal restriction gives [transfinite recursion](../../../../../transfinite-recursion.md) and constructs the printed $C_\alpha$.

Here “countable” means at most countable, including finite sets and the [empty set](../../../../../empty-set.md). By [transfinite induction](../../../../../transfinite-induction.md) each $C_\alpha$ is transitive, each of its elements is countable, and $C_\alpha\subseteq C_{\alpha+1}$. At a successor this follows because a member of $C_\alpha$ is a countable subset of $C_\alpha$; at a [limit](../../../../../limit-of-a-function.md) use the increasing [union](../../../../../set-union.md). Let $\omega_1$ be the [first uncountable ordinal](../../../../../first-uncountable-ordinal.md). Every countable subset of $C_{\omega_1}$ lies in some $C_\alpha$ with $\alpha<\omega_1$, since countably many [countable ordinal](../../../../../countable-ordinal.md) bounds have a countable supremum. It therefore belongs to $C_{\alpha+1}$. Consequently

$$
\boxed{C_{\omega_1+1}=C_{\omega_1}.}
$$

There is no earlier stabilization: for every [countable ordinal](../../../../../countable-ordinal.md) $\alpha$, induction gives $\alpha\subseteq C_\alpha$, so $\alpha\in C_{\alpha+1}$, while $C_\alpha\subseteq V_\alpha$ excludes $\alpha$ by its rank. Thus $\omega_1$ is the first such stage. The fixed set is the set of [hereditarily countable sets](../../../../../hereditarily-countable-set.md).

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
